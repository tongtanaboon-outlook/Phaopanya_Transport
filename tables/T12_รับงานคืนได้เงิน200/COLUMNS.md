# คอลัมน์ของตาราง รับงานคืนได้เงิน200

รวม **29 คอลัมน์** (จาก Schema `รับงานคืนได้เงิน200_Schema`)

| # | ชื่อคอลัมน์ | ชนิด | สถานะ | สูตร/เงื่อนไข |
|---:|---|---|---|---|
| 1 | _RowNumber | Number | 🔒 🙈 ⚙️ |  |
| 2 | ID_รับงานคืนได้เงิน200 | Text | 🔑 🏷️ 🔒 | InitValue |
| 3 | สถานะการเข้ารับสินค้า | Enum |  |  |
| 4 | วันที่เข้ารับ | Date |  | InitValue, Editable_If |
| 5 | ชื่อ - นามสกุล | Text | 🔒 | InitValue |
| 6 | ทะเบียนรถ | Text | 🔒 | InitValue |
| 7 | Shipment (หลัก) | Number |  | Valid_If, Show_If |
| 8 | Shipment (รับคืน) | Number |  | AppFormula, Show_If |
| 9 | เลขที่เอกสารรับคืน | Text |  | Valid_If, Show_If |
| 10 | จำนวนสินค้า | Number |  | Show_If |
| 11 | Shipment No | Number |  | Valid_If, Show_If |
| 12 | Invoice No | EnumList |  | Valid_If, Show_If |
| 13 | ชื่อเจ้าของสินค้า | Text |  | AppFormula |
| 14 | รหัสลูกค้า | Text |  | AppFormula |
| 15 | ชื่อลูกค้าที่เข้ารับ | Text |  | AppFormula |
| 16 | รูปสินค้า | Image |  |  |
| 17 | รูปบิลรับคืน | Image |  |  |
| 18 | หมายเหตุ | LongText |  | Show_If |
| 19 | รูปจุดที่ส่งงาน | Image |  | Show_If |
| 20 | Lat / Long | LatLong |  | AppFormula |
| 21 | Email พนักงาน | Email |  | InitValue, Editable_If |
| 22 | ราคา | Price |  | InitValue, Editable_If, Show_If |
| 23 | สร้างPDFรับคืน | Yes/No |  | Editable_If, Show_If |
| 24 | TimeChange | ChangeCounter | 🙈 |  |
| 25 | ตรวจสอบก่อนบันทึกข้อมูล | Number |  | AppFormula, Valid_If |
| 26 | เดือน | Text | 🔒 | InitValue |
| 27 | ID_พนักงาน | Ref |  | InitValue, Editable_If, Show_If |
| 28 | LINK_IMAGE | Text | 🔒 🙈 | AppFormula |
| 29 | รายชื่อจุดส่งในตารางงานประจำวัน | LongText | 🔒 | AppFormula |

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

### 2. ID_รับงานคืนได้เงิน200

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

### 4. วันที่เข้ารับ

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
=USERROLE() = "ADMIN"
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"UseLongDateFormat": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": "=USERROLE() = \"ADMIN\"", "Reset_If": null, "Suggested_Values": null}
```

</details>

### 5. ชื่อ - นามสกุล

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

### 6. ทะเบียนรถ

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

### 7. Shipment (หลัก)

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
=IF(

USERROLE()= "ADMIN",
 SELECT(
 ข้อมูลงานRT[Shipment (หลัก)],
 TRUE
 ),
 SELECT(
 ข้อมูล งานRT[Shipment (หลัก)],
 AND(
 [ชื่อ - นามสกุล] =[_THISROW].[ID_พนักงาน].[ชื่อ - นามสกุล],
 [วันที่เข้ารับ] = TODAY()
 )
 )
)
```

**Show_If (เงื่อนไขการแสดง):**

