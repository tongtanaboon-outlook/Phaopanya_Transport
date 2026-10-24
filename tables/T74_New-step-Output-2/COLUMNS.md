# คอลัมน์ของตาราง New step Output 2

รวม **49 คอลัมน์** (จาก Schema `New step Output 2_Schema`)

| # | ชื่อคอลัมน์ | ชนิด | สถานะ | สูตร/เงื่อนไข |
|---:|---|---|---|---|
| 1 | Instance Id | Text | 🔑 |  |
| 2 | head | LongText |  |  |
| 3 | ID_SCGนครหลวงJWDภูมิภาค | Text |  |  |
| 4 | วันที่ส่งสินค้า | Date |  | Editable_If |
| 5 | เวลาที่ส่งสินค้า | Time |  | Editable_If |
| 6 | จุดส่งสินค้าปลายทาง | LatLong |  | Valid_If, Editable_If |
| 7 | ชื่อ - นามสกุล | Text |  |  |
| 8 | ทะเบียนรถ | Text |  |  |
| 9 | Shipment No | Number |  | Valid_If |
| 10 | Invoice No | EnumList |  | Valid_If, Editable_If |
| 11 | รูปถ่ายบิลส่งสินค้า | Image |  |  |
| 12 | รหัสลูกค้า | Text |  | Editable_If, Show_If, Reset_If |
| 13 | ชื่อเจ้าของสินค้า | Text |  | Editable_If, Show_If, Reset_If |
| 14 | ชื่อปลายทาง | Text |  | Editable_If, Show_If, Reset_If |
| 15 | Email พนักงาน | Email |  | Editable_If |
| 16 | LAT | Decimal |  |  |
| 17 | LONG | Decimal |  |  |
| 18 | ID_Doc_Return | Ref |  | Editable_If, Reset_If |
| 19 | คลังสินค้า เอสซีจี เจดับเบิ้ลยูดี วังน้อย | LatLong |  |  |
| 20 | ที่อยู่ปลายทาง | LongText |  | Editable_If, Show_If, Reset_If |
| 21 | รูปสินค้าตอนส่ง | Image |  |  |
| 22 | รูปหน้าร้าน / บ้าน | Image |  |  |
| 23 | หมายเหตุ | LongText |  | Show_If |
| 24 | เดือน | Text |  |  |
| 25 | ระยะทางจากคลัง_Km | Decimal |  |  |
| 26 | ชื่อที่อยู่จาก_LatLong | LongText |  |  |
| 27 | SM_Link_SCG | Ref |  |  |
| 28 | ID_พนักงาน | Ref |  | Editable_If, Show_If |
| 29 | พิกัดตอนกดบันทึกงาน | LatLong |  | Reset_If |
| 30 | เวลาเริ่มกรอกงาน | Time |  |  |
| 31 | เวลาบันทึกงานสำเร็จ | Time |  | Reset_If |
| 32 | ระยะขยับจากจุดเริ่มต้น_เมตร | Decimal |  |  |
| 33 | ระยะเวลาใช้งาน_นาที | Duration |  |  |
| 34 | ความเร็วการเคลื่อนที่_เมตร_นาที | Decimal |  |  |
| 35 | ผลการตรวจสอบงานส่ง | Enum |  |  |
| 36 | เหตุผิดปกติที่ตรวจพบ | EnumList |  |  |
| 37 | เวลาถ่ายรูปหน้าร้าน_หน้าบ้าน | Time |  |  |
| 38 | SYNC_STATUS | Text |  |  |
| 39 | MD_LINK | Text |  |  |
| 40 | MATCH_KEY | Text |  |  |
| 41 | POINTS_AT_TIME | Number |  |  |
| 42 | STATUS | Text |  |  |
| 43 | เจ้าของสินค้า//ชื่อปลายทาง//Lat_Long//Inv No | LongText |  |  |
| 44 | Document_Return | LongText |  |  |
| 45 | Image_Document_Return | List |  |  |
| 46 | ที่อยู่ปลายทาง_LatLong_Api | LatLong |  |  |
| 47 | Related สรุปเบิกส่วนต่างs | List | 🔒 ⚙️ |  |
| 48 | Related ทำเบิกส่วนต่างScgวังน้อยs | List | 🔒 ⚙️ |  |
| 49 | พิกัดตอนกดบันทึก_เปลี่ยนแล้ว | Yes/No |  |  |

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

### 4. วันที่ส่งสินค้า

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
| นิยามคงที่ | Yes |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

