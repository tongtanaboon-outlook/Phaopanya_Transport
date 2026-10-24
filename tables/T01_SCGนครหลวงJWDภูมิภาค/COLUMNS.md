# คอลัมน์ของตาราง SCGนครหลวงJWDภูมิภาค

รวม **49 คอลัมน์** (จาก Schema `SCGนครหลวงJWDภูมิภาค_Schema`)

| # | ชื่อคอลัมน์ | ชนิด | สถานะ | สูตร/เงื่อนไข |
|---:|---|---|---|---|
| 1 | _RowNumber | Number | 🔒 🙈 ⚙️ |  |
| 2 | head | LongText |  |  |
| 3 | ID_SCGนครหลวงJWDภูมิภาค | Text | 🔑 🏷️ 🔒 | InitValue |
| 4 | วันที่ส่งสินค้า | Date |  | InitValue, Editable_If |
| 5 | เวลาที่ส่งสินค้า | Time |  | InitValue, Editable_If |
| 6 | จุดส่งสินค้าปลายทาง | LatLong |  | InitValue, Valid_If, Editable_If |
| 7 | ชื่อ - นามสกุล | Text | 🔒 | InitValue |
| 8 | ทะเบียนรถ | Text | 🔒 | InitValue |
| 9 | Shipment No | Number |  | Valid_If |
| 10 | Invoice No | EnumList |  | Valid_If, Editable_If |
| 11 | รูปถ่ายบิลส่งสินค้า | Image | 🏷️ |  |
| 12 | รหัสลูกค้า | Text |  | InitValue, Editable_If, Show_If, Reset_If |
| 13 | ชื่อเจ้าของสินค้า | Text |  | InitValue, Editable_If, Show_If, Reset_If |
| 14 | ชื่อปลายทาง | Text |  | InitValue, Editable_If, Show_If, Reset_If |
| 15 | Email พนักงาน | Email |  | InitValue, Editable_If |
| 16 | LAT | Decimal | 🔒 | InitValue |
| 17 | LONG | Decimal | 🔒 | InitValue |
| 18 | ID_Doc_Return | Ref |  | InitValue, Editable_If, Reset_If |
| 19 | คลังสินค้า เอสซีจี เจดับเบิ้ลยูดี วังน้อย | LatLong | 🔒 | InitValue |
| 20 | ที่อยู่ปลายทาง | LongText |  | InitValue, Editable_If, Show_If, Reset_If |
| 21 | รูปสินค้าตอนส่ง | Image |  |  |
| 22 | รูปหน้าร้าน / บ้าน | Image |  |  |
| 23 | หมายเหตุ | LongText |  | Show_If |
| 24 | เดือน | Text | 🔒 | InitValue |
| 25 | ระยะทางจากคลัง_Km | Decimal |  |  |
| 26 | ชื่อที่อยู่จาก_LatLong | LongText |  |  |
| 27 | SM_Link_SCG | Ref |  | InitValue |
| 28 | ID_พนักงาน | Ref |  | InitValue, Editable_If, Show_If |
| 29 | พิกัดตอนกดบันทึกงาน | LatLong |  | InitValue, Reset_If |
| 30 | เวลาเริ่มกรอกงาน | Time | 🔒 | InitValue |
| 31 | เวลาบันทึกงานสำเร็จ | Time |  | InitValue, Reset_If |
| 32 | ระยะขยับจากจุดเริ่มต้น_เมตร | Decimal |  | AppFormula |
| 33 | ระยะเวลาใช้งาน_นาที | Duration |  | AppFormula |
| 34 | ความเร็วการเคลื่อนที่_เมตร_นาที | Decimal |  | AppFormula |
| 35 | ผลการตรวจสอบงานส่ง | Enum |  | AppFormula |
| 36 | เหตุผิดปกติที่ตรวจพบ | EnumList |  | AppFormula |
| 37 | เวลาถ่ายรูปหน้าร้าน_หน้าบ้าน | Time | 🔒 | InitValue |
| 38 | SYNC_STATUS | Text |  |  |
| 39 | MD_LINK | Text |  |  |
| 40 | MATCH_KEY | Text |  |  |
| 41 | POINTS_AT_TIME | Number |  |  |
| 42 | STATUS | Text |  |  |
| 43 | เจ้าของสินค้า//ชื่อปลายทาง//Lat_Long//Inv No | LongText | 🔒 | AppFormula |
| 44 | Document_Return | LongText | 🔒 | AppFormula |
| 45 | Image_Document_Return | List | 🔒 | AppFormula |
| 46 | ที่อยู่ปลายทาง_LatLong_Api | LatLong | 🔒 | AppFormula |
| 47 | Related สรุปเบิกส่วนต่างs | List | 🔒 ⚙️ | AppFormula |
| 48 | Related ทำเบิกส่วนต่างScgวังน้อยs | List | 🔒 ⚙️ | AppFormula |
| 49 | พิกัดตอนกดบันทึก_เปลี่ยนแล้ว | Yes/No | 🔒 | AppFormula |

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

