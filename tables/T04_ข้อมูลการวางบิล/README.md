# 📋 ตารางข้อมูลหลัก: ข้อมูลการวางบิล

> รหัสโฟลเดอร์: `T04_ข้อมูลการวางบิล` · ลำดับในเอกสารต้นฉบับ: 4/90

| สรุป | จำนวน |
|---|---:|
| คอลัมน์ทั้งหมด | 45 |
| คอลัมน์ Key | 1 |
| คอลัมน์ Virtual (มีสูตรคำนวณ) | 0 |
| คอลัมน์ระบบ | 1 |
| Views | 12 |
| Actions | 10 |
| Slices | 3 |
| Format Rules | 4 |

## คุณสมบัติของตาราง

| มองเห็น (Visible) | ALWAYS |
| Shared | Yes |
| Locale ของข้อมูล | en-GB |
| Schema | ข้อมูลการวางบิล_Schema |
| สิทธิ์การแก้ไขข้อมูล (Update mode) | ALL_CHANGES |
| Security Filter | ```=OR(USERROLE() = "ADMIN", [Email พนักงาน] = USEREMAIL())``` |
| Source Path | เผ่าปัญญา ทรานสปอร์ต |
| Worksheet (แท็บใน Google Sheets) | ข้อมูลการวางบิล |
| โฟลเดอร์เก็บรูป/ไฟล์ | _Default |
| ลำดับคอลัมน์ | _RowNumber |
| Partition หลายไฟล์? | No |
| Partition หลายแท็บ? | No |

## 🔗 ความสัมพันธ์ออก (Ref ไปตารางอื่น)

| คอลัมน์ | อ้างถึงตาราง | ชนิด |
|---|---|---|
| `ID_พนักงาน` | [ข้อมูลพนักงาน](T15_ข้อมูลพนักงาน/) | Ref |

## ไฟล์ในโฟลเดอร์นี้

| ไฟล์ | เนื้อหา | จำนวน |
|---|---|---:|
| [COLUMNS.md](COLUMNS.md) | คอลัมน์ทุกคอลัมน์ + สูตร | 45 |
| [VIEWS.md](VIEWS.md) | Views | 12 |
| [ACTIONS.md](ACTIONS.md) | Actions | 10 |
| [SLICES.md](SLICES.md) | Slices | 3 |
| [FORMAT_RULES.md](FORMAT_RULES.md) | Format Rules | 4 |

