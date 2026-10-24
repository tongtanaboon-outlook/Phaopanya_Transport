# คอลัมน์ของตาราง สร้างเอกสาร

รวม **25 คอลัมน์** (จาก Schema `สร้างเอกสาร_Schema`)

| # | ชื่อคอลัมน์ | ชนิด | สถานะ | สูตร/เงื่อนไข |
|---:|---|---|---|---|
| 1 | _RowNumber | Number | 🔒 🙈 ⚙️ |  |
| 2 | ID_สร้างเอกสาร | Text | 🔑 🏷️ | InitValue |
| 3 | ชื่องาน | Text |  | Valid_If |
| 4 | ชื่อ - นามสกุล | Text |  | Valid_If |
| 5 | StartDate | Date |  |  |
| 6 | EndDate | Date |  |  |
| 7 | ราคารวม | Price |  | AppFormula |
| 8 | Export to xlsx | Yes/No |  |  |
| 9 | Export to xlsx To Athens | Yes/No |  |  |
| 10 | ปริ๊นใบวางบิลแยกตามชื่องาน | Yes/No |  |  |
| 11 | วันที่ออกเอกสาร | Date |  | InitValue |
| 12 | ราคารวมคนขับ | Price |  | AppFormula |
| 13 | Export to XLSX_12 | Yes/No |  |  |
| 14 | EXPORT TO PDFรับคืน | Yes/No |  |  |
| 15 | ปริ๊นใบวางบิล | List | 🔒 | AppFormula |
| 16 | ปริ๊นใบป่ะหน้า | List | 🔒 | AppFormula |
| 17 | ปริ๊นทำเบิกส่วนต่างScgวังน้อย | List | 🔒 | AppFormula |
| 18 | ราคารวม_ทำเบิกส่วนต่างScgวังน้อย | Price | 🔒 | AppFormula |
| 19 | สรุปจำนวนจุดส่งงาน | List | 🔒 | AppFormula |
| 20 | ได้เพิ่ม200_ไม่มีสินค้าคืน_ร้านปิด_ไม่มีในจุดส่ง | List | 🔒 | AppFormula |
| 21 | ทำเบิกค่ายกขึ้นชั้น | List | 🔒 | AppFormula |
| 22 | ได้เพิ่ม50%ของค่าเที่ยว | List | 🔒 | AppFormula |
| 23 | ราคา_ได้เพิ่ม200_ไม่มีสินค้าคืน_ร้านปิด_ไม่มีในจุดส่ง | Price | 🔒 | AppFormula |
| 24 | ราคา_ทำเบิกค่ายกขึ้นชั้น | Price | 🔒 | AppFormula |
| 25 | ราคา_ได้เพิ่ม50%ของค่าเที่ยว | Price | 🔒 | AppFormula |

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

### 2. ID_สร้างเอกสาร

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

### 4. ชื่อ - นามสกุล

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
| นิยามคงที่ | No |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**Valid_If (เงื่อนไขความถูกต้อง):**