### 3. ID_SCGนครหลวงJWDภูมิภาค

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Text |
| Key | Yes |
| Label | Yes |
| Virtual | No |
| Read-Only | Yes |
| Hidden | No |
| รีเซ็ตเมื่อแก้ไข | No |
| คอลัมน์ระบบ | No |
| ส่วนหนึ่งของ Key | Yes |
| นิยามคงที่ | No |
| ค้นหาได้ | No |
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
| นิยามคงที่ | No |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**ค่าเริ่มต้น (Initial Value):**

```
=TODAY()
```

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
| นิยามคงที่ | No |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**ค่าเริ่มต้น (Initial Value):**

```
=TIMENOW()
```

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
| นิยามคงที่ | No |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**ค่าเริ่มต้น (Initial Value):**

```
=HERE()
```

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

### 7. ชื่อ - นามสกุล

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Text |
| Key | No |
| Label | No |
| Virtual | No |
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

**ค่าเริ่มต้น (Initial Value):**

```
=[ID_พนักงาน].[ชื่อ - นามสกุล]
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": "", "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 8. ทะเบียนรถ

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Text |
| Key | No |
| Label | No |
| Virtual | No |
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

**ค่าเริ่มต้น (Initial Value):**

```
=[ID_พนักงาน].[ทะเบียนรถ]
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
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
| นิยามคงที่ | No |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

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
| นิยามคงที่ | No |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

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

### 11. รูปถ่ายบิลส่งสินค้า

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
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
| นิยามคงที่ | No |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**ค่าเริ่มต้น (Initial Value):**

```
=[SM_Link_SCG].[รหัสลูกค้า]
```

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
| นิยามคงที่ | No |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**ค่าเริ่มต้น (Initial Value):**

```
=[SM_Link_SCG].[ชื่อเจ้าของสินค้า]
```

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
| นิยามคงที่ | No |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**ค่าเริ่มต้น (Initial Value):**

```
=[SM_Link_SCG].[ชื่อปลายทาง]
```

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
| นิยามคงที่ | No |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**ค่าเริ่มต้น (Initial Value):**

```
=USEREMAIL()
```

**Editable_If (เงื่อนไขที่แก้ไขได้):**

```
=USERROLE()="ADMIN"
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": "=USERROLE()=\"ADMIN\"", "Reset_If": null, "Suggested_Values": null}
```

</details>

### 16. LAT

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Decimal |
| Key | No |
| Label | No |
| Virtual | No |
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

**ค่าเริ่มต้น (Initial Value):**

```
=LAT([จุดส่งสินค้าปลายทาง])
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxValue": null, "MinValue": null, "StepValue": null, "DecimalDigits": 6, "NumericDigits": null, "ShowThousandsSeparator": false, "NumberDisplayMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 17. LONG

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Decimal |
| Key | No |
| Label | No |
| Virtual | No |
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

**ค่าเริ่มต้น (Initial Value):**

```
=LONG([จุดส่งสินค้าปลายทาง])
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxValue": null, "MinValue": null, "StepValue": null, "DecimalDigits": 6, "NumericDigits": null, "ShowThousandsSeparator": false, "NumberDisplayMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
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
| นิยามคงที่ | No |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

- 🔗 **อ้างอิง (Ref) ไปตาราง:** `Doc_Return`

**ค่าเริ่มต้น (Initial Value):**

```
=LOOKUP( [_THISROW].[รหัสลูกค้า], "Doc_Return", "รหัสลูกค้า", "ID_Doc_Return" )
```

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

### 19. คลังสินค้า เอสซีจี เจดับเบิ้ลยูดี วังน้อย

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | LatLong |
| Key | No |
| Label | No |
| Virtual | No |
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

**ค่าเริ่มต้น (Initial Value):**