**Editable_If (เงื่อนไขที่แก้ไขได้):**

```
=USERROLE()="ADMIN"
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"UseLongDateFormat": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": "=USERROLE()=\"ADMIN\"", "Reset_If": null, "Suggested_Values": null}
```

</details>

### 5. เวลาที่ส่งสินค้า

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Time |
| Key | No |
| Label | No |
| Virtual | No |
| Read-Only | No |
| Hidden | No |
| รีเซ็ตเมื่อแก้ไข | No |
| คอลัมน์ระบบ | No |
| ส่วนหนึ่งของ Key | No |
| นิยามคงที่ | Yes |
| ค้นหาได้ | No |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

**Editable_If (เงื่อนไขที่แก้ไขได้):**

```
=USERROLE()="ADMIN"
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MinValue": null, "MaxValue": null, "IgnoreSeconds": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": "=USERROLE()=\"ADMIN\"", "Reset_If": null, "Suggested_Values": null}
```

</details>

### 6. จุดส่งสินค้าปลายทาง

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | LatLong |
| Key | No |
| Label | No |
| Virtual | No |
| Read-Only | No |
| Hidden | No |
| รีเซ็ตเมื่อแก้ไข | No |
| คอลัมน์ระบบ | No |
| ส่วนหนึ่งของ Key | No |
| นิยามคงที่ | Yes |
| ค้นหาได้ | No |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

**Valid_If (เงื่อนไขความถูกต้อง):**

```
=AND(
 ISNOTBLANK([_THIS]),
 [_THIS] <> "0.000000, 0.000000",
 [_THIS] <> "0, 0"
)
```

**Editable_If (เงื่อนไขที่แก้ไขได้):**

```
=USERROLE()="ADMIN"
```

**ข้อความเตือนเมื่อค่าไม่ถูกต้อง:**

```
="ไม่สามารถให้บันทึกข้อมูล ได้ ไม่มีสัญญาณ GPS"
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"RealTime": false, "PublishIfRowKey": null, "KMLFileUrl": null, "Valid_If": "=AND(\n ISNOTBLANK([_THIS]),\n [_THIS] <> \"0.000000, 0.000000\",\n [_THIS] <> \"0, 0\"\n)", "Error_Message_If_Invalid": "=\"ไม่สามารถให้บันทึกข้อมูล ได้ ไม่มีสัญญาณ GPS\"", "Show_If": null, "Required_If": null, "Editable_If": "=USERROLE()=\"ADMIN\"", "Reset_If": null, "Suggested_Values": null}
```

</details>

### 9. Shipment No

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Number |
| Key | No |
| Label | No |
| Virtual | No |
| Read-Only | No |
| Hidden | No |
| รีเซ็ตเมื่อแก้ไข | No |
| คอลัมน์ระบบ | No |
| ส่วนหนึ่งของ Key | No |
| นิยามคงที่ | Yes |
| ค้นหาได้ | No |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

**Valid_If (เงื่อนไขความถูกต้อง):**

```
=SORT(
 UNIQUE(
 LIST([_THISROW]. [Shipment No])
 + SM_Today_User[Shipment No]
 )
)
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxValue": null, "MinValue": null, "StepValue": null, "NumericDigits": null, "ShowThousandsSeparator": false, "NumberDisplayMode": "Auto", "Valid_If": "=SORT(\n UNIQUE(\n LIST([_THISROW]. [Shipment No])\n + SM_Today_User[Shipment No]\n )\n)", "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": ""}
```

</details>

