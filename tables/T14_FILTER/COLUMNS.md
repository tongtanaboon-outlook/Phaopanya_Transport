# คอลัมน์ของตาราง FILTER

รวม **14 คอลัมน์** (จาก Schema `FILTER_Schema`)

| # | ชื่อคอลัมน์ | ชนิด | สถานะ | สูตร/เงื่อนไข |
|---:|---|---|---|---|
| 1 | _RowNumber | Number | 🔒 🙈 ⚙️ |  |
| 2 | ID_เบิกค่าเข้ารับสินค้าคืนคลัง | Text | 🔑 🏷️ | InitValue |
| 3 | STARTDATE | Date |  |  |
| 4 | ENDDATE | Date |  |  |
| 5 | วันที่ออกเอกสาร | Date |  | InitValue |
| 6 | EXPORT TO PDF | Yes/No |  |  |
| 7 | EXPORT TO Excel(สรุปจำนวนจุดส่งงาน) | Yes/No |  |  |
| 8 | ราคา_ได้เพิ่ม200_ไม่มีสินค้าคืน_ร้านปิด_ไม่มีในจุดส่ง | Price |  | AppFormula |
| 9 | ได้เพิ่ม200_ไม่มีสินค้าคืน_ร้านปิด_ไม่มีในจุดส่ง | List | 🔒 | AppFormula |
| 10 | สรุปจำนวนจุดส่งงาน | List | 🔒 | AppFormula |
| 11 | ทำเบิกค่ายกขึ้นชั้น | List | 🔒 | AppFormula |
| 12 | ราคา_ทำเบิกค่ายกขึ้นชั้น | Price | 🔒 | AppFormula |
| 13 | ได้เพิ่ม50%ของค่าเที่ยว | List | 🔒 | AppFormula |
| 14 | ราคา_ได้เพิ่ม50%ของค่าเที่ยว | Price | 🔒 | AppFormula |

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

### 2. ID_เบิกค่าเข้ารับสินค้าคืนคลัง

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

### 5. วันที่ออกเอกสาร

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

### 8. ราคา_ได้เพิ่ม200_ไม่มีสินค้าคืน_ร้านปิด_ไม่มีในจุดส่ง

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
| ค้นหาได้ | No |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**App Formula (สูตรคำนวณ):**

