# คอลัมน์ของตาราง แจ้งปัญหาระหว่างวัน

รวม **29 คอลัมน์** (จาก Schema `แจ้งปัญหาระหว่างวัน_Schema`)

| # | ชื่อคอลัมน์ | ชนิด | สถานะ | สูตร/เงื่อนไข |
|---:|---|---|---|---|
| 1 | _RowNumber | Number | 🔒 🙈 ⚙️ |  |
| 2 | ID_แจ้งปัญหาระหว่างวัน | Text | 🔑 🏷️ | InitValue |
| 3 | กดปุ่มนี้เพื่อส่งข้อมูลแจ้งปัญหา | Yes/No |  | InitValue, Valid_If, Show_If |
| 4 | ข้อมูลการแจ้งปัญหา | Enum |  |  |
| 5 | รูป1 | Image |  |  |
| 6 | รูป2 | Image |  |  |
| 7 | รูป3 | Image |  |  |
| 8 | หมายเหตุ | LongText |  |  |
| 9 | วันที่+เวลา | DateTime |  | InitValue, Editable_If |
| 10 | ชื่อ - นามสกุล | Text | 🔒 | InitValue |
| 11 | ทะเบียนรถ | Text | 🔒 | InitValue |
| 12 | รหัสผู้รับเหมา | Text | 🔒 | InitValue, Show_If |
| 13 | ชื่อผู้รับเหมา | Text | 🔒 | InitValue, Show_If |
| 14 | Shipment No | Number |  | Valid_If |
| 15 | Invoice No | EnumList |  | Valid_If |
| 16 | รหัสลูกค้า | Text | 🔒 | InitValue, Show_If |
| 17 | ชื่อปลายทาง | Text | 🔒 | InitValue, Show_If |
| 18 | ใส่ข้อมูลการแจ้งปัญหา เพื่อนับจุดส่งงาน | LongText |  | Show_If |
| 19 | เพิ่มรูปแคปหน้าจอ นำกลับคืนคลัง | Image |  |  |
| 20 | อัพเดตข้อมูลการแจ้งปัญหา ไป ตารางส่งงานSCG | Yes/No |  | InitValue, Valid_If, Show_If |
| 21 | Lat/Long | LatLong | 🔒 | InitValue |
| 22 | LatLong_ตรวจสอบ | LatLong |  | InitValue, Reset_If |
| 23 | Email พนักงาน | Email |  | InitValue, Editable_If |
| 24 | เดือน | Text | 🔒 | InitValue |
| 25 | SM_Link | Ref | 🔒 | InitValue |
| 26 | RT_Link | Ref | 🔒 | InitValue |
| 27 | SCGนครหลวงJWDภูมิภาค_ID | Text |  |  |
| 28 | ID_พนักงาน | Ref |  | InitValue, Editable_If, Show_If |
| 29 | LINK_Image_แจ้งปัญหา | Text | 🔒 | AppFormula |

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

### 2. ID_แจ้งปัญหาระหว่างวัน

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

### 3. กดปุ่มนี้เพื่อส่งข้อมูลแจ้งปัญหา

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Yes/No |
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
=false
```

**Valid_If (เงื่อนไขความถูกต้อง):**

```
=OR(
 ISBLANK([กดปุ่มนี้เพื่อส่งข้อมูลแจ้งปัญหา]),
 NOT([กดปุ่มนี้เพื่อส่งข้อมูลแจ้งปัญหา])
)
```

**Show_If (เงื่อนไขการแสดง):**

```
=AND(
 ISNOTBLANK([รูป1]),
 ISNOTBLANK([รูป2]),
 ISNOTBLANK([รูป3]),
 NOT([กดปุ่มนี้เพื่อส่งข้อมูลแจ้งปัญหา])
)
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"YesLabel": "", "NoLabel": "", "Valid_If": "=OR(\n ISBLANK([กดปุ่มนี้เพื่อส่งข้อมูลแจ้งปัญหา]),\n NOT([กดปุ่มนี้เพื่อส่งข้อมูลแจ้งปัญหา])\n)", "Error_Message_If_Invalid": null, "Show_If": "=AND(\n ISNOTBLANK([รูป1]),\n ISNOTBLANK([รูป2]),\n ISNOTBLANK([รูป3]),\n NOT([กดปุ่มนี้เพื่อส่งข้อมูลแจ้งปัญหา])\n)", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 9. วันที่+เวลา

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | DateTime |
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
=NOW()
```

**Editable_If (เงื่อนไขที่แก้ไขได้):**

```
=USERROLE() = "ADMIN"
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MinValue": null, "MaxValue": null, "UseLongDateFormat": false, "IgnoreSeconds": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": "=USERROLE() = \"ADMIN\"", "Reset_If": null, "Suggested_Values": null}
```

</details>

### 10. ชื่อ - นามสกุล

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

### 11. ทะเบียนรถ

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

### 12. รหัสผู้รับเหมา

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
=[SM_Link].[รหัสผู้รับเหมา]
```

