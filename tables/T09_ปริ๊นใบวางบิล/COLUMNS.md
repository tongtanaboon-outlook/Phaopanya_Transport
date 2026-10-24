# คอลัมน์ของตาราง ปริ๊นใบวางบิล

รวม **11 คอลัมน์** (จาก Schema `ปริ๊นใบวางบิล_Schema`)

| # | ชื่อคอลัมน์ | ชนิด | สถานะ | สูตร/เงื่อนไข |
|---:|---|---|---|---|
| 1 | _RowNumber | Number | 🔒 🙈 ⚙️ |  |
| 2 | ID_ปริ๊นใบวางบิล | Text | 🔑 | InitValue |
| 3 | ชื่องาน | Text | 🏷️ | Valid_If |
| 4 | StartDate | Date |  |  |
| 5 | EndDate | Date |  |  |
| 6 | ราคารวม | Price |  | AppFormula |
| 7 | Export to xlsx | Yes/No |  |  |
| 8 | Export to xlsx To Athens | Yes/No |  |  |
| 9 | ปริ๊นใบวางบิลแยกตามชื่องาน | Yes/No |  |  |
| 10 | วันที่ออกเอกสาร | Date |  | InitValue |
| 11 | ผลลัพท์ | List | 🔒 | AppFormula |

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

### 2. ID_ปริ๊นใบวางบิล

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

### 3. ชื่องาน

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Text |
| Key | No |
| Label | Yes |
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
| Locale | en-GB |

**Valid_If (เงื่อนไขความถูกต้อง):**

```
=ข้อมูลชื่องานต้นทาง ปลายทาง[ชื่องาน]
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": "=ข้อมูลชื่องานต้นทาง ปลายทาง[ชื่องาน]", "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 6. ราคารวม

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Price |
| Key | No |
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
| Locale | en-GB |

**App Formula (สูตรคำนวณ):**

```
=SUM(SELECT(ข้อมูลการวางบิล[ราคา], AND([ชื่องาน]= [_THISROW].[ชื่องาน],[วันที่] >= [_THISROW].[Startdate], [วันที่] <= [_THISROW].[Enddate])))
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"CurrencySymbol": "฿", "MaxValue": null, "MinValue": null, "StepValue": null, "DecimalDigits": 2, "NumericDigits": null, "ShowThousandsSeparator": true, "NumberDisplayMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 10. วันที่ออกเอกสาร

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Date |
| Key | No |
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
| Locale | en-GB |

**ค่าเริ่มต้น (Initial Value):**

```
=TODAY()
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"UseLongDateFormat": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 11. ผลลัพท์

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
| ข้อมูลอ่อนไหว | No Schema Name PDFพนักงาน_Schema |
| Locale | en-GB |

**App Formula (สูตรคำนวณ):**

```
=FILTER("ข้อมูลการวางบิล",(AND([ชื่องาน]=[_THISROW].[ชื่องาน], [วันที่]>=[_THISROW].[StartDate],[วันที่]<=[_THISROW]. [EndDate])))
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"ElementType": "Ref", "ElementTypeQualifier": " {\"ReferencedTableName\":\"ข้อมูลการวาง บิล\",\"ReferencedRootTableName\":\"ข้อมูลการวาง บิล\",\"ReferencedType\":\"Text\",\"ReferencedTypeQualifier\":\"{\\\"MaxLength\\\":null,\\\"MinLength\\\":null,\\\"LongTextFor matting\\\":\\\"Plain Text\\\",\\\"IsMulticolumnKey\\\":false,\\\"Valid_If\\\":null,\\\"Error_Message_If_Invalid\\\":null,\\\"Show_If\\\":null,\\\"Required_If\\\":null,\\\"Editable_If\\\":null,\\\"Reset_If\\\":null,\\\"Suggested_Values\\\":null}\",\"ReferencedKeyColumn\":\"ID_วาง บิล\",\"IsAPartOf\":false,\"RelationshipName\":null,\"InputMode\":\"Auto\",\"Valid_If\":null,\"Error_Message_If_Invalid\":null,\"Show_If\":null,\"Required_If\":null,\"Editable_If\":null,\"Reset_If\":null,\"Suggested_Values\":null}", "ItemSeparator": " , ", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

## คอลัมน์ทั่วไป (ไม่มีสูตรหรือเงื่อนไขพิเศษ)

- **4. StartDate** — ชนิด `Date` (ค่าปกติ)
- **5. EndDate** — ชนิด `Date` (ค่าปกติ)
- **7. Export to xlsx** — ชนิด `Yes/No` (ค่าปกติ)
- **8. Export to xlsx To Athens** — ชนิด `Yes/No` (ค่าปกติ)
- **9. ปริ๊นใบวางบิลแยกตามชื่องาน** — ชนิด `Yes/No` (ค่าปกติ)