```
=SUM(SELECT( รับงานคืนได้เงิน200[ราคา], AND( ISNOTBLANK([วันที่เข้ารับ]), [วันที่เข้ารับ] >= [_THISROW]. [STARTDATE], [วันที่เข้ารับ] <= [_THISROW].[ENDDATE], IN( [สถานะการเข้ารับสินค้า], LIST( "(ได้เพิ่ม200) ไม่มีสินค้าคืน หรือ ร้านปิด", "(ได้เพิ่ม200) ไม่มีในจุด ที่ส่งงานวันนี้" ) ) ) ))
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"CurrencySymbol": "฿", "MaxValue": null, "MinValue": null, "StepValue": null, "DecimalDigits": 2, "NumericDigits": null, "ShowThousandsSeparator": true, "NumberDisplayMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 9. ได้เพิ่ม200_ไม่มีสินค้าคืน_ร้านปิด_ไม่มีในจุดส่ง

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
=FILTER( รับงานคืนได้เงิน200, AND( ISNOTBLANK([วันที่เข้ารับ]), [วันที่เข้ารับ] >= [_THISROW].[STARTDATE], [วันที่เข้ารับ] <= [_THISROW].[ENDDATE], IN( [สถานะการเข้ารับสินค้า], LIST( "(ได้ เพิ่ม200) ไม่มีสินค้าคืน หรือ ร้านปิด", "(ได้เพิ่ม200) ไม่มีในจุด ที่ส่ง งานวันนี้" ) ) ) )
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"ElementType": "Ref", "ElementTypeQualifier": " {\"ReferencedTableName\":\"รับงานคืนได้ เงิน200\",\"ReferencedRootTableName\":\"รับงานคืนได้ เงิน200\",\"ReferencedType\":\"Text\",\"ReferencedTypeQualifier\":\" {\\\"MaxLength\\\":null,\\\"MinLength\\\":null,\\\"LongTextFor matting\\\":\\\"Plain Text\\\",\\\"IsMulticolumnKey\\\":false,\\\"Valid_If\\\":null,\\\"Error_Message_If_Invalid\\\":null,\\\"Show_If\\\":null,\\\"Required_If\\\":null,\\\"Editable_If\\\":null,\\\"Reset_If\\\":null,\\\"Suggested_Values\\\":null}\",\"ReferencedKeyColumn\":\"ID_รับงานคืน ได้ เงิน200\",\"IsAPartOf\":false,\"RelationshipName\":null,\"InputMode\":\"Auto\",\"Valid_If\":null,\"Error_Message_If_Invalid\":null,\"Show_If\":null,\"Required_If\":null,\"Editable_If\":null,\"Reset_If\":null,\"Suggested_Values\":null}", "ItemSeparator": " , ", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 10. สรุปจำนวนจุดส่งงาน

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
=SELECT( ตารางงานประจำวัน[ID_งานประจำวัน], AND( [ลำดับแรก] = TRUE, ISNOTBLANK([Plan Delivery]), [Plan Delivery] >= [_THISROW].[STARTDATE], [Plan Delivery] <= [_THISROW]. [ENDDATE] ) )
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"ElementType": "Number", "ElementTypeQualifier": " {\"MaxValue\":null,\"MinValue\":null,\"StepValue\":null,\"NumericDigits\":null,\"ShowThousandsSeparator\":true,\"NumberDisplayMode\":\"Auto\",\"Valid_If\":null,\"Error_Message_If_Invalid\":null,\"Show_If\":null,\"Required_If\":null,\"Editable_If\":null,\"Reset_If\":null,\"Suggested_Values\":null}", "ItemSeparator": " , ", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 11. ทำเบิกค่ายกขึ้นชั้น

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
=FILTER( รับงานคืนได้เงิน200, AND( ISNOTBLANK([วันที่เข้ารับ]), [วันที่เข้ารับ] >= [_THISROW].[STARTDATE], [วันที่เข้ารับ] <= [_THISROW].[ENDDATE], [สถานะการเข้ารับสินค้า]="ทำเบิกค่ายก ขึ้นชั้น"))
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"ElementType": "Ref", "ElementTypeQualifier": " {\"ReferencedTableName\":\"รับงานคืนได้ เงิน200\",\"ReferencedRootTableName\":\"รับงานคืนได้ เงิน200\",\"ReferencedType\":\"Text\",\"ReferencedTypeQualifier\":\" {\\\"MaxLength\\\":null,\\\"MinLength\\\":null,\\\"LongTextFor matting\\\":\\\"Plain Text\\\",\\\"IsMulticolumnKey\\\":false,\\\"Valid_If\\\":null,\\\"Error_Message_If_Invalid\\\":null,\\\"Show_If\\\":null,\\\"Required_If\\\":null,\\\"Editable_If\\\":null,\\\"Reset_If\\\":null,\\\"Suggested_Values\\\":null}\",\"ReferencedKeyColumn\":\"ID_รับงานคืน ได้ เงิน200\",\"IsAPartOf\":false,\"RelationshipName\":null,\"InputMode\":\"Auto\",\"Valid_If\":null,\"Error_Message_If_Invalid\":null,\"Show_If\":null,\"Required_If\":null,\"Editable_If\":null,\"Reset_If\":null,\"Suggested_Values\":null}", "ItemSeparator": " , ", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 12. ราคา_ทำเบิกค่ายกขึ้นชั้น

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
=SUM(SELECT( รับงานคืนได้เงิน200[ราคา], AND( ISNOTBLANK([วันที่เข้ารับ]), [วันที่เข้ารับ] >= [_THISROW]. [STARTDATE], [วันที่เข้ารับ] <= [_THISROW].[ENDDATE], [สถานะการเข้ารับสินค้า] = "ทำเบิกค่ายกขึ้นชั้น")))
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"CurrencySymbol": "฿", "MaxValue": null, "MinValue": null, "StepValue": null, "DecimalDigits": 2, "NumericDigits": null, "ShowThousandsSeparator": true, "NumberDisplayMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 13. ได้เพิ่ม50%ของค่าเที่ยว

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
=FILTER( รับงานคืนได้เงิน200, AND( ISNOTBLANK([วันที่เข้ารับ]), [วันที่เข้ารับ] >= [_THISROW].[STARTDATE], [วันที่เข้ารับ] <= [_THISROW].[ENDDATE], [สถานะการเข้ารับสินค้า] = "(ได้เพิ่ม50%) ของค่าเที่ยว"))
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"ElementType": "Ref", "ElementTypeQualifier": " {\"ReferencedTableName\":\"รับงานคืนได้ เงิน200\",\"ReferencedRootTableName\":\"รับงานคืนได้ เงิน200\",\"ReferencedType\":\"Text\",\"ReferencedTypeQualifier\":\" {\\\"MaxLength\\\":null,\\\"MinLength\\\":null,\\\"LongTextFor matting\\\":\\\"Plain Text\\\",\\\"IsMulticolumnKey\\\":false,\\\"Valid_If\\\":null,\\\"Error_Message_If_Invalid\\\":null,\\\"Show_If\\\":null,\\\"Required_If\\\":null,\\\"Editable_If\\\":null,\\\"Reset_If\\\":null,\\\"Suggested_Values\\\":null}\",\"ReferencedKeyColumn\":\"ID_รับงานคืน ได้ เงิน200\",\"IsAPartOf\":false,\"RelationshipName\":null,\"InputMode\":\"Auto\",\"Valid_If\":null,\"Error_Message_If_Invalid\":null,\"Show_If\":null,\"Required_If\":null,\"Editable_If\":null,\"Reset_If\":null,\"Suggested_Values\":null}", "ItemSeparator": " , ", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 14. ราคา_ได้เพิ่ม50%ของค่าเที่ยว

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
| ข้อมูลอ่อนไหว | No Schema Name ข้อมูลพนักงาน_Schema |
| Locale | en-GB |

**App Formula (สูตรคำนวณ):**

```
=SUM(SELECT( รับงานคืนได้เงิน200[ราคา], AND( ISNOTBLANK([วันที่เข้ารับ]), [วันที่เข้ารับ] >= [_THISROW]. [STARTDATE], [วันที่เข้ารับ] <= [_THISROW].[ENDDATE], [สถานะการเข้ารับสินค้า] = "(ได้เพิ่ม50%) ของค่าเที่ยว")))
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"CurrencySymbol": "฿", "MaxValue": null, "MinValue": null, "StepValue": null, "DecimalDigits": 2, "NumericDigits": null, "ShowThousandsSeparator": true, "NumberDisplayMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

## คอลัมน์ทั่วไป (ไม่มีสูตรหรือเงื่อนไขพิเศษ)

- **3. STARTDATE** — ชนิด `Date` (ค่าปกติ)
- **4. ENDDATE** — ชนิด `Date` (ค่าปกติ)
- **6. EXPORT TO PDF** — ชนิด `Yes/No` (ค่าปกติ)
- **7. EXPORT TO Excel(สรุปจำนวนจุดส่งงาน)** — ชนิด `Yes/No` (ค่าปกติ)