**Show_If (เงื่อนไขการแสดง):**

```
=ISNOTBLANK([Invoice No])
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": "=ISNOTBLANK([Invoice No])", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 13. ชื่อผู้รับเหมา

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
=[SM_Link].[ชื่อผู้รับเหมา]
```

**Show_If (เงื่อนไขการแสดง):**

```
=ISNOTBLANK([Invoice No])
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": "=ISNOTBLANK([Invoice No])", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 14. Shipment No

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
=IF(USERROLE() = "ADMIN",
 (SM_Today_User[Shipment No] + 
 SELECT(ข้อมูล งานRT[Shipment (รับคืน)], [วันที่เข้ารับ] = TODAY())),
 IF([ข้อมูลการแจ้งปัญหา] = "ไม่มีในจุดส่งงานวันนี้ ไม่สามารถเข้ารับงานคืนให้ ได้",
 SELECT(ข้อมูลงานRT[Shipment (รับคืน)], 
 AND([Email พนักงาน] = USEREMAIL(), [วันที่เข้ารับ] = TODAY())
 ),
 SM_Today_User[Shipment No]
 )
)
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxValue": null, "MinValue": null, "StepValue": null, "NumericDigits": null, "ShowThousandsSeparator": false, "NumberDisplayMode": "Auto", "Valid_If": "=IF(USERROLE() = \"ADMIN\",\n (SM_Today_User[Shipment No] + \n SELECT(ข้อมูล งานRT[Shipment (รับคืน)], [วันที่เข้ารับ] = TODAY())),\n IF([ข้อมูลการแจ้งปัญหา] = \"ไม่มีในจุดส่งงานวันนี้ ไม่สามารถเข้ารับงานคืนให้ ได้\",\n SELECT(ข้อมูลงานRT[Shipment (รับคืน)], \n AND([Email พนักงาน] = USEREMAIL(), [วันที่เข้ารับ] = TODAY())\n ),\n SM_Today_User[Shipment No]\n )\n)", "Error_Message_If_Invalid": null, "Show_If": "", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 15. Invoice No

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
=UNIQUE(
 IF(USERROLE() = "ADMIN",
 SELECT(ตารางงานประจำวัน[Invoice No], [ShipmentNo] = [_THISROW].[Shipment No]) +
 SELECT(ข้อมูลงานRT[เลขที่เอกสารรับคืน], [Shipment (รับคืน)] = [_THISROW].[Shipment No]),
 IF([ข้อมูลการแจ้งปัญหา] = "ไม่มีในจุดส่งงานวันนี้ ไม่ สามารถเข้ารับงานคืนให้ได้",
 SELECT(ข้อมูลงานRT[เลขที่เอกสารรับคืน],
 AND(
 [Shipment (รับคืน)] = [_THISROW].[Shipment No],
 [Email พนักงาน] = USEREMAIL(),
 [วันที่เข้ารับ] = TODAY()
 )
 ),
 SELECT(SM_Today_User[Invoice No], 
 AND(
 [Shipment No] = [_THISROW].[Shipment No],
 [DeliveryStatus] <> "จัดส่งเรียบร้อย",
 NOT(IN([Invoice No], SELECT(แจ้งปัญหาระหว่างวัน[Invoice No], [Shipment No] = [_THISROW].[Shipment No])))
 )
 )
 )
 ) 
 + [_THISROW]. [Invoice No]
) -LIST("")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"ItemSeparator": ",", "EnumValues": [], "AllowOtherValues": true, "AutoCompleteOtherValues": true, "BaseType": "Text", "BaseTypeQualifier": " {\"MaxLength\":null,\"MinLength\":null,\"LongTextFormatting\":\"Plain Text\",\"IsMulticolumnKey\":false,\"Valid_If\":null,\"Error_Message_If_Invalid\":null,\"Show_If\":null,\"Required_If\":null,\"Editable_If\":null,\"Reset_If\":null,\"Suggested_Values\":null}", "EnumInputMode": "Dropdown", "Valid_If": "=UNIQUE(\n IF(USERROLE() = \"ADMIN\",\n SELECT(ตารางงานประจำวัน[Invoice No], [ShipmentNo] = [_THISROW].[Shipment No]) +\n SELECT(ข้อมูลงานRT[เลขที่เอกสารรับคืน], [Shipment (รับคืน)] = [_THISROW].[Shipment No]),\n IF([ข้อมูลการแจ้งปัญหา] = \"ไม่มีในจุดส่งงานวันนี้ ไม่ สามารถเข้ารับงานคืนให้ได้\",\n SELECT(ข้อมูลงานRT[เลขที่เอกสารรับคืน],\n AND(\n [Shipment (รับคืน)] = [_THISROW].[Shipment No],\n [Email พนักงาน] = USEREMAIL(),\n [วันที่เข้ารับ] = TODAY()\n )\n ),\n SELECT(SM_Today_User[Invoice No], \n AND(\n [Shipment No] = [_THISROW].[Shipment No],\n [DeliveryStatus] <> \"จัดส่งเรียบร้อย\",\n NOT(IN([Invoice No], SELECT(แจ้งปัญหาระหว่างวัน[Invoice No], [Shipment No] = [_THISROW].[Shipment No])))\n )\n )\n )\n ) \n + [_THISROW]. [Invoice No]\n) -LIST(\"\")", "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": ""}
```

