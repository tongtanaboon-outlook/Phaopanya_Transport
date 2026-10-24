# คอลัมน์ของตาราง สรุปเบิกส่วนต่าง

รวม **12 คอลัมน์** (จาก Schema `สรุปเบิกส่วนต่าง_Schema`)

| # | ชื่อคอลัมน์ | ชนิด | สถานะ | สูตร/เงื่อนไข |
|---:|---|---|---|---|
| 1 | _RowNumber | Number | 🔒 🙈 ⚙️ |  |
| 2 | ID_สรุปเบิกส่วนต่าง | Text | 🔑 🏷️ | InitValue |
| 3 | ID_Optimization | Text |  |  |
| 4 | ID_เบิกส่วนต่างSCGวังน้อย | Text |  |  |
| 5 | _ComputedKey_ID_SCGนครหลวงJWDภูมิภาค | Ref |  |  |
| 6 | วันที่เริ่มต้น | Date |  |  |
| 7 | วันที่สิ้นสุด | Date |  |  |
| 8 | รวมค่าขนส่งส่วนเพิ่ม | Decimal |  |  |
| 9 | วันที่ออกเอกสาร | Date |  |  |
| 10 | Export to Excel | Yes/No |  |  |
| 11 | สรุป_ทำเบิกส่วนต่างScgวังน้อย | List | 🔒 | AppFormula |
| 12 | ราคารวม_ทำเบิกส่วนต่างScgวังน้อย | Price | 🔒 | AppFormula |

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

### 2. ID_สรุปเบิกส่วนต่าง

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

### 11. สรุป_ทำเบิกส่วนต่างScgวังน้อย

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | List |
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
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**App Formula (สูตรคำนวณ):**

```
=FILTER( ทำเบิกส่วนต่างSCGวังน้อย, AND(ISNOTBLANK([วันที่ส่งสินค้า]), [วันที่ส่งสินค้า] >= [_THISROW].[วันที่เริ่มต้น], [วันที่ส่งสินค้า]<= [_THISROW].[วันที่สิ้นสุด], [สถานะ] = "ผ่านการตรวจสอบ" ) )
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"ElementType": "Ref", "ElementTypeQualifier": " {\"ReferencedTableName\":\"ทำเบิกส่วน ต่างScgวังน้อย\",\"ReferencedRootTableName\":\"ทำเบิกส่วน ต่างScgวังน้อย\",\"ReferencedType\":\"Text\",\"ReferencedTypeQualifier\":\" {\\\"MaxLength\\\":null,\\\"MinLength\\\":null,\\\"LongTextFor matting\\\":\\\"Plain Text\\\",\\\"IsMulticolumnKey\\\":false,\\\"Valid_If\\\":null,\\\"Error_Message_If_Invalid\\\":null,\\\"Show_If\\\":null,\\\"Required_If\\\":null,\\\"Editable_If\\\":null,\\\"Reset_If\\\":null,\\\"Suggested_Values\\\":null}\",\"ReferencedKeyColumn\":\"ID_ทำเบิกส่วนต่างScgวังน้อย\",\"IsAPartOf\":false,\"RelationshipName\":null,\"InputMode\":\"Auto\",\"Valid_If\":null,\"Error_Message_If_Invalid\":null,\"Show_If\":null,\"Required_If\":null,\"Editable_If\":null,\"Reset_If\":null,\"Suggested_Values\":null}", "ItemSeparator": " , ", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 12. ราคารวม_ทำเบิกส่วนต่างScgวังน้อย

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Price |
| Key | No |
| Label | No |
| Virtual | Yes |
| Read-Only | Yes |
| Hidden | No |
| รีเซ็ตเมื่อแก้ไข | No |
| คอลัมน์ระบบ | No |
| ส่วนหนึ่งของ Key | No |
| นิยามคงที่ | No |
| ค้นหาได้ | No |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No Schema Name Doc_Return_Schema |
| Locale | en-GB |

**App Formula (สูตรคำนวณ):**

```
=SUM(SELECT( ทำเบิกส่วนต่างScgวังน้อย[ขออนุมัติเบิกค่าขนส่งส่วนเพิ่ม], AND(ISNOTBLANK([วันที่ส่งสินค้า]), [วันที่ส่งสินค้า] >= [_THISROW].[วันที่เริ่มต้น], [วันที่ส่งสินค้า] <= [_THISROW].[วันที่สิ้นสุด], [สถานะ] = "ผ่านการตรวจสอบ" ) ))
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"CurrencySymbol": "฿", "MaxValue": null, "MinValue": null, "StepValue": null, "DecimalDigits": 2, "NumericDigits": null, "ShowThousandsSeparator": true, "NumberDisplayMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

## คอลัมน์ทั่วไป (ไม่มีสูตรหรือเงื่อนไขพิเศษ)

- **3. ID_Optimization** — ชนิด `Text` (ค่าปกติ)
- **4. ID_เบิกส่วนต่างSCGวังน้อย** — ชนิด `Text` (ค่าปกติ)
- **5. _ComputedKey_ID_SCGนครหลวงJWDภูมิภาค** — ชนิด `Ref` (ค่าปกติ)
- **6. วันที่เริ่มต้น** — ชนิด `Date` (ค่าปกติ)
- **7. วันที่สิ้นสุด** — ชนิด `Date` (ค่าปกติ)
- **8. รวมค่าขนส่งส่วนเพิ่ม** — ชนิด `Decimal` (ค่าปกติ)
- **9. วันที่ออกเอกสาร** — ชนิด `Date` (ค่าปกติ)
- **10. Export to Excel** — ชนิด `Yes/No` (ค่าปกติ)

