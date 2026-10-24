# 🤖 Process Table (สถานะของ Bot): Process for Update ScanStatus เมื่อสแกน Invoice - 1 Process Table

> รหัสโฟลเดอร์: `T77_Process-for-Update-ScanStatus-เมื่อสแกน-Invoice-1-Proce` · ลำดับในเอกสารต้นฉบับ: 77/90

| สรุป | จำนวน |
|---|---:|
| คอลัมน์ทั้งหมด | 19 |
| คอลัมน์ Key | 1 |
| คอลัมน์ Virtual (มีสูตรคำนวณ) | 0 |
| คอลัมน์ระบบ | 0 |
| Views | 0 |
| Actions | 0 |
| Slices | 0 |
| Format Rules | 0 |

## คุณสมบัติของตาราง

| มองเห็น (Visible) | NEVER |
| Shared | Yes |
| Schema | Process for Update ScanStatus เมื่อสแกน Invoice - 1 Process Table_Schema |
| สิทธิ์การแก้ไขข้อมูล (Update mode) | READ_ONLY |
| Source Path | /ProcessStateTables/70999aca-5a1f-4dfc-907b-417bc046f574/d77c3cd8-7325-4d1b-8dd0-0a391dcc374c/State Table |
| แหล่งข้อมูล | native |
| โฟลเดอร์เก็บรูป/ไฟล์ | _Default |
| ลำดับคอลัมน์ | _RowNumber |
| Partition หลายไฟล์? | No |
| Partition หลายแท็บ? | No |

## 🔗 ความสัมพันธ์ออก (Ref ไปตารางอื่น)

| คอลัมน์ | อ้างถึงตาราง | ชนิด |
|---|---|---|
| `Invoice_No` | [ตารางงานประจำวัน](T05_ตารางงานประจำวัน/) | Ref |
| `Update` | [Update Output](T78_Update-Output/) | Ref |

## ไฟล์ในโฟลเดอร์นี้

| ไฟล์ | เนื้อหา | จำนวน |
|---|---|---:|
| [COLUMNS.md](COLUMNS.md) | คอลัมน์ทุกคอลัมน์ + สูตร | 19 |
| [VIEWS.md](VIEWS.md) | Views | 0 |
| [ACTIONS.md](ACTIONS.md) | Actions | 0 |
| [SLICES.md](SLICES.md) | Slices | 0 |
| [FORMAT_RULES.md](FORMAT_RULES.md) | Format Rules | 0 |

