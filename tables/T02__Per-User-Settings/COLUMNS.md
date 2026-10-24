# คอลัมน์ของตาราง _Per User Settings

รวม **15 คอลัมน์** (จาก Schema `_Per User Settings_Schema`)

| # | ชื่อคอลัมน์ | ชนิด | สถานะ | สูตร/เงื่อนไข |
|---:|---|---|---|---|
| 1 | _RowNumber | Number | 🔒 🙈 ⚙️ |  |
| 2 | _EMAIL | Email | 🙈 | AppFormula |
| 3 | _NAME | Name | 🙈 | AppFormula |
| 4 | _LOCATION | LatLong | 🙈 |  |
| 5 | Options Heading | Show | 🔒 🙈 |  |
| 6 | Option 1 | Text | 🙈 |  |
| 7 | Option 2 | Text | 🙈 |  |
| 8 | Option 3 | Text | 🙈 |  |
| 9 | Option 4 | Text | 🙈 |  |
| 10 | Option 5 | Text | 🙈 |  |
| 11 | Option 6 | Number | 🙈 |  |
| 12 | Option 7 | Text | 🙈 |  |
| 13 | Option 8 | Text | 🙈 |  |
| 14 | Option 9 | Text | 🙈 |  |
| 15 | _THISUSER | Text | 🔑 🙈 | InitValue |

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
| Locale | th-TH |

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxValue": null, "MinValue": null, "StepValue": null, "NumericDigits": null, "ShowThousandsSeparator": true, "NumberDisplayMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 2. _EMAIL

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Email |
| Key | No |
| Label | No |
| Virtual | No |
| Read-Only | No |
| Hidden | Yes |
| รีเซ็ตเมื่อแก้ไข | No |
| คอลัมน์ระบบ | No |
| ส่วนหนึ่งของ Key | No |
| นิยามคงที่ | Yes |
| ค้นหาได้ | No |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | th-TH |

**App Formula (สูตรคำนวณ):**

```
USEREMAIL()
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 3. _NAME

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Name |
| Key | No |
| Label | No |
| Virtual | No |
| Read-Only | No |
| Hidden | Yes |
| รีเซ็ตเมื่อแก้ไข | No |
| คอลัมน์ระบบ | No |
| ส่วนหนึ่งของ Key | No |
| นิยามคงที่ | Yes |
| ค้นหาได้ | No |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | th-TH |

**App Formula (สูตรคำนวณ):**

```
USERNAME()
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 15. _THISUSER

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Text |
| Key | Yes |
| Label | No |
| Virtual | No |
| Read-Only | No |
| Hidden | Yes |
| รีเซ็ตเมื่อแก้ไข | No |
| คอลัมน์ระบบ | No |
| ส่วนหนึ่งของ Key | Yes |
| นิยามคงที่ | Yes |
| ค้นหาได้ | No |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No Schema Name SCGนครหลวงJWDภูมิภาค_Schema |
| Locale | th-TH |

**ค่าเริ่มต้น (Initial Value):**

```
onlyvalue
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

## คอลัมน์ทั่วไป (ไม่มีสูตรหรือเงื่อนไขพิเศษ)

- **4. _LOCATION** — ชนิด `LatLong` (Hidden=Yes)
- **5. Options Heading** — ชนิด `Show` (Read-Only=Yes Hidden=Yes)
- **6. Option 1** — ชนิด `Text` (Hidden=Yes)
- **7. Option 2** — ชนิด `Text` (Hidden=Yes)
- **8. Option 3** — ชนิด `Text` (Hidden=Yes)
- **9. Option 4** — ชนิด `Text` (Hidden=Yes)
- **10. Option 5** — ชนิด `Text` (Hidden=Yes)
- **11. Option 6** — ชนิด `Number` (Hidden=Yes)
- **12. Option 7** — ชนิด `Text` (Hidden=Yes)
- **13. Option 8** — ชนิด `Text` (Hidden=Yes)
- **14. Option 9** — ชนิด `Text` (Hidden=Yes)