```
=ข้อมูลพนักงาน[ชื่อ - นามสกุล]
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": "=ข้อมูลพนักงาน[ชื่อ - นามสกุล]", "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 7. ราคารวม

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
{"CurrencySymbol": "$", "MaxValue": null, "MinValue": null, "StepValue": null, "DecimalDigits": 2, "NumericDigits": null, "ShowThousandsSeparator": true, "NumberDisplayMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 11. วันที่ออกเอกสาร

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

### 12. ราคารวมคนขับ

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
=SUM(SELECT(ข้อมูลการวางบิล[ราคา], AND([ชื่อ - นามสกุล]= [_THISROW].[ชื่อ - นามสกุล],[วันที่] >= [_THISROW].[Startdate], [วันที่] <= [_THISROW].[Enddate])))
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"CurrencySymbol": "$", "MaxValue": null, "MinValue": null, "StepValue": null, "DecimalDigits": 2, "NumericDigits": null, "ShowThousandsSeparator": true, "NumberDisplayMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 15. ปริ๊นใบวางบิล

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
=FILTER("ข้อมูลการวางบิล",(AND([ชื่องาน]=[_THISROW].[ชื่องาน], [วันที่]>=[_THISROW].[StartDate],[วันที่]<=[_THISROW]. [EndDate])))
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"ElementType": "Ref", "ElementTypeQualifier": " {\"ReferencedTableName\":\"ข้อมูลการวาง บิล\",\"ReferencedRootTableName\":\"ข้อมูลการวาง บิล\",\"ReferencedType\":\"Text\",\"ReferencedTypeQualifier\":\"{\\\"MaxLength\\\":null,\\\"MinLength\\\":null,\\\"LongTextFor matting\\\":\\\"Plain Text\\\",\\\"IsMulticolumnKey\\\":false,\\\"Valid_If\\\":null,\\\"Error_Message_If_Invalid\\\":null,\\\"Show_If\\\":null,\\\"Required_If\\\":null,\\\"Editable_If\\\":null,\\\"Reset_If\\\":null,\\\"Suggested_Values\\\":null}\",\"ReferencedKeyColumn\":\"ID_วาง บิล\",\"IsAPartOf\":false,\"RelationshipName\":null,\"InputMode\":\"Auto\",\"Valid_If\":null,\"Error_Message_If_Invalid\":null,\"Show_If\":null,\"Required_If\":null,\"Editable_If\":null,\"Reset_If\":null,\"Suggested_Values\":null}", "ItemSeparator": " , ", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 16. ปริ๊นใบป่ะหน้า

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
=FILTER("ข้อมูลการวางบิล",(AND([ชื่อ - นามสกุล]=[_THISROW].[ชื่อ - นามสกุล],[วันที่]>=[_THISROW].[StartDate],[วันที่]<=[_THISROW]. [EndDate])))
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"ElementType": "Ref", "ElementTypeQualifier": " {\"ReferencedTableName\":\"ข้อมูลการวาง บิล\",\"ReferencedRootTableName\":\"ข้อมูลการวาง บิล\",\"ReferencedType\":\"Text\",\"ReferencedTypeQualifier\":\"{\\\"MaxLength\\\":null,\\\"MinLength\\\":null,\\\"LongTextFor matting\\\":\\\"Plain Text\\\",\\\"IsMulticolumnKey\\\":false,\\\"Valid_If\\\":null,\\\"Error_Message_If_Invalid\\\":null,\\\"Show_If\\\":null,\\\"Required_If\\\":null,\\\"Editable_If\\\":null,\\\"Reset_If\\\":null,\\\"Suggested_Values\\\":null}\",\"ReferencedKeyColumn\":\"ID_วาง บิล\",\"IsAPartOf\":false,\"RelationshipName\":null,\"InputMode\":\"Auto\",\"Valid_If\":null,\"Error_Message_If_Invalid\":null,\"Show_If\":null,\"Required_If\":null,\"Editable_If\":null,\"Reset_If\":null,\"Suggested_Values\":null}", "ItemSeparator": " , ", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 17. ปริ๊นทำเบิกส่วนต่างScgวังน้อย

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
=FILTER( ทำเบิกส่วนต่างSCGวังน้อย, AND(ISNOTBLANK([วันที่ส่งสินค้า]), [วันที่ส่งสินค้า] >= [_THISROW].[StartDate], [วันที่ส่งสินค้า] <= [_THISROW].[EndDate], [สถานะ] = "ผ่านการตรวจสอบ" ) )
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"ElementType": "Ref", "ElementTypeQualifier": " {\"ReferencedTableName\":\"ทำเบิกส่วน ต่างScgวังน้อย\",\"ReferencedRootTableName\":\"ทำเบิกส่วน ต่างScgวังน้อย\",\"ReferencedType\":\"Text\",\"ReferencedTypeQualifier\":\" {\\\"MaxLength\\\":null,\\\"MinLength\\\":null,\\\"LongTextFor matting\\\":\\\"Plain Text\\\",\\\"IsMulticolumnKey\\\":false,\\\"Valid_If\\\":null,\\\"Error_Message_If_Invalid\\\":null,\\\"Show_If\\\":null,\\\"Required_If\\\":null,\\\"Editable_If\\\":null,\\\"Reset_If\\\":null,\\\"Suggested_Values\\\":null}\",\"ReferencedKeyColumn\":\"ID_ทำเบิกส่วนต่างScgวังน้อย\",\"IsAPartOf\":false,\"RelationshipName\":null,\"InputMode\":\"Auto\",\"Valid_If\":null,\"Error_Message_If_Invalid\":null,\"Show_If\":null,\"Required_If\":null,\"Editable_If\":null,\"Reset_If\":null,\"Suggested_Values\":null}", "ItemSeparator": " , ", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 18. ราคารวม_ทำเบิกส่วนต่างScgวังน้อย

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
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**App Formula (สูตรคำนวณ):**

```
=SUM(SELECT( ทำเบิกส่วนต่างScgวังน้อย[ขออนุมัติเบิกค่าขนส่งส่วนเพิ่ม], AND(ISNOTBLANK([วันที่ส่งสินค้า]), [วันที่ส่งสินค้า] >= [_THISROW].[StartDate], [วันที่ส่งสินค้า] <= [_THISROW]. [EndDate], [สถานะ] = "ผ่านการตรวจสอบ" ) ))
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"CurrencySymbol": "฿", "MaxValue": null, "MinValue": null, "StepValue": null, "DecimalDigits": 2, "NumericDigits": null, "ShowThousandsSeparator": true, "NumberDisplayMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 19. สรุปจำนวนจุดส่งงาน

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
=SELECT( ตารางงานประจำวัน[ID_งานประจำวัน], AND( [ลำดับแรก] = TRUE, ISNOTBLANK([Plan Delivery]), [Plan Delivery] >= [_THISROW].[StartDate], [Plan Delivery] <= [_THISROW]. [EndDate] ) )
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"ElementType": "Ref", "ElementTypeQualifier": " {\"ReferencedTableName\":\"ตารางงานประจำ วัน\",\"ReferencedRootTableName\":\"ตารางงานประจำ วัน\",\"ReferencedType\":\"Text\",\"ReferencedTypeQualifier\":\"{\\\"MaxLength\\\":null,\\\"MinLength\\\":null,\\\"LongTextFor matting\\\":\\\"Plain Text\\\",\\\"IsMulticolumnKey\\\":false,\\\"Valid_If\\\":null,\\\"Error_Message_If_Invalid\\\":null,\\\"Show_If\\\":null,\\\"Required_If\\\":null,\\\"Editable_If\\\":null,\\\"Reset_If\\\":null,\\\"Suggested_Values\\\":null}\",\"ReferencedKeyColumn\":\"ID_งานประจำ วัน\",\"IsAPartOf\":false,\"RelationshipName\":null,\"InputMode\":\"Auto\",\"Valid_If\":null,\"Error_Message_If_Invalid\":null,\"Show_If\":null,\"Required_If\":null,\"Editable_If\":null,\"Reset_If\":null,\"Suggested_Values\":null}", "ItemSeparator": " , ", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 20. ได้เพิ่ม200_ไม่มีสินค้าคืน_ร้านปิด_ไม่มีในจุดส่ง

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
=FILTER( รับงานคืนได้เงิน200, AND( ISNOTBLANK([วันที่เข้ารับ]), [วันที่เข้ารับ] >= [_THISROW].[StartDate], [วันที่เข้ารับ] <= [_THISROW].[EndDate], IN( [สถานะการเข้ารับสินค้า], LIST( "(ได้ เพิ่ม200) ไม่มีสินค้าคืน หรือ ร้านปิด", "(ได้เพิ่ม200) ไม่มีในจุด ที่ส่ง งานวันนี้" ) ) ) )
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"ElementType": "Ref", "ElementTypeQualifier": " {\"ReferencedTableName\":\"รับงานคืนได้ เงิน200\",\"ReferencedRootTableName\":\"รับงานคืนได้ เงิน200\",\"ReferencedType\":\"Text\",\"ReferencedTypeQualifier\":\" {\\\"MaxLength\\\":null,\\\"MinLength\\\":null,\\\"LongTextFor matting\\\":\\\"Plain Text\\\",\\\"IsMulticolumnKey\\\":false,\\\"Valid_If\\\":null,\\\"Error_Message_If_Invalid\\\":null,\\\"Show_If\\\":null,\\\"Required_If\\\":null,\\\"Editable_If\\\":null,\\\"Reset_If\\\":null,\\\"Suggested_Values\\\":null}\",\"ReferencedKeyColumn\":\"ID_รับงานคืน ได้ เงิน200\",\"IsAPartOf\":false,\"RelationshipName\":null,\"InputMode\":\"Auto\",\"Valid_If\":null,\"Error_Message_If_Invalid\":null,\"Show_If\":null,\"Required_If\":null,\"Editable_If\":null,\"Reset_If\":null,\"Suggested_Values\":null}", "ItemSeparator": " , ", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 21. ทำเบิกค่ายกขึ้นชั้น

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
=FILTER( รับงานคืนได้เงิน200, AND( ISNOTBLANK([วันที่เข้ารับ]), [วันที่เข้ารับ] >= [_THISROW].[StartDate], [วันที่เข้ารับ] <= [_THISROW].[EndDate], [สถานะการเข้ารับสินค้า]="ทำเบิกค่ายกขึ้น ชั้น"))
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"ElementType": "Ref", "ElementTypeQualifier": " {\"ReferencedTableName\":\"รับงานคืนได้ เงิน200\",\"ReferencedRootTableName\":\"รับงานคืนได้ เงิน200\",\"ReferencedType\":\"Text\",\"ReferencedTypeQualifier\":\" {\\\"MaxLength\\\":null,\\\"MinLength\\\":null,\\\"LongTextFor matting\\\":\\\"Plain Text\\\",\\\"IsMulticolumnKey\\\":false,\\\"Valid_If\\\":null,\\\"Error_Message_If_Invalid\\\":null,\\\"Show_If\\\":null,\\\"Required_If\\\":null,\\\"Editable_If\\\":null,\\\"Reset_If\\\":null,\\\"Suggested_Values\\\":null}\",\"ReferencedKeyColumn\":\"ID_รับงานคืน ได้ เงิน200\",\"IsAPartOf\":false,\"RelationshipName\":null,\"InputMode\":\"Auto\",\"Valid_If\":null,\"Error_Message_If_Invalid\":null,\"Show_If\":null,\"Required_If\":null,\"Editable_If\":null,\"Reset_If\":null,\"Suggested_Values\":null}", "ItemSeparator": " , ", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 22. ได้เพิ่ม50%ของค่าเที่ยว

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
=FILTER( รับงานคืนได้เงิน200, AND( ISNOTBLANK([วันที่เข้ารับ]), [วันที่เข้ารับ] >= [_THISROW].[StartDate], [วันที่เข้ารับ] <= [_THISROW].[EndDate], [สถานะการเข้ารับสินค้า] = "(ได้เพิ่ม50%) ของค่าเที่ยว"))
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"ElementType": "Ref", "ElementTypeQualifier": " {\"ReferencedTableName\":\"รับงานคืนได้ เงิน200\",\"ReferencedRootTableName\":\"รับงานคืนได้ เงิน200\",\"ReferencedType\":\"Text\",\"ReferencedTypeQualifier\":\" {\\\"MaxLength\\\":null,\\\"MinLength\\\":null,\\\"LongTextFor matting\\\":\\\"Plain Text\\\",\\\"IsMulticolumnKey\\\":false,\\\"Valid_If\\\":null,\\\"Error_Message_If_Invalid\\\":null,\\\"Show_If\\\":null,\\\"Required_If\\\":null,\\\"Editable_If\\\":null,\\\"Reset_If\\\":null,\\\"Suggested_Values\\\":null}\",\"ReferencedKeyColumn\":\"ID_รับงานคืน ได้ เงิน200\",\"IsAPartOf\":false,\"RelationshipName\":null,\"InputMode\":\"Auto\",\"Valid_If\":null,\"Error_Message_If_Invalid\":null,\"Show_If\":null,\"Required_If\":null,\"Editable_If\":null,\"Reset_If\":null,\"Suggested_Values\":null}", "ItemSeparator": " , ", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 23. ราคา_ได้เพิ่ม200_ไม่มีสินค้าคืน_ร้านปิด_ไม่มีในจุดส่ง

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
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**App Formula (สูตรคำนวณ):**

