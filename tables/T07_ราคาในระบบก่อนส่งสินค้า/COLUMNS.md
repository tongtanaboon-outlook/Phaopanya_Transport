# คอลัมน์ของตาราง ราคาในระบบก่อนส่งสินค้า

รวม **15 คอลัมน์** (จาก Schema `ราคาในระบบก่อนส่งสินค้า_Schema`)

| # | ชื่อคอลัมน์ | ชนิด | สถานะ | สูตร/เงื่อนไข |
|---:|---|---|---|---|
| 1 | _RowNumber | Number | 🔒 🙈 ⚙️ |  |
| 2 | ID_ราคา | Number | 🔒 🙈 |  |
| 3 | Shipment No | Number | 🔑 🏷️ |  |
| 4 | วันที่ส่งสินค้า | Date |  |  |
| 5 | ชื่อต้นทาง | Text |  |  |
| 6 | ชื่อปลายทาง | Text |  |  |
| 7 | ชื่อ - นามสกุล | Text |  |  |
| 8 | ทะเบียนรถ | Text |  |  |
| 9 | Truck Type | Text |  |  |
| 10 | Weight (t) | Decimal |  |  |
| 11 | น้ำหนัก | Decimal |  |  |
| 12 | ระยะทาง (km) | Decimal |  |  |
| 13 | ราคา | Price |  |  |
| 14 | ราคาหลังส่งสินค้า | Price | 🔒 |  |
| 15 | เดือน | Text | 🔒 | AppFormula |

> สถานะ: 🔑=Key · 🏷️=Label · 𝑓=Virtual · 🔒=Read-Only · 🙈=Hidden · ⚙️=คอลัมน์ระบบ

## คอลัมน์ที่มีสูตร / เงื่อนไข / บทบาทพิเศษ

### 1. _RowNumber

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Number |
| Key | No |
| Label | No |
| Virtual | No |
| Read-Only | Yes |
| Hidden | Yes |
| รีเซ็ตเมื่อแก้ไข | No |
| คอลัมน์ระบบ | Yes |
| ส่วนหนึ่งของ Key | No |
| นิยามคงที่ | Yes |
| ค้นหาได้ | No |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxValue": null, "MinValue": null, "StepValue": null, "NumericDigits": null, "ShowThousandsSeparator": true, "NumberDisplayMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 3. Shipment No

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Number |
| Key | Yes |
| Label | Yes |
| Virtual | No |
| Read-Only | No |
| Hidden | No |
| รีเซ็ตเมื่อแก้ไข | No |
| คอลัมน์ระบบ | No |
| ส่วนหนึ่งของ Key | Yes |
| นิยามคงที่ | No |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxValue": null, "MinValue": null, "StepValue": null, "NumericDigits": null, "ShowThousandsSeparator": false, "NumberDisplayMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 15. เดือน

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Text |
| Key | No |
| Label | No |
| Virtual | Yes |
| Read-Only | Yes |
| Hidden | No |
| รีเซ็ตเมื่อแก้ไข | No |
| คอลัมน์ระบบ | No |
| ส่วนหนึ่งของ Key | No |
| นิยามคงที่ | No |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No Schema Name หน้าหลัก_Schema |
| Locale | en-GB |

**App Formula (สูตรคำนวณ):**

```
=IF( ISBLANK([วันที่ส่งสินค้า]), "", CONCATENATE( YEAR([วันที่ส่งสินค้า]) - IF(YEAR([วันที่ส่งสินค้า]) > 2500, 543, 0), "-", TEXT([วันที่ส่งสินค้า], "MM") ) )
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

## คอลัมน์ทั่วไป (ไม่มีสูตรหรือเงื่อนไขพิเศษ)

- **2. ID_ราคา** — ชนิด `Number` (Label=No Spreadsheet formula IF(RC[1]<>"","ในระบบ-" & ROW(), "") Read-Only=Yes Hidden=Yes)
- **4. วันที่ส่งสินค้า** — ชนิด `Date` (ค่าปกติ)
- **5. ชื่อต้นทาง** — ชนิด `Text` (ค่าปกติ)
- **6. ชื่อปลายทาง** — ชนิด `Text` (ค่าปกติ)
- **7. ชื่อ - นามสกุล** — ชนิด `Text` (ค่าปกติ)
- **8. ทะเบียนรถ** — ชนิด `Text` (ค่าปกติ)
- **9. Truck Type** — ชนิด `Text` (ค่าปกติ)
- **10. Weight (t)** — ชนิด `Decimal` (ค่าปกติ)
- **11. น้ำหนัก** — ชนิด `Decimal` (ค่าปกติ)
- **12. ระยะทาง (km)** — ชนิด `Decimal` (ค่าปกติ)
- **13. ราคา** — ชนิด `Price` (ค่าปกติ)
- **14. ราคาหลังส่งสินค้า** — ชนิด `Price` (Label=No Spreadsheet formula =ArrayFormula(XLOOKUP(RC[-11],'ราคาในระบบหลังส่ง สินค้า'!C[-12]:C[-12],'ราคาในระบบหลังส่งสินค้า'!C[-9]:C[-9])) Read-Only=Yes)