```
=IN([สถานะการเข้ารับสินค้า],{"(ได้เพิ่ม200) ไม่มีในจุด ที่ส่งงานวันนี้","(ไม่ได้เพิ่ม) มีในจุดที่ ส่งงานวันนี้", "(ได้เพิ่ม50%) ของค่าเที่ยว","(ได้เพิ่ม200) ไม่มีสินค้าคืน หรือ ร้าน ปิด"})
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxValue": null, "MinValue": null, "StepValue": null, "NumericDigits": null, "ShowThousandsSeparator": false, "NumberDisplayMode": "Auto", "Valid_If": "=IF(\n\nUSERROLE()= \"ADMIN\",\n SELECT(\n ข้อมูลงานRT[Shipment (หลัก)],\n TRUE\n ),\n SELECT(\n ข้อมูล งานRT[Shipment (หลัก)],\n AND(\n [ชื่อ - นามสกุล] =[_THISROW].[ID_พนักงาน].[ชื่อ - นามสกุล],\n [วันที่เข้ารับ] = TODAY()\n )\n )\n)", "Error_Message_If_Invalid": null, "Show_If": "=IN([สถานะการเข้ารับสินค้า],{\"(ได้เพิ่ม200) ไม่มีในจุด ที่ส่งงานวันนี้\",\"(ไม่ได้เพิ่ม) มีในจุดที่ ส่งงานวันนี้\", \"(ได้เพิ่ม50%) ของค่าเที่ยว\",\"(ได้เพิ่ม200) ไม่มีสินค้าคืน หรือ ร้าน ปิด\"})", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 8. Shipment (รับคืน)

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

**App Formula (สูตรคำนวณ):**

```
=LOOKUP([_THISROW].[Shipment (หลัก)],"ข้อมูล งานRT","Shipment (หลัก)","Shipment (รับคืน)")
```

**Show_If (เงื่อนไขการแสดง):**

```
=IN([สถานะการเข้ารับสินค้า],{"(ได้เพิ่ม200) ไม่มีในจุด ที่ส่งงานวันนี้","(ไม่ได้เพิ่ม) มีในจุดที่ ส่งงานวันนี้", "(ได้เพิ่ม50%) ของค่าเที่ยว","(ได้ เพิ่ม200) ไม่มีสินค้าคืน หรือ ร้าน ปิด"})
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxValue": null, "MinValue": null, "StepValue": null, "NumericDigits": null, "ShowThousandsSeparator": false, "NumberDisplayMode": "Auto", "Valid_If": "", "Error_Message_If_Invalid": null, "Show_If": "=IN([สถานะการเข้ารับสินค้า],{\"(ได้เพิ่ม200) ไม่มีในจุด ที่ส่งงานวันนี้\",\"(ไม่ได้เพิ่ม) มีในจุดที่ ส่งงานวันนี้\", \"(ได้เพิ่ม50%) ของค่าเที่ยว\",\"(ได้ เพิ่ม200) ไม่มีสินค้าคืน หรือ ร้าน ปิด\"})", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 9. เลขที่เอกสารรับคืน

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
=IF( 
USERROLE() = "ADMIN",
 SELECT(
 ข้อมูลงานRT[เลขที่เอกสารรับคืน],
 IN([Shipment (รับคืน)], LIST([_THISROW].[Shipment (รับคืน)])) 
),

 SELECT(
 ข้อมูลงานRT[เลขที่เอกสารรับคืน],
 AND(
 IN([Shipment (รับคืน)], LIST([_THISROW].[Shipment (รับคืน)])),
[ชื่อ - นามสกุล] = [_THISROW].[ID_พนักงาน].[ชื่อ - นามสกุล],
 [วันที่เข้ารับ] = TODAY(),
 NOT(IN([เลขที่เอกสารรับคืน], SELECT(รับงานคืนได้เงิน200[เลขที่เอกสารรับคืน], TRUE)))
 )
 )
)
```

**Show_If (เงื่อนไขการแสดง):**

```
=IN([สถานะการเข้ารับสินค้า],{"(ได้เพิ่ม200) ไม่มีในจุด ที่ส่งงานวันนี้","(ไม่ได้เพิ่ม) มีในจุดที่ ส่งงานวันนี้", "(ได้เพิ่ม50%) ของค่าเที่ยว","(ได้เพิ่ม200) ไม่มีสินค้าคืน หรือ ร้าน ปิด"})
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": "=IF( \nUSERROLE() = \"ADMIN\",\n SELECT(\n ข้อมูลงานRT[เลขที่เอกสารรับคืน],\n IN([Shipment (รับคืน)], LIST([_THISROW].[Shipment (รับคืน)])) \n),\n\n SELECT(\n ข้อมูลงานRT[เลขที่เอกสารรับคืน],\n AND(\n IN([Shipment (รับคืน)], LIST([_THISROW].[Shipment (รับคืน)])),\n[ชื่อ - นามสกุล] = [_THISROW].[ID_พนักงาน].[ชื่อ - นามสกุล],\n [วันที่เข้ารับ] = TODAY(),\n NOT(IN([เลขที่เอกสารรับคืน], SELECT(รับงานคืนได้เงิน200[เลขที่เอกสารรับคืน], TRUE)))\n )\n )\n)", "Error_Message_If_Invalid": null, "Show_If": "=IN([สถานะการเข้ารับสินค้า],{\"(ได้เพิ่ม200) ไม่มีในจุด ที่ส่งงานวันนี้\",\"(ไม่ได้เพิ่ม) มีในจุดที่ ส่งงานวันนี้\", \"(ได้เพิ่ม50%) ของค่าเที่ยว\",\"(ได้เพิ่ม200) ไม่มีสินค้าคืน หรือ ร้าน ปิด\"})", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 10. จำนวนสินค้า

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

**Show_If (เงื่อนไขการแสดง):**

```
=IN([สถานะการเข้ารับสินค้า],{"(ได้เพิ่ม200) ไม่มีในจุด ที่ส่งงานวันนี้"," (ไม่ได้เพิ่ม) มีในจุดที่ ส่งงานวันนี้", "(ได้เพิ่ม50%) ของค่า เที่ยว","เบิกค่าขนส่งตามระยะทาง","ทำเบิกค่ายกขึ้น ชั้น"})
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxValue": null, "MinValue": null, "StepValue": null, "NumericDigits": null, "ShowThousandsSeparator": true, "NumberDisplayMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": "=IN([สถานะการเข้ารับสินค้า],{\"(ได้เพิ่ม200) ไม่มีในจุด ที่ส่งงานวันนี้\",\" (ไม่ได้เพิ่ม) มีในจุดที่ ส่งงานวันนี้\", \"(ได้เพิ่ม50%) ของค่า เที่ยว\",\"เบิกค่าขนส่งตามระยะทาง\",\"ทำเบิกค่ายกขึ้น ชั้น\"})", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 11. Shipment No

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
=SM_Today_User 2[Shipment No]
```

**Show_If (เงื่อนไขการแสดง):**

```
=IN([สถานะการเข้ารับสินค้า],{"เบิกค่าขนส่งตามระยะทาง","ทำเบิกค่ายกขึ้น ชั้น"})
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxValue": null, "MinValue": null, "StepValue": null, "NumericDigits": null, "ShowThousandsSeparator": false, "NumberDisplayMode": "Auto", "Valid_If": "=SM_Today_User 2[Shipment No]", "Error_Message_If_Invalid": null, "Show_If": "=IN([สถานะการเข้ารับสินค้า],{\"เบิกค่าขนส่งตามระยะทาง\",\"ทำเบิกค่ายกขึ้น ชั้น\"})", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 12. Invoice No

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
=IF(
 ISBLANK([Shipment No]),
 LIST(),
 UNIQUE(
 SELECT(
 SM_Today_User 2[Invoice No],
 AND(
 [Shipment No] = [_THISROW]. [Shipment No],
 NOT(
 IN(
 [Invoice No],
 รับงานคืนได้ เงิน200[Invoice No]
 )
 )
 )
 )
 + [_THISROW].[Invoice No]
 )
 -LIST("")
)
```

**Show_If (เงื่อนไขการแสดง):**

```
=IN([สถานะการเข้ารับสินค้า],{"เบิกค่าขนส่งตามระยะทาง","ทำเบิกค่ายก ขึ้น ชั้น"})
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"ItemSeparator": ",", "EnumValues": [], "AllowOtherValues": true, "AutoCompleteOtherValues": true, "BaseType": "Text", "BaseTypeQualifier": " {\"MaxLength\":null,\"MinLength\":null,\"LongTextFormatting\":\"Plain Text\",\"IsMulticolumnKey\":false,\"Valid_If\":null,\"Error_Message_If_Invalid\":null,\"Show_If\":null,\"Required_If\":null,\"Editable_If\":null,\"Reset_If\":null,\"Suggested_Values\":null}", "EnumInputMode": "Dropdown", "Valid_If": "=IF(\n ISBLANK([Shipment No]),\n LIST(),\n UNIQUE(\n SELECT(\n SM_Today_User 2[Invoice No],\n AND(\n [Shipment No] = [_THISROW]. [Shipment No],\n NOT(\n IN(\n [Invoice No],\n รับงานคืนได้ เงิน200[Invoice No]\n )\n )\n )\n )\n + [_THISROW].[Invoice No]\n )\n -LIST(\"\")\n)", "Error_Message_If_Invalid": null, "Show_If": "=IN([สถานะการเข้ารับสินค้า],{\"เบิกค่าขนส่งตามระยะทาง\",\"ทำเบิกค่ายก ขึ้น ชั้น\"})", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
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
=IF( IN([สถานะการเข้ารับสินค้า],{"เบิกค่าขนส่งตามระยะทาง","ทำ เบิกค่ายกขึ้นชั้น"}), LOOKUP(ANY([_THISROW].[Invoice No]), "ตารางงานประจำวัน", "Invoice No", "ชื่อเจ้าของสินค้า"), LOOKUP([_THISROW].[รหัสลูกค้า],"DOC_RETURN","รหัสลูกค้า","ชื่อเจ้าของสินค้า") )
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 14. รหัสลูกค้า

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

**App Formula (สูตรคำนวณ):**

```
=IF( IN([สถานะการเข้ารับสินค้า],{"เบิกค่าขนส่งตามระยะทาง","ทำ เบิกค่ายกขึ้นชั้น"}), LOOKUP(ANY([_THISROW].[Invoice No]), "ตารางงานประจำวัน", "Invoice No", "รหัสลูกค้า"), LOOKUP([_THISROW].[เลขที่เอกสารรับคืน], "ข้อมูลงานRT", "เลขที่ เอกสารรับคืน", "รหัสลูกค้า") )
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 15. ชื่อลูกค้าที่เข้ารับ

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

**App Formula (สูตรคำนวณ):**

```
=IF( IN([สถานะการเข้ารับสินค้า],{"เบิกค่าขนส่งตามระยะทาง","ทำ เบิกค่ายกขึ้นชั้น"}), LOOKUP(ANY([_THISROW].[Invoice No]), "ตารางงานประจำวัน", "Invoice No", "ชื่อปลายทาง"), LOOKUP([_THISROW].[เลขที่เอกสารรับคืน],"ข้อมูลงานRT","เลขที่ เอกสารรับคืน","ชื่อลูกค้าที่เข้ารับ") )
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": "", "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 18. หมายเหตุ

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
=IN([สถานะการเข้ารับสินค้า],{"ทำเบิกค่ายกขึ้นชั้น","เบิกค่าขนส่งตามระยะทาง","(ได้เพิ่ม200) ไม่มีสินค้าคืน หรือ ร้าน ปิด"})
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": "=IN([สถานะการเข้ารับสินค้า],{\"ทำเบิกค่ายกขึ้นชั้น\",\"เบิกค่าขนส่งตามระยะทาง\",\"(ได้เพิ่ม200) ไม่มีสินค้าคืน หรือ ร้าน ปิด\"})", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 19. รูปจุดที่ส่งงาน

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=IN([สถานะการเข้ารับสินค้า] ,{"(ได้เพิ่ม200) ไม่มีสินค้าคืน หรือ ร้านปิด","(ได้เพิ่ม50%) ของค่า เที่ยว","(ได้เพิ่ม200) ไม่มีในจุด ที่ส่งงานวันนี้","เบิกค่าขนส่งตาม ระยะทาง","ทำเบิกค่ายกขึ้น ชั้น"})
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": "=IN([สถานะการเข้ารับสินค้า] ,{\"(ได้เพิ่ม200) ไม่มีสินค้าคืน หรือ ร้านปิด\",\"(ได้เพิ่ม50%) ของค่า เที่ยว\",\"(ได้เพิ่ม200) ไม่มีในจุด ที่ส่งงานวันนี้\",\"เบิกค่าขนส่งตาม ระยะทาง\",\"ทำเบิกค่ายกขึ้น ชั้น\"})", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 20. Lat / Long

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

**App Formula (สูตรคำนวณ):**

```
=HERE()
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"RealTime": false, "PublishIfRowKey": null, "KMLFileUrl": null, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 21. Email พนักงาน

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

### 22. ราคา

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

**ค่าเริ่มต้น (Initial Value):**

```
=IFS( OR( [สถานะการเข้ารับสินค้า] = "(ได้เพิ่ม200) ไม่มีในจุด ที่ส่ง งานวันนี้", [สถานะการเข้ารับสินค้า] = "(ได้เพิ่ม200) ไม่มีสินค้าคืน หรือร้านปิด" ), 200, [สถานะการเข้ารับสินค้า] = "(ไม่ได้เพิ่ม) มีในจุดที่ ส่ง งานวันนี้", 0, [สถานะการเข้ารับสินค้า] = "(ได้เพิ่ม50%) ของค่าเที่ยว", LOOKUP( [Shipment (หลัก)], "ราคาในระบบก่อนส่งสินค้า", "Shipment No", "ราคา" ) * 0.50, [สถานะการเข้ารับสินค้า] = "(ทำเบิกค่ายกขึ้นชั้น)", "" )
```

**Editable_If (เงื่อนไขที่แก้ไขได้):**

```
=USERROLE() = "ADMIN"
```

**Show_If (เงื่อนไขการแสดง):**

```
=IN([สถานะการเข้ารับสินค้า] ,{"(ได้เพิ่ม200) ไม่มีสินค้าคืน หรือ ร้านปิด","(ได้เพิ่ม50%) ของค่า เที่ยว","(ได้เพิ่ม200) ไม่มีในจุด ที่ส่งงานวันนี้","เบิกค่าขนส่งตาม ระยะทาง","ทำเบิกค่ายกขึ้น ชั้น"})
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"CurrencySymbol": "฿", "MaxValue": null, "MinValue": null, "StepValue": null, "DecimalDigits": 2, "NumericDigits": null, "ShowThousandsSeparator": true, "NumberDisplayMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": "=IN([สถานะการเข้ารับสินค้า] ,{\"(ได้เพิ่ม200) ไม่มีสินค้าคืน หรือ ร้านปิด\",\"(ได้เพิ่ม50%) ของค่า เที่ยว\",\"(ได้เพิ่ม200) ไม่มีในจุด ที่ส่งงานวันนี้\",\"เบิกค่าขนส่งตาม ระยะทาง\",\"ทำเบิกค่ายกขึ้น ชั้น\"})", "Required_If": null, "Editable_If": "=USERROLE() = \"ADMIN\"", "Reset_If": null, "Suggested_Values": null}
```

</details>

### 23. สร้างPDFรับคืน

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

**Editable_If (เงื่อนไขที่แก้ไขได้):**

```
=USERROLE() = "ADMIN"
```

**Show_If (เงื่อนไขการแสดง):**

```
=USERROLE() = "ADMIN"
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"YesLabel": "", "NoLabel": "", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": "=USERROLE() = \"ADMIN\"", "Required_If": null, "Editable_If": "=USERROLE() = \"ADMIN\"", "Reset_If": null, "Suggested_Values": null}
```

</details>

### 25. ตรวจสอบก่อนบันทึกข้อมูล

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

**App Formula (สูตรคำนวณ):**

```
=IF( IN([สถานะการเข้ารับสินค้า],{"เบิกค่าขนส่งตามระยะทาง","ทำ เบิกค่ายกขึ้นชั้น"}), 1, IF( COUNT( SELECT( ข้อมูลงานRT[เลขที่เอกสารรับคืน], AND( [วันที่เข้ารับ] = [_THISROW].[วันที่เข้ารับ], [ชื่อ - นามสกุล] = [_THISROW].[ชื่อ - นามสกุล], [Shipment (หลัก)] = [_THISROW].[Shipment (หลัก)], [Shipment (รับคืน)] = [_THISROW].[Shipment (รับคืน)], [เลขที่เอกสารรับคืน] = [_THISROW].[เลขที่เอกสารรับคืน] ) ) ) > 0, 1, 0 ) )
```

**Valid_If (เงื่อนไขความถูกต้อง):**

```
=[ตรวจสอบก่อนบันทึกข้อมูล] >0
```

**ข้อความเตือนเมื่อค่าไม่ถูกต้อง:**

```
=บันทึกข้อมูลไม่สำเร็จ กรุณา ติดต่อแอดมินเพื่อตรวจ สอบ
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxValue": null, "MinValue": null, "StepValue": null, "NumericDigits": null, "ShowThousandsSeparator": true, "NumberDisplayMode": "Auto", "Valid_If": "=[ตรวจสอบก่อนบันทึกข้อมูล] >0", "Error_Message_If_Invalid": "=บันทึกข้อมูลไม่สำเร็จ กรุณา ติดต่อแอดมินเพื่อตรวจ สอบ", "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 26. เดือน

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
=IF( ISBLANK([วันที่เข้ารับ]), "", CONCATENATE( YEAR([วันที่เข้ารับ]) - IF(YEAR([วันที่เข้ารับ]) > 2500, 543, 0), "-", TEXT([วันที่เข้ารับ],"MM") ) )
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 27. ID_พนักงาน

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

### 28. LINK_IMAGE

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Text |
| Key | No |
| Label | No |
| Virtual | Yes |
| Read-Only | Yes |
| Hidden | Yes |
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
=TEXT( LIST( IF(ISNOTBLANK([รูปสินค้า]), CONCATENATE( "https://www.appsheet.com/template/gettablefileurl?", "appName=", ENCODEURL("เผ่าปัญญาทรานสปอร์ต-915154893"),"&appId=", ENCODEURL("70999aca-5a1f-4dfc-907b-417bc046f574"), "&tableName=", ENCODEURL("รับงานคืนได้ เงิน200"), "&fileName=", ENCODEURL([รูปสินค้า]) ), ""), IF(ISNOTBLANK([รูปบิลรับคืน]), CONCATENATE( "https://www.appsheet.com/template/gettablefileurl?", "appName=", ENCODEURL("เผ่าปัญญาทรานสปอร์ต-915154893"),"&appId=", ENCODEURL("70999aca-5a1f-4dfc-907b-417bc046f574"), "&tableName=", ENCODEURL("รับงานคืนได้ เงิน200"), "&fileName=", ENCODEURL([รูปบิลรับคืน]) ), ""), IF(ISNOTBLANK([รูปจุดที่ส่งงาน]), CONCATENATE( "https://www.appsheet.com/template/gettablefileurl?", "appName=", ENCODEURL("เผ่าปัญญาทรานสปอร์ต-915154893"),"&appId=", ENCODEURL("70999aca-5a1f-4dfc-907b-417bc046f574"), "&tableName=", ENCODEURL("รับงานคืนได้ เงิน200"), "&fileName=", ENCODEURL([รูปจุดที่ส่งงาน]) ), "") ) )
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 29. รายชื่อจุดส่งในตารางงานประจำวัน

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
| ข้อมูลอ่อนไหว | No Schema Name ข้อมูลงานRT_Schema |
| Locale | en-GB |

**App Formula (สูตรคำนวณ):**

```
=SUBSTITUTE( ANY( SELECT( ตารางงานประจำวัน[รายชื่อปลายทาง_System], [Shipment No] = IF(ISNOTBLANK([_THISROW]. [Shipment (หลัก)]), [_THISROW].[Shipment (หลัก)], [_THISROW].[Shipment No]) ) ), ", ", " " )
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

## คอลัมน์ทั่วไป (ไม่มีสูตรหรือเงื่อนไขพิเศษ)

- **3. สถานะการเข้ารับสินค้า** — ชนิด `Enum` (ค่าปกติ)
- **16. รูปสินค้า** — ชนิด `Image` (ค่าปกติ)
- **17. รูปบิลรับคืน** — ชนิด `Image` (ค่าปกติ)
- **24. TimeChange** — ชนิด `ChangeCounter` (Hidden=Yes)