### 10. Invoice No

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | EnumList |
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
=IF(ISBLANK([Shipment No]),
 LIST(),
 UNIQUE(
 IF(USERROLE() = "ADMIN",
 SELECT(ตารางงานประจำวัน[Invoice No], [Shipment No] = [_THISROW].[Shipment No]),
 SELECT(SM_Today_User[Invoice No],
 AND(
 [Shipment No] = [_THISROW].[Shipment No],
 
NOT(IN([Invoice No], SCGนครหลวงJWDภูมิภาค[Invoice No]))
 )
 )
 )
 + [_THISROW].[Invoice No]
 ) -LIST("")
)
```

**Editable_If (เงื่อนไขที่แก้ไขได้):**

```
=OR(
 USERROLE() = "ADMIN",
 ISBLANK([_THISROW].[Invoice No])
)
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"ItemSeparator": ",", "EnumValues": [], "AllowOtherValues": true, "AutoCompleteOtherValues": true, "BaseType": "Text", "BaseTypeQualifier": " {\"MaxLength\":null,\"MinLength\":null,\"LongTextFormatting\":\"Plain Text\",\"IsMulticolumnKey\":false,\"Valid_If\":null,\"Error_Message_If_Invalid\":null,\"Show_If\":null,\"Required_If\":null,\"Editable_If\":null,\"Reset_If\":null,\"Suggested_Values\":null}", "EnumInputMode": "Dropdown", "Valid_If": "=IF(ISBLANK([Shipment No]),\n LIST(),\n UNIQUE(\n IF(USERROLE() = \"ADMIN\",\n SELECT(ตารางงานประจำวัน[Invoice No], [Shipment No] = [_THISROW].[Shipment No]),\n SELECT(SM_Today_User[Invoice No],\n AND(\n [Shipment No] = [_THISROW].[Shipment No],\n \nNOT(IN([Invoice No], SCGนครหลวงJWDภูมิภาค[Invoice No]))\n )\n )\n )\n + [_THISROW].[Invoice No]\n ) -LIST(\"\")\n)", "Error_Message_If_Invalid": null, "Show_If": "", "Required_If": null, "Editable_If": "=OR(\n USERROLE() = \"ADMIN\",\n ISBLANK([_THISROW].[Invoice No])\n)", "Reset_If": null, "Suggested_Values": ""}
```

</details>

### 12. รหัสลูกค้า

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Text |
| Key | No |
| Label | No |
| Virtual | No |
| Read-Only | No |
| Hidden | No |
| รีเซ็ตเมื่อแก้ไข | =[_THISROW_BEFORE].[Invoice No] <> [_THISROW].[Invoice No] |
| คอลัมน์ระบบ | No |
| ส่วนหนึ่งของ Key | No |
| นิยามคงที่ | Yes |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

**Editable_If (เงื่อนไขที่แก้ไขได้):**

```
=USERROLE() = "ADMIN"
```

**Show_If (เงื่อนไขการแสดง):**

```
=ISNOTBLANK([Invoice No])
```

**Reset_If (เงื่อนไขรีเซ็ต):**

```
=[_THISROW_BEFORE].[Invoice No] <> [_THISROW].[Invoice No]
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": "=ISNOTBLANK([Invoice No])", "Required_If": null, "Editable_If": "=USERROLE() = \"ADMIN\"", "Reset_If": "=[_THISROW_BEFORE].[Invoice No] <> [_THISROW].[Invoice No]", "Suggested_Values": null}
```

</details>

### 13. ชื่อเจ้าของสินค้า

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Text |
| Key | No |
| Label | No |
| Virtual | No |
| Read-Only | No |
| Hidden | No |
| รีเซ็ตเมื่อแก้ไข | =[_THISROW_BEFORE].[Invoice No] <> [_THISROW].[Invoice No] |
| คอลัมน์ระบบ | No |
| ส่วนหนึ่งของ Key | No |
| นิยามคงที่ | Yes |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

**Editable_If (เงื่อนไขที่แก้ไขได้):**

```
=USERROLE() = "ADMIN"
```

**Show_If (เงื่อนไขการแสดง):**

```
=ISNOTBLANK([Invoice No])
```

**Reset_If (เงื่อนไขรีเซ็ต):**

```
=[_THISROW_BEFORE].[Invoice No] <> [_THISROW].[Invoice No]
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": "=ISNOTBLANK([Invoice No])", "Required_If": null, "Editable_If": "=USERROLE() = \"ADMIN\"", "Reset_If": "=[_THISROW_BEFORE].[Invoice No] <> [_THISROW].[Invoice No]", "Suggested_Values": null}
```

</details>

### 14. ชื่อปลายทาง

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Text |
| Key | No |
| Label | No |
| Virtual | No |
| Read-Only | No |
| Hidden | No |
| รีเซ็ตเมื่อแก้ไข | =[_THISROW_BEFORE].[Invoice No] <> [_THISROW].[Invoice No] |
| คอลัมน์ระบบ | No |
| ส่วนหนึ่งของ Key | No |
| นิยามคงที่ | Yes |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

**Editable_If (เงื่อนไขที่แก้ไขได้):**

```
=USERROLE() = "ADMIN"
```

**Show_If (เงื่อนไขการแสดง):**

```
=ISNOTBLANK([Invoice No])
```

**Reset_If (เงื่อนไขรีเซ็ต):**

```
=[_THISROW_BEFORE].[Invoice No] <> [_THISROW].[Invoice No]
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": "=ISNOTBLANK([Invoice No])", "Required_If": null, "Editable_If": "=USERROLE() = \"ADMIN\"", "Reset_If": "=[_THISROW_BEFORE].[Invoice No] <> [_THISROW].[Invoice No]", "Suggested_Values": null}
```

</details>

### 15. Email พนักงาน

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Email |
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

**Editable_If (เงื่อนไขที่แก้ไขได้):**

```
=USERROLE()="ADMIN"
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": "=USERROLE()=\"ADMIN\"", "Reset_If": null, "Suggested_Values": null}
```

</details>

### 18. ID_Doc_Return

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Ref |
| Key | No |
| Label | No |
| Virtual | No |
| Read-Only | No |
| Hidden | No |
| รีเซ็ตเมื่อแก้ไข | =[_THISROW_BEFORE].[Invoice No] <> [_THISROW].[Invoice No] |
| คอลัมน์ระบบ | No |
| ส่วนหนึ่งของ Key | No |
| นิยามคงที่ | Yes |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

- 🔗 **อ้างอิง (Ref) ไปตาราง:** `Doc_Return`

**Editable_If (เงื่อนไขที่แก้ไขได้):**

```
=USERROLE()="ADMIN"
```

**Reset_If (เงื่อนไขรีเซ็ต):**

```
=[_THISROW_BEFORE].[Invoice No] <> [_THISROW].[Invoice No]
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"ReferencedTableName": "Doc_Return", "ReferencedRootTableName": "Doc_Return", "ReferencedType": "Text", "ReferencedTypeQualifier": " {\"MaxLength\":null,\"MinLength\":null,\"LongTextFormatting\":\"Plain Text\",\"IsMulticolumnKey\":false,\"Valid_If\":null,\"Error_Message_If_Invalid\":null,\"Show_If\":null,\"Required_If\":null,\"Editable_If\":null,\"Reset_If\":null,\"Suggested_Values\":null}", "ReferencedKeyColumn": "ID_Doc_Return", "IsAPartOf": false, "RelationshipName": null, "InputMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": "=USERROLE()=\"ADMIN\"", "Reset_If": "=[_THISROW_BEFORE].[Invoice No] <> [_THISROW].[Invoice No]", "Suggested_Values": null}
```

</details>

### 20. ที่อยู่ปลายทาง

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | LongText |
| Key | No |
| Label | No |
| Virtual | No |
| Read-Only | No |
| Hidden | No |
| รีเซ็ตเมื่อแก้ไข | =[_THISROW_BEFORE].[Invoice No] <> [_THISROW].[Invoice No] |
| คอลัมน์ระบบ | No |
| ส่วนหนึ่งของ Key | No |
| นิยามคงที่ | Yes |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

**Editable_If (เงื่อนไขที่แก้ไขได้):**

```
=USERROLE() = "ADMIN"
```

**Show_If (เงื่อนไขการแสดง):**

```
=ISNOTBLANK([Invoice No])
```

**Reset_If (เงื่อนไขรีเซ็ต):**

```
=[_THISROW_BEFORE].[Invoice No] <> [_THISROW].[Invoice No]
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": "=ISNOTBLANK([Invoice No])", "Required_If": null, "Editable_If": "=USERROLE() = \"ADMIN\"", "Reset_If": "=[_THISROW_BEFORE].[Invoice No] <> [_THISROW].[Invoice No]", "Suggested_Values": null}
```

</details>

### 23. หมายเหตุ

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | LongText |
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

**Show_If (เงื่อนไขการแสดง):**

```
=AND(
 ISNOTBLANK([รูปถ่ายบิลส่งสินค้า]),
 ISNOTBLANK([รูปสินค้าตอนส่ง]),
 ISNOTBLANK([รูปหน้าร้าน / บ้าน])
)
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": "=AND(\n ISNOTBLANK([รูปถ่ายบิลส่งสินค้า]),\n ISNOTBLANK([รูปสินค้าตอนส่ง]),\n ISNOTBLANK([รูปหน้าร้าน / บ้าน])\n)", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 28. ID_พนักงาน

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Ref |
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