```
="14.165716365156051, 100.62529569032515"
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"RealTime": false, "PublishIfRowKey": null, "KMLFileUrl": null, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
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
| นิยามคงที่ | No |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**ค่าเริ่มต้น (Initial Value):**

```
=[SM_Link_SCG].[ที่อยู่ปลายทาง]
```

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
| นิยามคงที่ | No |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

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

### 24. เดือน

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Text |
| Key | No |
| Label | No |
| Virtual | No |
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

**ค่าเริ่มต้น (Initial Value):**

```
=IF( ISBLANK([วันที่ส่งสินค้า]), "", CONCATENATE( YEAR([วันที่ส่งสินค้า]) - IF(YEAR([วันที่ส่งสินค้า]) > 2500, 543, 0), "-", TEXT([วันที่ส่งสินค้า], "MM") ) )
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 27. SM_Link_SCG

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
| นิยามคงที่ | No |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

- 🔗 **อ้างอิง (Ref) ไปตาราง:** `ตารางงานประจำวัน`

**ค่าเริ่มต้น (Initial Value):**

```
=ANY(SELECT(ตารางงานประจำวัน[ID_งานประจำวัน], AND([Invoice No] = ANY([_THISROW].[Invoice No]), [_ROWNUMBER] = MIN(SELECT(ตารางงานประจำ วัน[_ROWNUMBER], [Invoice No] = ANY([_THISROW].[Invoice No]))))))
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"ReferencedTableName": "ตารางงานประจำวัน", "ReferencedRootTableName": "ตารางงานประจำวัน", "ReferencedType": "Text", "ReferencedTypeQualifier": " {\"MaxLength\":null,\"MinLength\":null,\"LongTextFormatting\":\"Plain Text\",\"IsMulticolumnKey\":false,\"Valid_If\":null,\"Error_Message_If_Invalid\":null,\"Show_If\":null,\"Required_If\":null,\"Editable_If\":null,\"Reset_If\":null,\"Suggested_Values\":null}", "ReferencedKeyColumn": "ID_งานประจำ วัน", "IsAPartOf": false, "RelationshipName": null, "InputMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
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
| นิยามคงที่ | No |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

- 🔗 **อ้างอิง (Ref) ไปตาราง:** `ข้อมูลพนักงาน`

**ค่าเริ่มต้น (Initial Value):**

```
=LOOKUP(USEREMAIL(), "ข้อมูลพนักงาน", "Email พนักงาน", "ID_พนักงาน")
```

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
| นิยามคงที่ | No |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**ค่าเริ่มต้น (Initial Value):**

```
=HERE()
```

**Reset_If (เงื่อนไขรีเซ็ต):**

```
=ISNOTBLANK([หมายเหตุ])
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"RealTime": false, "PublishIfRowKey": null, "KMLFileUrl": null, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": "=ISNOTBLANK([หมายเหตุ])", "Suggested_Values": null}
```

</details>

### 30. เวลาเริ่มกรอกงาน

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Time |
| Key | No |
| Label | No |
| Virtual | No |
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

**ค่าเริ่มต้น (Initial Value):**

```
=TIMENOW()
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MinValue": null, "MaxValue": null, "IgnoreSeconds": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
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
| นิยามคงที่ | No |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**ค่าเริ่มต้น (Initial Value):**

```
=TIMENOW()
```

**Reset_If (เงื่อนไขรีเซ็ต):**

```
=ISNOTBLANK([หมายเหตุ])
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MinValue": null, "MaxValue": null, "IgnoreSeconds": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": "=ISNOTBLANK([หมายเหตุ])", "Suggested_Values": null}
```

</details>

