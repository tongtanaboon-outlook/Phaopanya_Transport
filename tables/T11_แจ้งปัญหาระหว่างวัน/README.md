# 📋 ตารางข้อมูลหลัก: แจ้งปัญหาระหว่างวัน

> รหัสโฟลเดอร์: `T11_แจ้งปัญหาระหว่างวัน` · ลำดับในเอกสารต้นฉบับ: 11/90

| สรุป | จำนวน |
|---|---:|
| คอลัมน์ทั้งหมด | 29 |
| คอลัมน์ Key | 1 |
| คอลัมน์ Virtual (มีสูตรคำนวณ) | 0 |
| คอลัมน์ระบบ | 1 |
| Views | 4 |
| Actions | 14 |
| Slices | 0 |
| Format Rules | 0 |

## คุณสมบัติของตาราง

| มองเห็น (Visible) | ALWAYS |
| Shared | Yes |
| Locale ของข้อมูล | en-GB |
| Schema | แจ้งปัญหาระหว่างวัน_Schema |
| สิทธิ์การแก้ไขข้อมูล (Update mode) | ALL_CHANGES |
| Security Filter | ```=OR(USERROLE() = "ADMIN", [Email พนักงาน] = USEREMAIL())``` |
| Source Path | เผ่าปัญญา ทรานสปอร์ต |
| Worksheet (แท็บใน Google Sheets) | แจ้งปัญหาระหว่างวัน |
| โฟลเดอร์เก็บรูป/ไฟล์ | _Default |
| ลำดับคอลัมน์ | _RowNumber |
| Partition หลายไฟล์? | No |
| Partition หลายแท็บ? | No |

## 🔗 ความสัมพันธ์ออก (Ref ไปตารางอื่น)

| คอลัมน์ | อ้างถึงตาราง | ชนิด |
|---|---|---|
| `SM_Link` | [ตารางงานประจำวัน](T05_ตารางงานประจำวัน/) | Ref |
| `RT_Link` | [ข้อมูลงานRT](T13_ข้อมูลงานRT/) | Ref |
| `ID_พนักงาน` | [ข้อมูลพนักงาน](T15_ข้อมูลพนักงาน/) | Ref |

## ไฟล์ในโฟลเดอร์นี้

| ไฟล์ | เนื้อหา | จำนวน |
|---|---|---:|
| [COLUMNS.md](COLUMNS.md) | คอลัมน์ทุกคอลัมน์ + สูตร | 29 |
| [VIEWS.md](VIEWS.md) | Views | 4 |
| [ACTIONS.md](ACTIONS.md) | Actions | 14 |
| [SLICES.md](SLICES.md) | Slices | 0 |
| [FORMAT_RULES.md](FORMAT_RULES.md) | Format Rules | 0 |