- 🔗 **อ้างอิง (Ref) ไปตาราง:** `ข้อมูลพนักงาน`

**Editable_If (เงื่อนไขที่แก้ไขได้):**

```
=USERROLE()= "ADMIN"
```

**Show_If (เงื่อนไขการแสดง):**

```
=USERROLE()= "ADMIN"
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"ReferencedTableName": "ข้อมูลพนักงาน", "ReferencedRootTableName": "ข้อมูลพนักงาน", "ReferencedType": "Text", "ReferencedTypeQualifier": " {\"MaxLength\":null,\"MinLength\":null,\"LongTextFormatting\":\"Plain Text\",\"IsMulticolumnKey\":false,\"Valid_If\":null,\"Error_Message_If_Invalid\":null,\"Show_If\":null,\"Required_If\":null,\"Editable_If\":null,\"Reset_If\":null,\"Suggested_Values\":null}", "ReferencedKeyColumn": "ID_พนักงาน", "IsAPartOf": false, "RelationshipName": null, "InputMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": "=USERROLE()= \"ADMIN\"", "Required_If": null, "Editable_If": "=USERROLE()= \"ADMIN\"", "Reset_If": null, "Suggested_Values": null}
```

</details>

### 29. พิกัดตอนกดบันทึกงาน

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | LatLong |
| Key | No |
| Label | No |
| Virtual | No |
| Read-Only | No |
| Hidden | No |
| รีเซ็ตเมื่อแก้ไข | =ISNOTBLANK([หมายเหตุ]) |
| คอลัมน์ระบบ | No |
| ส่วนหนึ่งของ Key | No |
| นิยามคงที่ | Yes |
| ค้นหาได้ | No |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

