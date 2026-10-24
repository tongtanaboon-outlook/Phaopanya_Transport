# 📋 ตารางข้อมูลหลัก: ตารางงานประจำวัน

> รหัสโฟลเดอร์: `T05_ตารางงานประจำวัน` · ลำดับในเอกสารต้นฉบับ: 5/90

| สรุป | จำนวน |
|---|---:|
| คอลัมน์ทั้งหมด | 40 |
| คอลัมน์ Key | 1 |
| คอลัมน์ Virtual (มีสูตรคำนวณ) | 0 |
| คอลัมน์ระบบ | 4 |
| Views | 10 |
| Actions | 10 |
| Slices | 5 |
| Format Rules | 3 |

## คุณสมบัติของตาราง

| มองเห็น (Visible) | ALWAYS |
| Shared | Yes |
| Locale ของข้อมูล | en-GB |
| Schema | ตารางงานประจำวัน_Schema |
| สิทธิ์การแก้ไขข้อมูล (Update mode) | ALL_CHANGES |
| Security Filter | ```=OR(USERROLE() = "ADMIN", [Email พนักงาน] = USEREMAIL())``` |
| Source Path | เผ่าปัญญา ทรานสปอร์ต |
| Worksheet (แท็บใน Google Sheets) | ตารางงานประจำวัน |
| โฟลเดอร์เก็บรูป/ไฟล์ | _Default |
| ลำดับคอลัมน์ | _RowNumber |
| Partition หลายไฟล์? | No |
| Partition หลายแท็บ? | No |

## 🔗 ความสัมพันธ์เข้า (ตารางอื่นอ้างถึง)

| ตาราง | คอลัมน์ | ชนิด |
|---|---|---|
| [SCGนครหลวงJWDภูมิภาค](T01_SCGนครหลวงJWDภูมิภาค/) | `SM_Link_SCG` | Ref |
| [แจ้งปัญหาระหว่างวัน](T11_แจ้งปัญหาระหว่างวัน/) | `SM_Link` | Ref |
| [ScanDocs](T23_ScanDocs/) | `Invoice_No` | Ref |
| [Process for Telegram_แจ้งปัญหา - 1 Process Table](T33_Process-for-Telegram_แจ้งปัญหา-1-Process-Table/) | `SM_Link` | Ref |
| [Process for AppSheet_KM - 1 Process Table](T72_Process-for-AppSheet_KM-1-Process-Table/) | `SM_Link_SCG` | Ref |
| [New step Output 2](T74_New-step-Output-2/) | `SM_Link_SCG` | Ref |
| [Process for New bot - 1 Process Table](T75_Process-for-New-bot-1-Process-Table/) | `SM_Link` | Ref |
| [New step Output 3](T76_New-step-Output-3/) | `SM_Link` | Ref |
| [Process for Update ScanStatus เมื่อสแกน Invoice - 1 Process Table](T77_Process-for-Update-ScanStatus-เมื่อสแกน-Invoice-1-Proce/) | `Invoice_No` | Ref |
| [Update Output](T78_Update-Output/) | `Invoice_No` | Ref |

## ไฟล์ในโฟลเดอร์นี้

| ไฟล์ | เนื้อหา | จำนวน |
|---|---|---:|
| [COLUMNS.md](COLUMNS.md) | คอลัมน์ทุกคอลัมน์ + สูตร | 40 |
| [VIEWS.md](VIEWS.md) | Views | 10 |
| [ACTIONS.md](ACTIONS.md) | Actions | 10 |
| [SLICES.md](SLICES.md) | Slices | 5 |
| [FORMAT_RULES.md](FORMAT_RULES.md) | Format Rules | 3 |

