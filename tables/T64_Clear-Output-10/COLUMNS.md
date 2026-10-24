# คอลัมน์ของตาราง Clear Output 10

รวม **11 คอลัมน์** (จาก Schema `Clear Output 10_Schema`)

| # | ชื่อคอลัมน์ | ชนิด | สถานะ | สูตร/เงื่อนไข |
|---:|---|---|---|---|
| 1 | Instance Id | Text | 🔑 |  |
| 2 | ID_ปริ๊นใบวางบิล | Text |  |  |
| 3 | ชื่องาน | Text |  | Valid_If |
| 4 | StartDate | Date |  |  |
| 5 | EndDate | Date |  |  |
| 6 | ราคารวม | Price |  |  |
| 7 | Export to xlsx | Yes/No |  |  |
| 8 | Export to xlsx To Athens | Yes/No |  |  |
| 9 | ปริ๊นใบวางบิลแยกตามชื่องาน | Yes/No |  |  |
| 10 | วันที่ออกเอกสาร | Date |  |  |
| 11 | ผลลัพท์ | List |  |  |

> สถานะ: 🔑=Key · 🏷️=Label · 𝑓=Virtual · 🔒=Read-Only · 🙈=Hidden · ⚙️=คอลัมน์ระบบ

## คอลัมน์ที่มีสูตร / เงื่อนไข / บทบาทพิเศษ

### 1. Instance Id

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Text |
| Key | Yes |
| Label | No |
| Virtual | No |
| Read-Only | No |
| Hidden | No |
| รีเซ็ตเมื่อแก้ไข | No |
| คอลัมน์ระบบ | No |
| ส่วนหนึ่งของ Key | No |
| นิยามคงที่ | No |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 3. ชื่องาน

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Text |
| Key | No |
| Label | No |
| Virtual | No |
| Read-Only | No |
| Hidden | No |
| รีเซ็ตเมื่อแก้ไข | No |
| คอลัมน์ระบบ | No |
| ส่วนหนึ่งของ Key | No |
| นิยามคงที่ | Yes |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

**Valid_If (เงื่อนไขความถูกต้อง):**

```
=ข้อมูลชื่องานต้นทาง ปลายทาง[ชื่องาน]
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": "=ข้อมูลชื่องานต้นทาง ปลายทาง[ชื่องาน]", "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

## คอลัมน์ทั่วไป (ไม่มีสูตรหรือเงื่อนไขพิเศษ)

- **2. ID_ปริ๊นใบวางบิล** — ชนิด `Text` (ค่าปกติ)
- **4. StartDate** — ชนิด `Date` (ค่าปกติ)
- **5. EndDate** — ชนิด `Date` (ค่าปกติ)
- **6. ราคารวม** — ชนิด `Price` (ค่าปกติ)
- **7. Export to xlsx** — ชนิด `Yes/No` (ค่าปกติ)
- **8. Export to xlsx To Athens** — ชนิด `Yes/No` (ค่าปกติ)
- **9. ปริ๊นใบวางบิลแยกตามชื่องาน** — ชนิด `Yes/No` (ค่าปกติ)
- **10. วันที่ออกเอกสาร** — ชนิด `Date` (ค่าปกติ)
- **11. ผลลัพท์** — ชนิด `List` (ค่าปกติ)

