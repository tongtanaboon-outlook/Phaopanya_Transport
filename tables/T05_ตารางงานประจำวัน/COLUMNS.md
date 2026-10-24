# คอลัมน์ของตาราง ตารางงานประจำวัน

รวม **40 คอลัมน์** (จาก Schema `ตารางงานประจำวัน_Schema`)

| # | ชื่อคอลัมน์ | ชนิด | สถานะ | สูตร/เงื่อนไข |
|---:|---|---|---|---|
| 1 | _RowNumber | Number | 🔒 🙈 ⚙️ |  |
| 2 | ID_งานประจำวัน | Text | 🔑 🔒 | InitValue |
| 3 | Plan Delivery | Date |  |  |
| 4 | Invoice No | Text | 🏷️ |  |
| 5 | Shipment No | Number |  |  |
| 6 | ชื่อ - นามสกุล | Text |  |  |
| 7 | ทะเบียนรถ | Text |  |  |
| 8 | รหัสผู้รับเหมา | Text |  |  |
| 9 | ชื่อผู้รับเหมา | Text |  |  |
| 10 | รหัสลูกค้า | Text |  |  |
| 11 | ชื่อเจ้าของสินค้า | Text |  |  |
| 12 | ชื่อปลายทาง | Text |  |  |
| 13 | ที่อยู่ปลายทาง | Text |  |  |
| 14 | ที่อยู่ปลายทาง_LatLong | LatLong |  |  |
| 15 | ชื่อวัสดุ | Text |  |  |
| 16 | จำนวนสินค้า | Number |  |  |
| 17 | หน่วย | Text |  |  |
| 18 | ItemWeight | Number |  |  |
| 19 | DeliveryNo | Text |  |  |
| 20 | จำนวนปลายทาง_System | Number |  |  |
| 21 | รายชื่อปลายทาง_System | Text |  |  |
| 22 | ScanStatus | Enum |  |  |
| 23 | DeliveryStatus | Text |  |  |
| 24 | Email พนักงาน | Email |  |  |
| 25 | จำนวนสินค้ารวมของร้านนี้ | Number |  |  |
| 26 | น้ำหนักสินค้ารวมของร้านนี้ | Decimal |  |  |
| 27 | จำนวน_Invoice_ที่ต้องสแกน | Number |  |  |
| 28 | LatLong_Actual | LatLong |  |  |
| 29 | ชื่อเจ้าของสินค้า_Invoice_ที่ต้องสแกน | LongText |  |  |
| 30 | ShopKey | Text |  |  |
| 31 | MATCH_KEY | Text |  |  |
| 32 | MD_ID | Text |  |  |
| 33 | LatLong_Actual_Status | Text |  |  |
| 34 | จำนวนปลายทาง | Number | 🔒 | AppFormula |
| 35 | ลำดับแรก | Yes/No | 🔒 | AppFormula |
| 36 | จำนวนจุดที่ส่งจริง | Number | 🔒 | AppFormula |
| 37 | เดือน | Text | 🔒 | AppFormula |
| 38 | Related SCGนครหลวงJWDภูมิภาคs | List | 🔒 ⚙️ | AppFormula |
| 39 | Related แจ้งปัญหาระหว่างวันs | List | 🔒 ⚙️ | AppFormula |
| 40 | Related ScanDocs | List | 🔒 ⚙️ | AppFormula |

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

### 2. ID_งานประจำวัน

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Text |
| Key | Yes |
| Label | No |
| Virtual | No |
| Read-Only | Yes |
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
=UNIQUEID()
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 4. Invoice No

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

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 34. จำนวนปลายทาง

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Number |
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
=COUNT( UNIQUE( SELECT( ตารางงานประจำวัน[ชื่อปลายทาง], [Shipment No] = [_THISROW].[Shipment No] ) ) )
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxValue": null, "MinValue": null, "StepValue": null, "NumericDigits": null, "ShowThousandsSeparator": false, "NumberDisplayMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 35. ลำดับแรก

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Yes/No |
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
=[_ROWNUMBER] = MIN( SELECT( ตารางงานประจำ วัน[_ROWNUMBER], [Shipment No] = [_THISROW].[Shipment No], ) )
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"YesLabel": "", "NoLabel": "", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 36. จำนวนจุดที่ส่งจริง

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Number |
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
=COUNT( SELECT( SCGนครหลวงJWDภูมิภาค[Shipment No], [Shipment No] = [_THISROW].[Shipment No]) )
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxValue": null, "MinValue": null, "StepValue": null, "NumericDigits": null, "ShowThousandsSeparator": false, "NumberDisplayMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 37. เดือน

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
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**App Formula (สูตรคำนวณ):**