```
=SUM(SELECT( รับงานคืนได้เงิน200[ราคา], AND( ISNOTBLANK([วันที่เข้ารับ]), [วันที่เข้ารับ] >= [_THISROW]. [StartDate], [วันที่เข้ารับ] <= [_THISROW].[EndDate], IN( [สถานะการเข้ารับสินค้า], LIST( "(ได้เพิ่ม200) ไม่มีสินค้าคืน หรือ ร้านปิด", " (ได้เพิ่ม200) ไม่มีในจุด ที่ส่งงานวันนี้" ) ) ) ))
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"CurrencySymbol": "฿", "MaxValue": null, "MinValue": null, "StepValue": null, "DecimalDigits": 2, "NumericDigits": null, "ShowThousandsSeparator": true, "NumberDisplayMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 24. ราคา_ทำเบิกค่ายกขึ้นชั้น

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
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**App Formula (สูตรคำนวณ):**

```
=SUM(SELECT( รับงานคืนได้เงิน200[ราคา], AND( ISNOTBLANK([วันที่เข้ารับ]), [วันที่เข้ารับ] >= [_THISROW]. [StartDate], [วันที่เข้ารับ] <= [_THISROW].[EndDate], [สถานะการเข้ารับสินค้า] = "ทำเบิกค่ายกขึ้นชั้น")))
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"CurrencySymbol": "฿", "MaxValue": null, "MinValue": null, "StepValue": null, "DecimalDigits": 2, "NumericDigits": null, "ShowThousandsSeparator": true, "NumberDisplayMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 25. ราคา_ได้เพิ่ม50%ของค่าเที่ยว

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
| ข้อมูลอ่อนไหว | No Schema Name ScanDocs_Schema |
| Locale | en-GB |