**Reset_If (เงื่อนไขรีเซ็ต):**

```
=ISNOTBLANK([หมายเหตุ])
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"RealTime": false, "PublishIfRowKey": null, "KMLFileUrl": null, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": "=ISNOTBLANK([หมายเหตุ])", "Suggested_Values": null}
```

</details>

### 31. เวลาบันทึกงานสำเร็จ

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Time |
| Key | No |
| Label | No |
| Virtual | No |
| Read-Only | No |
| Hidden | No |
| รีเซ็ตเมื่อแก้ไข | =ISNOTBLANK([หมายเหตุ]) |
| คอลัมน์ระบบ | No |
| ส่วนหนึ่งของ Key | No |
| นิยามคงที่ | Yes |
| ค้นหาได้ | No |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

**Reset_If (เงื่อนไขรีเซ็ต):**

```
=ISNOTBLANK([หมายเหตุ])
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MinValue": null, "MaxValue": null, "IgnoreSeconds": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": "=ISNOTBLANK([หมายเหตุ])", "Suggested_Values": null}
```

</details>

### 47. Related สรุปเบิกส่วนต่างs

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | List |
| Key | No |
| Label | No |
| Virtual | No |
| Read-Only | Yes |
| Hidden | No |
| รีเซ็ตเมื่อแก้ไข | No |
| คอลัมน์ระบบ | Yes |
| ส่วนหนึ่งของ Key | No |
| นิยามคงที่ | Yes |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"ElementType": "Ref", "ElementTypeQualifier": " {\"ReferencedTableName\":\"สรุปเบิกส่วน ต่าง\",\"ReferencedRootTableName\":\"สรุปเบิกส่วน ต่าง\",\"ReferencedType\":\"Text\",\"ReferencedTypeQualifier\":\" {\\\"MaxLength\\\":null,\\\"MinLength\\\":null,\\\"LongTextFor matting\\\":\\\"Plain Text\\\",\\\"IsMulticolumnKey\\\":false,\\\"Valid_If\\\":null,\\\"Error_Message_If_Invalid\\\":null,\\\"Show_If\\\":null,\\\"Required_If\\\":null,\\\"Editable_If\\\":null,\\\"Reset_If\\\":null,\\\"Suggested_Values\\\":null}\",\"ReferencedKeyColumn\":\"ID_สรุปเบิก ส่วน ต่าง\",\"IsAPartOf\":false,\"RelationshipName\":null,\"InputMode\":\"Auto\",\"Valid_If\":null,\"Error_Message_If_Invalid\":null,\"Show_If\":null,\"Required_If\":null,\"Editable_If\":null,\"Reset_If\":null,\"Suggested_Values\":null}", "ItemSeparator": " , ", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 48. Related ทำเบิกส่วนต่างScgวังน้อยs

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | List |
| Key | No |
| Label | No |
| Virtual | No |
| Read-Only | Yes |
| Hidden | No |
| รีเซ็ตเมื่อแก้ไข | No |
| คอลัมน์ระบบ | Yes |
| ส่วนหนึ่งของ Key | No |
| นิยามคงที่ | Yes |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"ElementType": "Ref", "ElementTypeQualifier": " {\"ReferencedTableName\":\"ทำเบิกส่วน ต่างScgวังน้อย\",\"ReferencedRootTableName\":\"ทำเบิกส่วน ต่างScgวังน้อย\",\"ReferencedType\":\"Text\",\"ReferencedTypeQualifier\":\" {\\\"MaxLength\\\":null,\\\"MinLength\\\":null,\\\"LongTextFor matting\\\":\\\"Plain Text\\\",\\\"IsMulticolumnKey\\\":false,\\\"Valid_If\\\":null,\\\"Error_Message_If_Invalid\\\":null,\\\"Show_If\\\":null,\\\"Required_If\\\":null,\\\"Editable_If\\\":null,\\\"Reset_If\\\":null,\\\"Suggested_Values\\\":null}\",\"ReferencedKeyColumn\":\"ID_ทำเบิกส่วนต่างScgวังน้อย\",\"IsAPartOf\":false,\"RelationshipName\":null,\"InputMode\":\"Auto\",\"Valid_If\":null,\"Error_Message_If_Invalid\":null,\"Show_If\":null,\"Required_If\":null,\"Editable_If\":null,\"Reset_If\":null,\"Suggested_Values\":null}", "ItemSeparator": " , ", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