```
=IF( ISBLANK([Plan Delivery]), "", CONCATENATE( YEAR([Plan Delivery]) - IF(YEAR([Plan Delivery]) > 2500, 543, 0), "-", TEXT([Plan Delivery], "MM") ) )
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 38. Related SCGนครหลวงJWDภูมิภาคs

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | List |
| Key | No |
| Label | No |
| Virtual | Yes |
| Read-Only | Yes |
| Hidden | No |
| รีเซ็ตเมื่อแก้ไข | No |
| คอลัมน์ระบบ | Yes |
| ส่วนหนึ่งของ Key | No |
| นิยามคงที่ | No |
| ค้นหาได้ | Yes |
| สแกนได้ | No NFC Scannable No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**App Formula (สูตรคำนวณ):**

```
=REF_ROWS("SCGนครหลวงJWDภูมิภาค", "SM_Link_SCG")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"ElementType": "Ref", "ElementTypeQualifier": " {\"ReferencedTableName\":\"SCGนครหลวงJWDภูมิภาค\",\"ReferencedRootTableName\":\"SCGนครหลวงJWDภูมิภาค\",\"ReferencedType\":\"Text\",\"ReferencedTypeQualifier\":\" {\\\"MaxLength\\\":null,\\\"MinLength\\\":null,\\\"LongTextFor matting\\\":\\\"Plain Text\\\",\\\"IsMulticolumnKey\\\":false,\\\"Valid_If\\\":null,\\\"Error_Message_If_Invalid\\\":null,\\\"Show_If\\\":null,\\\"Required_If\\\":null,\\\"Editable_If\\\":null,\\\"Reset_If\\\":null,\\\"Suggested_Values\\\":null}\",\"ReferencedKeyColumn\":\"ID_SCGนครหลวงJWDภูมิภาค\",\"IsAPartOf\":false,\"RelationshipName\":null,\"InputMode\":\"Auto\",\"Valid_If\":null,\"Error_Message_If_Invalid\":null,\"Show_If\":null,\"Required_If\":null,\"Editable_If\":null,\"Reset_If\":null,\"Suggested_Values\":null}", "ItemSeparator": " , ", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 39. Related แจ้งปัญหาระหว่างวันs

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | List |
| Key | No |
| Label | No |
| Virtual | Yes |
| Read-Only | Yes |
| Hidden | No |
| รีเซ็ตเมื่อแก้ไข | No |
| คอลัมน์ระบบ | Yes |
| ส่วนหนึ่งของ Key | No |
| นิยามคงที่ | No |
| ค้นหาได้ | Yes |
| สแกนได้ | No NFC Scannable No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**App Formula (สูตรคำนวณ):**

```
REF_ROWS("แจ้งปัญหาระหว่างวัน", "SM_Link")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"ElementType": "Ref", "ElementTypeQualifier": " {\"ReferencedTableName\":\"แจ้งปัญหาระหว่าง วัน\",\"ReferencedRootTableName\":\"แจ้งปัญหาระหว่าง วัน\",\"ReferencedType\":\"Text\",\"ReferencedTypeQualifier\":\"{\\\"MaxLength\\\":null,\\\"MinLength\\\":null,\\\"LongTextFor matting\\\":\\\"Plain Text\\\",\\\"IsMulticolumnKey\\\":false,\\\"Valid_If\\\":null,\\\"Error_Message_If_Invalid\\\":null,\\\"Show_If\\\":null,\\\"Required_If\\\":null,\\\"Editable_If\\\":null,\\\"Reset_If\\\":null,\\\"Suggested_Values\\\":null}\",\"ReferencedKeyColumn\":\"ID_แจ้งปัญหาระหว่าง วัน\",\"IsAPartOf\":false,\"RelationshipName\":null,\"InputMode\":\"Auto\",\"Valid_If\":null,\"Error_Message_If_Invalid\":null,\"Show_If\":null,\"Required_If\":null,\"Editable_If\":null,\"Reset_If\":null,\"Suggested_Values\":null}", "ItemSeparator": " , ", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 40. Related ScanDocs

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | List |
| Key | No |
| Label | No |
| Virtual | Yes |
| Read-Only | Yes |
| Hidden | No |
| รีเซ็ตเมื่อแก้ไข | No |
| คอลัมน์ระบบ | Yes |
| ส่วนหนึ่งของ Key | No |
| นิยามคงที่ | No |
| ค้นหาได้ | Yes |
| สแกนได้ | No NFC Scannable No |
| ข้อมูลอ่อนไหว | No Schema Name ราคาน้ำมันดีเซล_Schema |
| Locale | en-GB |

**App Formula (สูตรคำนวณ):**

```
REF_ROWS("ScanDocs", "Invoice_No")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"ElementType": "Ref", "ElementTypeQualifier": " {\"ReferencedTableName\":\"ScanDocs\",\"ReferencedRootTableName\":\"ScanDocs\",\"ReferencedType\":\"Text\",\"ReferencedTypeQualifier\":\" {\\\"MaxLength\\\":null,\\\"MinLength\\\":null,\\\"LongTextFor matting\\\":\\\"Plain Text\\\",\\\"IsMulticolumnKey\\\":false,\\\"Valid_If\\\":null,\\\"Error_Message_If_Invalid\\\":null,\\\"Show_If\\\":null,\\\"Required_If\\\":null,\\\"Editable_If\\\":null,\\\"Reset_If\\\":null,\\\"Suggested_Values\\\":null}\",\"ReferencedKeyColumn\":\"ID_ScanDocs\",\"IsAPartOf\":false,\"RelationshipName\":null,\"InputMode\":\"Auto\",\"Valid_If\":null,\"Error_Message_If_Invalid\":null,\"Show_If\":null,\"Required_If\":null,\"Editable_If\":null,\"Reset_If\":null,\"Suggested_Values\":null}", "ItemSeparator": " , ", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

