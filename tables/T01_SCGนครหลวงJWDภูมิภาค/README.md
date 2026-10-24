# 📋 ตารางข้อมูลหลัก: SCGนครหลวงJWDภูมิภาค

> รหัสโฟลเดอร์: `T01_SCGนครหลวงJWDภูมิภาค` · ลำดับในเอกสารต้นฉบับ: 1/90

| สรุป | จำนวน |
|---|---:|
| คอลัมน์ทั้งหมด | 49 |
| คอลัมน์ Key | 1 |
| คอลัมน์ Virtual (มีสูตรคำนวณ) | 0 |
| คอลัมน์ระบบ | 3 |
| Views | 4 |
| Actions | 13 |
| Slices | 0 |
| Format Rules | 2 |

## คุณสมบัติของตาราง

| มองเห็น (Visible) | ALWAYS |
| Shared | Yes |
| Locale ของข้อมูล | en-GB |
| Schema | SCGนครหลวงJWDภูมิภาค_Schema |
| สิทธิ์การแก้ไขข้อมูล (Update mode) | ALL_CHANGES |
| Security Filter | ```=OR(USERROLE() = "ADMIN", [Email พนักงาน] = USEREMAIL())``` |
| Source Path | เผ่าปัญญา ทรานสปอร์ต |
| Worksheet (แท็บใน Google Sheets) | SCGนครหลวงJWDภูมิภาค |
| โฟลเดอร์เก็บรูป/ไฟล์ | _Default |
| ลำดับคอลัมน์ | _RowNumber |
| Partition หลายไฟล์? | No |
| Partition หลายแท็บ? | No |

## 🔗 ความสัมพันธ์ออก (Ref ไปตารางอื่น)

| คอลัมน์ | อ้างถึงตาราง | ชนิด |
|---|---|---|
| `ID_Doc_Return` | [Doc_Return](T18_Doc_Return/) | Ref |
| `SM_Link_SCG` | [ตารางงานประจำวัน](T05_ตารางงานประจำวัน/) | Ref |
| `ID_พนักงาน` | [ข้อมูลพนักงาน](T15_ข้อมูลพนักงาน/) | Ref |

## 🔗 ความสัมพันธ์เข้า (ตารางอื่นอ้างถึง)

| ตาราง | คอลัมน์ | ชนิด |
|---|---|---|
| [สรุปเบิกส่วนต่าง](T17_สรุปเบิกส่วนต่าง/) | `_ComputedKey_ID_SCGนครหลวงJWDภูมิภาค` | Ref |
| [ทำเบิกส่วนต่างScgวังน้อย](T20_ทำเบิกส่วนต่างScgวังน้อย/) | `ID_SCGนครหลวงJWDภูมิภาค` | Ref |
| [Process for สรุปส่วนต่าง - 1 Process Table](T42_Process-for-สรุปส่วนต่าง-1-Process-Table/) | `_ComputedKey_ID_SCGนครหลวงJWDภูมิภาค` | Ref |
| [Process for ฺBot_4ตัว_จัดเรียงเส้นทาง Process Table](T57_Process-for-ฺBot_4ตัว_จัดเรียงเส้นทาง-Process-Table/) | `ID_SCGนครหลวงJWDภูมิภาค` | Ref |
| [Process for ทำเบิกส่วนต่างScgวังน้อย - 1 Process Table](T68_Process-for-ทำเบิกส่วนต่างScgวังน้อย-1-Process-Table/) | `ID_SCGนครหลวงJWDภูมิภาค` | Ref |
| [New step2 Output](T70_New-step2-Output/) | `ID_SCGนครหลวงJWDภูมิภาค` | Ref |
| [ไม่ผ่านNew step Output](T71_ไม่ผ่านNew-step-Output/) | `ID_SCGนครหลวงJWDภูมิภาค` | Ref |
| [Process for Bot_เบิกค่าขนส่งตามระยะทาง - 1 Process Table](T87_Process-for-Bot_เบิกค่าขนส่งตามระยะทาง-1-Process-Table/) | `ID_SCGนครหลวงJWDภูมิภาค` | Ref |
| [New step4 Output](T89_New-step4-Output/) | `ID_SCGนครหลวงJWDภูมิภาค` | Ref |
| [New step3 Output](T90_New-step3-Output/) | `ID_SCGนครหลวงJWDภูมิภาค` | Ref |

## ไฟล์ในโฟลเดอร์นี้

| ไฟล์ | เนื้อหา | จำนวน |
|---|---|---:|
| [COLUMNS.md](COLUMNS.md) | คอลัมน์ทุกคอลัมน์ + สูตร | 49 |
| [VIEWS.md](VIEWS.md) | Views | 4 |
| [ACTIONS.md](ACTIONS.md) | Actions | 13 |
| [SLICES.md](SLICES.md) | Slices | 0 |
| [FORMAT_RULES.md](FORMAT_RULES.md) | Format Rules | 2 |