## คอลัมน์ทั่วไป (ไม่มีสูตรหรือเงื่อนไขพิเศษ)

- **2. head** — ชนิด `LongText` (ค่าปกติ)
- **3. ID_SCGนครหลวงJWDภูมิภาค** — ชนิด `Text` (ค่าปกติ)
- **7. ชื่อ - นามสกุล** — ชนิด `Text` (ค่าปกติ)
- **8. ทะเบียนรถ** — ชนิด `Text` (ค่าปกติ)
- **11. รูปถ่ายบิลส่งสินค้า** — ชนิด `Image` (ค่าปกติ)
- **16. LAT** — ชนิด `Decimal` (ค่าปกติ)
- **17. LONG** — ชนิด `Decimal` (ค่าปกติ)
- **19. คลังสินค้า เอสซีจี เจดับเบิ้ลยูดี วังน้อย** — ชนิด `LatLong` (ค่าปกติ)
- **21. รูปสินค้าตอนส่ง** — ชนิด `Image` (ค่าปกติ)
- **22. รูปหน้าร้าน / บ้าน** — ชนิด `Image` (ค่าปกติ)
- **24. เดือน** — ชนิด `Text` (ค่าปกติ)
- **25. ระยะทางจากคลัง_Km** — ชนิด `Decimal` (ค่าปกติ)
- **26. ชื่อที่อยู่จาก_LatLong** — ชนิด `LongText` (ค่าปกติ)
- **27. SM_Link_SCG** — ชนิด `Ref` (ค่าปกติ)
- **30. เวลาเริ่มกรอกงาน** — ชนิด `Time` (ค่าปกติ)
- **32. ระยะขยับจากจุดเริ่มต้น_เมตร** — ชนิด `Decimal` (ค่าปกติ)
- **33. ระยะเวลาใช้งาน_นาที** — ชนิด `Duration` (ค่าปกติ)
- **34. ความเร็วการเคลื่อนที่_เมตร_นาที** — ชนิด `Decimal` (ค่าปกติ)
- **35. ผลการตรวจสอบงานส่ง** — ชนิด `Enum` (ค่าปกติ)
- **36. เหตุผิดปกติที่ตรวจพบ** — ชนิด `EnumList` (ค่าปกติ)
- **37. เวลาถ่ายรูปหน้าร้าน_หน้าบ้าน** — ชนิด `Time` (ค่าปกติ)
- **38. SYNC_STATUS** — ชนิด `Text` (ค่าปกติ)
- **39. MD_LINK** — ชนิด `Text` (ค่าปกติ)
- **40. MATCH_KEY** — ชนิด `Text` (ค่าปกติ)
- **41. POINTS_AT_TIME** — ชนิด `Number` (ค่าปกติ)
- **42. STATUS** — ชนิด `Text` (ค่าปกติ)
- **43. เจ้าของสินค้า//ชื่อปลายทาง//Lat_Long//Inv No** — ชนิด `LongText` (ค่าปกติ)
- **44. Document_Return** — ชนิด `LongText` (ค่าปกติ)
- **45. Image_Document_Return** — ชนิด `List` (ค่าปกติ)
- **46. ที่อยู่ปลายทาง_LatLong_Api** — ชนิด `LatLong` (ค่าปกติ)
- **49. พิกัดตอนกดบันทึก_เปลี่ยนแล้ว** — ชนิด `Yes/No` (ค่าปกติ)