### 32. ระยะขยับจากจุดเริ่มต้น_เมตร

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Decimal |
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
=DISTANCE( [จุดส่งสินค้าปลายทาง], [พิกัดตอนกดบันทึกงาน] ) * 1000
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxValue": null, "MinValue": null, "StepValue": null, "DecimalDigits": 2, "NumericDigits": null, "ShowThousandsSeparator": true, "NumberDisplayMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": "", "S uggested_Values": null}
```

</details>

### 33. ระยะเวลาใช้งาน_นาที

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Duration |
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
=[เวลาบันทึกงานสำเร็จ] - [เวลาที่ส่งสินค้า]
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"IgnoreSeconds": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 34. ความเร็วการเคลื่อนที่_เมตร_นาที

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Decimal |
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
=IF( TOTALMINUTES([ระยะเวลาใช้งาน_นาที]) > 0, [ระยะขยับจากจุดเริ่มต้น_เมตร] / TOTALMINUTES([ระยะเวลาใช้งาน_นาที]), 0 )
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxValue": null, "MinValue": null, "StepValue": null, "DecimalDigits": 2, "NumericDigits": null, "ShowThousandsSeparator": true, "NumberDisplayMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 35. ผลการตรวจสอบงานส่ง

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Enum |
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
=IFS( AND([ระยะขยับจากจุดเริ่มต้น_เมตร] <= 40, TOTALMINUTES([ระยะเวลาใช้งาน_นาที]) <= 10), "PASS", AND([ระยะขยับจากจุดเริ่มต้น_เมตร] <= 60, TOTALMINUTES([ระยะเวลาใช้งาน_นาที]) <= 15), "WARNING", OR([ระยะขยับจากจุดเริ่มต้น_เมตร] > 100, [ความเร็วการเคลื่อนที่_เมตร_นาที]> 60), "FAIL", TRUE, "WARNING" )
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"EnumValues": ["PASS", "WARNING", "FAIL"], "AllowOtherValues": false, "AutoCompleteOtherValues": true, "BaseType": "Text", "BaseTypeQualifier": " {\"MaxLength\":null,\"MinLength\":null,\"LongTextFormatting\":\"Plain Text\",\"IsMulticolumnKey\":false,\"Valid_If\":null,\"Error_Message_If_Invalid\":null,\"Show_If\":null,\"Required_If\":null,\"Editable_If\":null,\"Reset_If\":null,\"Suggested_Values\":null}", "EnumInputMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 36. เหตุผิดปกติที่ตรวจพบ

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
| นิยามคงที่ | No |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**App Formula (สูตรคำนวณ):**

```
=UNIQUE( LIST( IF([ระยะขยับจากจุดเริ่มต้น_เมตร] > 60, "มีการ เคลื่อนที่จากจุดเริ่มต้น", ""), IF(TOTALMINUTES([ระยะเวลาใช้งาน_นาที]) > 15, "ใช้เวลานานกว่าปกติ", ""), IF([ความเร็วการเคลื่อนที่_เมตร_นาที] > 60, "ความเร็วผิดปกติ", "") ) ) - LIST("")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"ItemSeparator": ",", "EnumValues": [], "AllowOtherValues": true, "AutoCompleteOtherValues": true, "BaseType": "Text", "BaseTypeQualifier": " {\"MaxLength\":null,\"MinLength\":null,\"LongTextFormatting\":\"Plain Text\",\"IsMulticolumnKey\":false,\"Valid_If\":null,\"Error_Message_If_Invalid\":null,\"Show_If\":null,\"Required_If\":null,\"Editable_If\":null,\"Reset_If\":null,\"Suggested_Values\":null}", "EnumInputMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 37. เวลาถ่ายรูปหน้าร้าน_หน้าบ้าน

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Time |
| Key | No |
| Label | No |
| Virtual | No |
| Read-Only | Yes |
| Hidden | No |
| รีเซ็ตเมื่อแก้ไข | Yes |
| คอลัมน์ระบบ | No |
| ส่วนหนึ่งของ Key | No |
| นิยามคงที่ | No |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**ค่าเริ่มต้น (Initial Value):**