</details>

### 16. รหัสลูกค้า

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
=IF(ISNOTBLANK([SM_Link]), [SM_Link].[รหัสลูกค้า], IF(ISNOTBLANK([RT_Link]), [RT_Link].[รหัสลูกค้า], "ไม่พบข้อมูล" ))
```

**Show_If (เงื่อนไขการแสดง):**

```
=ISNOTBLANK([Invoice No])
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": "=ISNOTBLANK([Invoice No])", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 17. ชื่อปลายทาง

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
=IF(ISNOTBLANK([SM_Link]), [SM_Link].[ชื่อปลายทาง], IF(ISNOTBLANK([RT_Link]), [RT_Link].[ชื่อลูกค้าที่เข้ารับ], "ไม่พบ ข้อมูล" ) )
```

**Show_If (เงื่อนไขการแสดง):**

```
=ISNOTBLANK([Invoice No])
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": "=ISNOTBLANK([Invoice No])", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 18. ใส่ข้อมูลการแจ้งปัญหา เพื่อนับจุดส่งงาน

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
=ISNOTBLANK([เพิ่มรูปแคปหน้าจอ นำกลับ คืน คลัง])
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": "=ISNOTBLANK([เพิ่มรูปแคปหน้าจอ นำกลับ คืน คลัง])", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 20. อัพเดตข้อมูลการแจ้งปัญหา ไป ตารางส่งงานSCG

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Yes/No |
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
=false
```

**Valid_If (เงื่อนไขความถูกต้อง):**

```
=OR(
 ISBLANK([อัพเดตข้อมูลการแจ้งปัญหา ไป ตารางส่งงานSCG]),
 NOT([อัพเดตข้อมูล การแจ้งปัญหา ไป ตารางส่ง งานSCG])
)
```

**Show_If (เงื่อนไขการแสดง):**

```
=AND(
 ISNOTBLANK([ใส่ข้อมูลการแจ้งปัญหา เพื่อนับจุดส่งงาน]),
 ISNOTBLANK([เพิ่มรูปแคปหน้าจอ นำกลับคืนคลัง]),
 NOT([อัพเดตข้อมูลการแจ้งปัญหา ไป ตารางส่งงานSCG])
)
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"YesLabel": "", "NoLabel": "", "Valid_If": "=OR(\n ISBLANK([อัพเดตข้อมูลการแจ้งปัญหา ไป ตารางส่งงานSCG]),\n NOT([อัพเดตข้อมูล การแจ้งปัญหา ไป ตารางส่ง งานSCG])\n)", "Error_Message_If_Invalid": "", "Show_If": "=AND(\n ISNOTBLANK([ใส่ข้อมูลการแจ้งปัญหา เพื่อนับจุดส่งงาน]),\n ISNOTBLANK([เพิ่มรูปแคปหน้าจอ นำกลับคืนคลัง]),\n NOT([อัพเดตข้อมูลการแจ้งปัญหา ไป ตารางส่งงานSCG])\n)", "Required_If": null, "Editable_If": "", "Reset_If": null, "Suggested_Values": null}
```

</details>

### 21. Lat/Long

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
| ค้นหาได้ | No |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**ค่าเริ่มต้น (Initial Value):**

```
=HERE()
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"RealTime": false, "PublishIfRowKey": null, "KMLFileUrl": null, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 22. LatLong_ตรวจสอบ

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | LatLong |
| Key | No |
| Label | No |
| Virtual | No |
| Read-Only | No |
| Hidden | No |
| รีเซ็ตเมื่อแก้ไข | =ISNOTBLANK([เพิ่มรูปแคปหน้าจอ นำกลับคืนคลัง]) |
| คอลัมน์ระบบ | No |
| ส่วนหนึ่งของ Key | No |
| นิยามคงที่ | No |
| ค้นหาได้ | No |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**ค่าเริ่มต้น (Initial Value):**