**App Formula (สูตรคำนวณ):**

```
=SUM(SELECT( รับงานคืนได้เงิน200[ราคา], AND( ISNOTBLANK([วันที่เข้ารับ]), [วันที่เข้ารับ] >= [_THISROW]. [StartDate], [วันที่เข้ารับ] <= [_THISROW].[EndDate], [สถานะการเข้ารับสินค้า] = "(ได้เพิ่ม50%) ของค่าเที่ยว")))
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"CurrencySymbol": "฿", "MaxValue": null, "MinValue": null, "StepValue": null, "DecimalDigits": 2, "NumericDigits": null, "ShowThousandsSeparator": true, "NumberDisplayMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

## คอลัมน์ทั่วไป (ไม่มีสูตรหรือเงื่อนไขพิเศษ)

- **5. StartDate** — ชนิด `Date` (ค่าปกติ)
- **6. EndDate** — ชนิด `Date` (ค่าปกติ)
- **8. Export to xlsx** — ชนิด `Yes/No` (ค่าปกติ)
- **9. Export to xlsx To Athens** — ชนิด `Yes/No` (ค่าปกติ)
- **10. ปริ๊นใบวางบิลแยกตามชื่องาน** — ชนิด `Yes/No` (ค่าปกติ)
- **13. Export to XLSX_12** — ชนิด `Yes/No` (ค่าปกติ)
- **14. EXPORT TO PDFรับคืน** — ชนิด `Yes/No` (ค่าปกติ)

