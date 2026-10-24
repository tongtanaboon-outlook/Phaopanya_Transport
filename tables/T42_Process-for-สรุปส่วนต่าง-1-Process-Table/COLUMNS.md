# คอลัมน์ของตาราง Process for สรุปส่วนต่าง - 1 Process Table

รวม **12 คอลัมน์** (จาก Schema `Process for สรุปส่วนต่าง - 1 Process Table_Schema`)

| # | ชื่อคอลัมน์ | ชนิด | สถานะ | สูตร/เงื่อนไข |
|---:|---|---|---|---|
| 1 | Instance Id | Text | 🔑 |  |
| 2 | ID_สรุปเบิกส่วนต่าง | Text |  |  |
| 3 | ID_Optimization | Text |  |  |
| 4 | ID_เบิกส่วนต่างSCGวังน้อย | Text |  |  |
| 5 | _ComputedKey_ID_SCGนครหลวงJWDภูมิภาค | Ref |  |  |
| 6 | วันที่เริ่มต้น | Date |  |  |
| 7 | วันที่สิ้นสุด | Date |  |  |
| 8 | รวมค่าขนส่งส่วนเพิ่ม | Decimal |  |  |
| 9 | วันที่ออกเอกสาร | Date |  |  |
| 10 | Export to Excel | Yes/No |  |  |
| 11 | สรุป_ทำเบิกส่วนต่างScgวังน้อย | List |  |  |
| 12 | ราคารวม_ทำเบิกส่วนต่างScgวังน้อย | Price |  |  |

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
| นิยามคงที่ | Yes |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

## คอลัมน์ทั่วไป (ไม่มีสูตรหรือเงื่อนไขพิเศษ)

- **2. ID_สรุปเบิกส่วนต่าง** — ชนิด `Text` (ค่าปกติ)
- **3. ID_Optimization** — ชนิด `Text` (ค่าปกติ)
- **4. ID_เบิกส่วนต่างSCGวังน้อย** — ชนิด `Text` (ค่าปกติ)
- **5. _ComputedKey_ID_SCGนครหลวงJWDภูมิภาค** — ชนิด `Ref` (ค่าปกติ)
- **6. วันที่เริ่มต้น** — ชนิด `Date` (ค่าปกติ)
- **7. วันที่สิ้นสุด** — ชนิด `Date` (ค่าปกติ)
- **8. รวมค่าขนส่งส่วนเพิ่ม** — ชนิด `Decimal` (ค่าปกติ)
- **9. วันที่ออกเอกสาร** — ชนิด `Date` (ค่าปกติ)
- **10. Export to Excel** — ชนิด `Yes/No` (ค่าปกติ)
- **11. สรุป_ทำเบิกส่วนต่างScgวังน้อย** — ชนิด `List` (ค่าปกติ)
- **12. ราคารวม_ทำเบิกส่วนต่างScgวังน้อย** — ชนิด `Price` (ค่าปกติ)