```
=HERE()
```

**Reset_If (เงื่อนไขรีเซ็ต):**

```
=ISNOTBLANK([เพิ่มรูปแคปหน้าจอ นำกลับคืนคลัง])
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"RealTime": false, "PublishIfRowKey": null, "KMLFileUrl": null, "Valid_If": "", "Error_Message_If_Invalid": "", "Show_If": "", "Required_If": null, "Editable_If": null, "Reset_If": "=ISNOTBLANK([เพิ่มรูปแคปหน้าจอ นำกลับคืนคลัง])", "Suggested_Values": null}
```

</details>

### 23. Email พนักงาน

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
=USERROLE() = "ADMIN"
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": "=USERROLE() = \"ADMIN\"", "Reset_If": null, "Suggested_Values": null}
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
=IF( ISBLANK([วันที่+เวลา]), "", (YEAR(DATE([วันที่+เวลา])) -IF(YEAR(DATE([วันที่+เวลา])) > 2500, 543, 0)) & "-" & TEXT(DATE([วันที่+เวลา]), "MM") )
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 25. SM_Link

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Ref |
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

### 26. RT_Link

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Ref |
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

- 🔗 **อ้างอิง (Ref) ไปตาราง:** `ข้อมูลงานRT`

**ค่าเริ่มต้น (Initial Value):**