## คอลัมน์ทั่วไป (ไม่มีสูตรหรือเงื่อนไขพิเศษ)

- **3. Plan Delivery** — ชนิด `Date` (ค่าปกติ)
- **5. Shipment No** — ชนิด `Number` (ค่าปกติ)
- **6. ชื่อ - นามสกุล** — ชนิด `Text` (ค่าปกติ)
- **7. ทะเบียนรถ** — ชนิด `Text` (ค่าปกติ)
- **8. รหัสผู้รับเหมา** — ชนิด `Text` (ค่าปกติ)
- **9. ชื่อผู้รับเหมา** — ชนิด `Text` (ค่าปกติ)
- **10. รหัสลูกค้า** — ชนิด `Text` (ค่าปกติ)
- **11. ชื่อเจ้าของสินค้า** — ชนิด `Text` (ค่าปกติ)
- **12. ชื่อปลายทาง** — ชนิด `Text` (ค่าปกติ)
- **13. ที่อยู่ปลายทาง** — ชนิด `Text` (ค่าปกติ)
- **14. ที่อยู่ปลายทาง_LatLong** — ชนิด `LatLong` (ค่าปกติ)
- **15. ชื่อวัสดุ** — ชนิด `Text` (ค่าปกติ)
- **16. จำนวนสินค้า** — ชนิด `Number` (ค่าปกติ)
- **17. หน่วย** — ชนิด `Text` (ค่าปกติ)
- **18. ItemWeight** — ชนิด `Number` (ค่าปกติ)
- **19. DeliveryNo** — ชนิด `Text` (ค่าปกติ)
- **20. จำนวนปลายทาง_System** — ชนิด `Number` (ค่าปกติ)
- **21. รายชื่อปลายทาง_System** — ชนิด `Text` (ค่าปกติ)
- **22. ScanStatus** — ชนิด `Enum` (ค่าปกติ)
- **23. DeliveryStatus** — ชนิด `Text` (ค่าปกติ)
- **24. Email พนักงาน** — ชนิด `Email` (ค่าปกติ)
- **25. จำนวนสินค้ารวมของร้านนี้** — ชนิด `Number` (ค่าปกติ)
- **26. น้ำหนักสินค้ารวมของร้านนี้** — ชนิด `Decimal` (ค่าปกติ)
- **27. จำนวน_Invoice_ที่ต้องสแกน** — ชนิด `Number` (ค่าปกติ)
- **28. LatLong_Actual** — ชนิด `LatLong` (ค่าปกติ)
- **29. ชื่อเจ้าของสินค้า_Invoice_ที่ต้องสแกน** — ชนิด `LongText` (ค่าปกติ)
- **30. ShopKey** — ชนิด `Text` (ค่าปกติ)
- **31. MATCH_KEY** — ชนิด `Text` (ค่าปกติ)
- **32. MD_ID** — ชนิด `Text` (ค่าปกติ)
- **33. LatLong_Actual_Status** — ชนิด `Text` (ค่าปกติ)

