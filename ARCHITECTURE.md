# สถาปัตยกรรมแอป (Architecture)

## ภาพรวม 3 ชั้น

```mermaid
flowchart TB
  subgraph UX["📱 ชั้นหน้าจอ (115 Views)"]
    V1["ฟอร์มรับงาน/สแกน"]
    V2["ตารางติดตาม + สรุป"]
    V3["หน้าจอแยกตามบทบาท (Show if: USERROLE)"]
  end
  subgraph LOGIC["⚙️ ชั้นตรรกะ"]
    C1["สูตร App Formula / Initial Value (ใน 2,304 คอลัมน์)"]
    C2["Actions 214 ตัว (SET_COLUMN_VALUE, พิมพ์, เปิดแผนที่, Email)"]
    C3["Bots ~30 ตัว: พิมพ์ใบวางบิลตามคลัง · Telegram · GoogleMapsRoutesAPI"]
  end
  subgraph DATA["💾 ชั้นข้อมูล (Google Sheets + Native)"]
    D1["📋 29 ตารางธุรกิจหลัก"]
    D2["🤖 60 ตาราง Process/Output ของ Bot"]
  end
  V1 --> C2 --> D1
  V2 --> C1 --> D1
  C2 --> C3 --> D2 --> D1
```

## แผนภาพความสัมพันธ์ของตารางหลัก (Ref Relations)

เส้นเชื่อมด้านล่างอ่านจากคอลัมน์ชนิด `Ref` ในเอกสารจริงทั้งหมด (16 เส้น ระหว่างตารางหลัก) ลูกศรชี้จาก "ตารางที่มีคอลัมน์ Ref" ไปหา "ตารางที่ถูกอ้างถึง"

```mermaid
flowchart LR
  NAcknowledgeL8818["Acknowledge_Logs"]
  NAnnouncement2258["Announcements"]
  NDocReturn3089["Doc_Return"]
  NImageDocRetu9168["Image_Doc_Return"]
  NSCGJWD8918["SCGนครหลวงJWDภูมิภาค"]
  NScanDocs7857["ScanDocs"]
  NX5236["ข้อมูลการวางบิล"]
  NX6329["ข้อมูลการเข้าบำรุงรักษา"]
  NRT6764["ข้อมูลงานRT"]
  NX8283["ข้อมูลพนักงาน"]
  NX2249["ตารางงานประจำวัน"]
  NScg401["ทำเบิกส่วนต่างScgวังน้อย"]
  N2001559["รับงานคืนได้เงิน200"]
  NX5809["สรุปเบิกส่วนต่าง"]
  NX1431["ส่งงานที่ยังไม่มีข้อมูลในระบบ"]
  NX9490["แจ้งปัญหาระหว่างวัน"]
  NSCGJWD8918 -->|"ID_Doc_Return"| NDocReturn3089
  NSCGJWD8918 -->|"SM_Link_SCG"| NX2249
  NSCGJWD8918 -->|"ID_พนักงาน"| NX8283
  NX6329 -->|"ID_พนักงาน"| NX8283
  NX5236 -->|"ID_พนักงาน"| NX8283
  NX9490 -->|"SM_Link"| NX2249
  NX9490 -->|"RT_Link"| NRT6764
  NX9490 -->|"ID_พนักงาน"| NX8283
  N2001559 -->|"ID_พนักงาน"| NX8283
  NX5809 -->|"_ComputedKey_ID_SCGนครหลวงJW"| NSCGJWD8918
  NImageDocRetu9168 -->|"ID_Doc_Return"| NDocReturn3089
  NScg401 -->|"ID_SCGนครหลวงJWDภูมิภาค"| NSCGJWD8918
  NScg401 -->|"ID_พนักงาน"| NX8283
  NScanDocs7857 -->|"Invoice_No"| NX2249
  NX1431 -->|"ID_พนักงาน"| NX8283
  NAcknowledgeL8818 -->|"ID_ประกาศ"| NAnnouncement2258
```

ตารางหลักที่ไม่มี Ref เชื่อม (ใช้แบบสแตนด์อโลนหรือเชื่อมผ่านสูตร SELECT แทน): `ราคาน้ำมันดีเซล`, `ราคาในระบบก่อนส่งสินค้า`, `หน้าหลัก`, `ปริ๊นใบวางบิล`, `PDFพนักงาน`, `FILTER`, `ข้อมูลชื่องานต้นทางปลายทาง`, `ข้อมูลงานRW`, `สร้างเอกสาร`, `สรุป_เจ้าของสินค้า`, `สรุป_Shipment`, `PriceOverride`, `Price_Table`

## โมเดลสิทธิ์ผู้ใช้

```mermaid
flowchart TB
  U["👤 USER (พนักงาน)"] -->|เห็นเฉพาะแถวที่ [Email พนักงาน] = USEREMAIL| D["ตารางที่มี Security Filter"]
  U -->|ADDS_AND_UPDATES ลบไม่ได้| D
  A["👑 ADMIN"] -->|ALL_CHANGES + เห็นทุกแถว| D
  R["ระดับอื่น"] -->|READ_ONLY| D
```

ตารางที่ใช้ Security Filter รูปแบบ `=OR(USERROLE() = "ADMIN", [Email พนักงาน] = USEREMAIL())`: ดูรายการเต็มใน `docs/00_APP_OVERVIEW.md` และใน README ของแต่ละตาราง

## ชั้นระบบอัตโนมัติ (Bots)

สรุปกลุ่มงานอัตโนมัติจากร่องรอย Process/Output Tables (รายละเอียดเต็มใน [docs/06](docs/06_BOTS_AND_PROCESS_TABLES.md)):

| กลุ่มงาน | จำนวน (สันนิษฐาน) | เทคโนโลยีที่พบ |
|---|---:|---|
| พิมพ์ใบวางบิลแยกตามคลัง/ลูกค้า | ~12 | PDF/Printer Task |
| จัดเส้นทาง/คำนวณค่าส่งตามระยะทาง | 2 | GoogleMapsRoutesAPI |
| เบิกค่า/ส่วนต่าง/ค่ายกขึ้นชั้น | ~5 | Data Actions + สรุป |
| แจ้งเตือน/สื่อสาร | ~3 | Telegram, AppSheet_KM |
| สแกน/รับคืน/เอกสาร | ~4 | ScanStatus, Doc_Return |
| โอนคลัง (GQ จีคิว, MeSpace) | ~2 | Data Actions |

## ความสัมพันธ์ View ↔ ข้อมูล

- View ที่ map กับตาราง/slice ได้: **107/115** (อีก 8 เป็น view ระดับแอป เช่น dashboard)
- ชนิด View ที่ใช้มากที่สุด: `detail` (38), `form` (36), `table` (32), `deck` (8), `gallery` (1)