```
=ANY(SELECT(ข้อมูลงานRT[ID_RT], [เลขที่เอกสารรับคืน] = ANY([_THISROW].[Invoice No])))
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"ReferencedTableName": "ข้อมูลงานRT", "ReferencedRootTableName": "ข้อมูลงานRT", "ReferencedType": "Text", "ReferencedTypeQualifier": " {\"MaxLength\":null,\"MinLength\":null,\"LongTextFormatting\":\"Plain Text\",\"IsMulticolumnKey\":false,\"Valid_If\":null,\"Error_Message_If_Invalid\":null,\"Show_If\":null,\"Required_If\":null,\"Editable_If\":null,\"Reset_If\":null,\"Suggested_Values\":null}", "ReferencedKeyColumn": "ID_RT", "IsAPartOf": false, "RelationshipName": null, "InputMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
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
=USERROLE() = "ADMIN"
```

**Show_If (เงื่อนไขการแสดง):**

```
=USERROLE()= "ADMIN"
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"ReferencedTableName": "ข้อมูลพนักงาน", "ReferencedRootTableName": "ข้อมูลพนักงาน", "ReferencedType": "Text", "ReferencedTypeQualifier": " {\"MaxLength\":null,\"MinLength\":null,\"LongTextFormatting\":\"Plain Text\",\"IsMulticolumnKey\":false,\"Valid_If\":null,\"Error_Message_If_Invalid\":null,\"Show_If\":null,\"Required_If\":null,\"Editable_If\":null,\"Reset_If\":null,\"Suggested_Values\":null}", "ReferencedKeyColumn": "ID_พนักงาน", "IsAPartOf": false, "RelationshipName": null, "InputMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": "=USERROLE()= \"ADMIN\"", "Required_If": null, "Editable_If": "=USERROLE() = \"ADMIN\"", "Reset_If": null, "Suggested_Values": null}
```

</details>

### 29. LINK_Image_แจ้งปัญหา

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
| ข้อมูลอ่อนไหว | No Schema Name รับงานคืนได้เงิน200_Schema |
| Locale | en-GB |

**App Formula (สูตรคำนวณ):**

```
=TEXT( LIST( IF(ISNOTBLANK([รูป1]), CONCATENATE( "https://www.appsheet.com/template/gettablefileurl?", "appName=", ENCODEURL("เผ่าปัญญาทรานสปอร์ต-915154893"),"&appId=", ENCODEURL("70999aca-5a1f-4dfc-907b-417bc046f574"), "&tableName=", ENCODEURL("แจ้งปัญหา ระหว่างวัน"), "&fileName=", ENCODEURL([รูป1]) ), ""), IF(ISNOTBLANK([รูป2]), CONCATENATE( "https://www.appsheet.com/template/gettablefileurl?", "appName=", ENCODEURL("เผ่าปัญญาทรานสปอร์ต-915154893"),"&appId=", ENCODEURL("70999aca-5a1f-4dfc-907b-417bc046f574"), "&tableName=", ENCODEURL("แจ้งปัญหา ระหว่างวัน"), "&fileName=", ENCODEURL([รูป2]) ), ""), IF(ISNOTBLANK([รูป3]), CONCATENATE( "https://www.appsheet.com/template/gettablefileurl?", "appName=", ENCODEURL("เผ่าปัญญาทรานสปอร์ต-915154893"),"&appId=", ENCODEURL("70999aca-5a1f-4dfc-907b-417bc046f574"), "&tableName=", ENCODEURL("แจ้งปัญหา ระหว่างวัน"), "&fileName=", ENCODEURL([รูป3]) ), "") ) )
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

## คอลัมน์ทั่วไป (ไม่มีสูตรหรือเงื่อนไขพิเศษ)

- **4. ข้อมูลการแจ้งปัญหา** — ชนิด `Enum` (ค่าปกติ)
- **5. รูป1** — ชนิด `Image` (ค่าปกติ)
- **6. รูป2** — ชนิด `Image` (ค่าปกติ)
- **7. รูป3** — ชนิด `Image` (ค่าปกติ)
- **8. หมายเหตุ** — ชนิด `LongText` (ค่าปกติ)
- **19. เพิ่มรูปแคปหน้าจอ นำกลับคืนคลัง** — ชนิด `Image` (ค่าปกติ)
- **27. SCGนครหลวงJWDภูมิภาค_ID** — ชนิด `Text` (ค่าปกติ)

