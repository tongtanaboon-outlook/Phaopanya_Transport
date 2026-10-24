# คอลัมน์ของตาราง ข้อมูลงานRW

รวม **15 คอลัมน์** (จาก Schema `ข้อมูลงานRW_Schema`)

| # | ชื่อคอลัมน์ | ชนิด | สถานะ | สูตร/เงื่อนไข |
|---:|---|---|---|---|
| 1 | _RowNumber | Number | 🔒 🙈 ⚙️ |  |
| 2 | ID_ข้อมูลงานRW | Text | 🔑 🏷️ | InitValue |
| 3 | วันที่จัดงาน | Date |  |  |
| 4 | Due Date | Date |  |  |
| 5 | ผรม. | Text |  |  |
| 6 | พขร. | Text |  |  |
| 7 | ทะเบียน | Text |  |  |
| 8 | Shipment | Number |  |  |
| 9 | สินค้า | Text |  |  |
| 10 | Model สินค้า | Text |  |  |
| 11 | เลขที่เอกสาร | Text |  |  |
| 12 | ชื่อร้าน | Text |  |  |
| 13 | จังหวัด | Text |  |  |
| 14 | ภาค | Text |  |  |
| 15 | ปัญหา | Text |  |  |

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

### 2. ID_ข้อมูลงานRW

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Text |
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

**ค่าเริ่มต้น (Initial Value):**

```
UNIQUEID()
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

## คอลัมน์ทั่วไป (ไม่มีสูตรหรือเงื่อนไขพิเศษ)

- **3. วันที่จัดงาน** — ชนิด `Date` (ค่าปกติ)
- **4. Due Date** — ชนิด `Date` (ค่าปกติ)
- **5. ผรม.** — ชนิด `Text` (ค่าปกติ)
- **6. พขร.** — ชนิด `Text` (ค่าปกติ)
- **7. ทะเบียน** — ชนิด `Text` (ค่าปกติ)
- **8. Shipment** — ชนิด `Number` (ค่าปกติ)
- **9. สินค้า** — ชนิด `Text` (ค่าปกติ)
- **10. Model สินค้า** — ชนิด `Text` (ค่าปกติ)
- **11. เลขที่เอกสาร** — ชนิด `Text` (ค่าปกติ)
- **12. ชื่อร้าน** — ชนิด `Text` (ค่าปกติ)
- **13. จังหวัด** — ชนิด `Text` (ค่าปกติ)
- **14. ภาค** — ชนิด `Text` (ค่าปกติ)
- **15. ปัญหา** — ชนิด `Text` (ค่าปกติ)