```
=IF( ISNOTBLANK([รูปหน้าร้าน / บ้าน]), TIMENOW(), [_THIS] )
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MinValue": null, "MaxValue": null, "IgnoreSeconds": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 43. เจ้าของสินค้า//ชื่อปลายทาง//Lat_Long//Inv No

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | LongText |
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
=CONCATENATE( IF(ISNOTBLANK([ชื่อเจ้าของสินค้า]), CONCATENATE("ต้นทาง ", [ชื่อเจ้าของสินค้า], " "), ""), IF(ISNOTBLANK([ชื่อปลายทาง]), CONCATENATE("ปลายทาง ", [ชื่อปลายทาง], " "), ""), IF(ISNOTBLANK([จุดส่งสินค้าปลายทาง]), CONCATENATE("Lat/Lng ", TEXT([จุดส่งสินค้าปลายทาง]), " "), ""),IF(ISNOTBLANK([Invoice No]), CONCATENATE("INV. ", INDEX([Invoice No], 1)), "") )
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 44. Document_Return

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | LongText |
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
=[ID_Doc_Return].[ข้อความอธิบาย_Document_Return]
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 45. Image_Document_Return

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
=[ID_Doc_Return].[Related Image_Doc_Returns]
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"ElementType": "Ref", "ElementTypeQualifier": " {\"ReferencedTableName\":\"Image_Doc_Return\",\"ReferencedRootTableName\":\"Image_Doc_Return\",\"ReferencedType\":\"Text\",\"ReferencedTypeQualifier\":\" {\\\"MaxLength\\\":null,\\\"MinLength\\\":null,\\\"LongTextFor matting\\\":\\\"Plain Text\\\",\\\"IsMulticolumnKey\\\":false,\\\"Valid_If\\\":null,\\\"Error_Message_If_Invalid\\\":null,\\\"Show_If\\\":null,\\\"Required_If\\\":null,\\\"Editable_If\\\":null,\\\"Reset_If\\\":null,\\\"Suggested_Values\\\":null}\",\"ReferencedKeyColumn\":\"ID_Image_Doc_Return\",\"IsAPartOf\":false,\"RelationshipName\":null,\"InputMode\":\"Auto\",\"Valid_If\":null,\"Error_Message_If_Invalid\":null,\"Show_If\":null,\"Required_If\":null,\"Editable_If\":null,\"Reset_If\":null,\"Suggested_Values\":null}", "ItemSeparator": " , ", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 46. ที่อยู่ปลายทาง_LatLong_Api

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | LatLong |
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
=LOOKUP([_THISROW].[ชื่อปลายทาง],"ตารางงานประจำวัน","ชื่อ ปลายทาง","ที่อยู่ปลายทาง_LatLong")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"RealTime": false, "PublishIfRowKey": null, "KMLFileUrl": null, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 47. Related สรุปเบิกส่วนต่างs

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
REF_ROWS("สรุปเบิกส่วนต่าง", "_ComputedKey_ID_SCGนครหลวงJWDภูมิภาค")
```

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
REF_ROWS("ทำเบิกส่วนต่างScgวังน้อย", "ID_SCGนครหลวงJWDภูมิภาค")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"ElementType": "Ref", "ElementTypeQualifier": " {\"ReferencedTableName\":\"ทำเบิกส่วน ต่างScgวังน้อย\",\"ReferencedRootTableName\":\"ทำเบิกส่วน ต่างScgวังน้อย\",\"ReferencedType\":\"Text\",\"ReferencedTypeQualifier\":\" {\\\"MaxLength\\\":null,\\\"MinLength\\\":null,\\\"LongTextFor matting\\\":\\\"Plain Text\\\",\\\"IsMulticolumnKey\\\":false,\\\"Valid_If\\\":null,\\\"Error_Message_If_Invalid\\\":null,\\\"Show_If\\\":null,\\\"Required_If\\\":null,\\\"Editable_If\\\":null,\\\"Reset_If\\\":null,\\\"Suggested_Values\\\":null}\",\"ReferencedKeyColumn\":\"ID_ทำเบิกส่วนต่างScgวังน้อย\",\"IsAPartOf\":false,\"RelationshipName\":null,\"InputMode\":\"Auto\",\"Valid_If\":null,\"Error_Message_If_Invalid\":null,\"Show_If\":null,\"Required_If\":null,\"Editable_If\":null,\"Reset_If\":null,\"Suggested_Values\":null}", "ItemSeparator": " , ", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 49. พิกัดตอนกดบันทึก_เปลี่ยนแล้ว

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
| ข้อมูลอ่อนไหว | No Schema Name ข้อมูลการเข้าบำรุงรักษา_Schema |
| Locale | en-GB |

**App Formula (สูตรคำนวณ):**

```
=AND( ISNOTBLANK([พิกัดตอนกดบันทึกงาน]), [พิกัดตอนกดบันทึกงาน] <> [_THISROW_BEFORE].[พิกัดตอนกดบันทึกงาน] )
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"YesLabel": "", "NoLabel": "", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

## คอลัมน์ทั่วไป (ไม่มีสูตรหรือเงื่อนไขพิเศษ)

- **2. head** — ชนิด `LongText` (ค่าปกติ)
- **21. รูปสินค้าตอนส่ง** — ชนิด `Image` (ค่าปกติ)
- **22. รูปหน้าร้าน / บ้าน** — ชนิด `Image` (ค่าปกติ)
- **25. ระยะทางจากคลัง_Km** — ชนิด `Decimal` (ค่าปกติ)
- **26. ชื่อที่อยู่จาก_LatLong** — ชนิด `LongText` (ค่าปกติ)
- **38. SYNC_STATUS** — ชนิด `Text` (ค่าปกติ)
- **39. MD_LINK** — ชนิด `Text` (ค่าปกติ)
- **40. MATCH_KEY** — ชนิด `Text` (ค่าปกติ)
- **41. POINTS_AT_TIME** — ชนิด `Number` (ค่าปกติ)
- **42. STATUS** — ชนิด `Text` (ค่าปกติ)

