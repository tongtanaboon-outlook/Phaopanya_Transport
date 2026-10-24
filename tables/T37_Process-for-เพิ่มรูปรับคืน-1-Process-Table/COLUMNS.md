# คอลัมน์ของตาราง Process for เพิ่มรูปรับคืน - 1 Process Table

รวม **30 คอลัมน์** (จาก Schema `Process for เพิ่มรูปรับคืน - 1 Process Table_Schema`)

| # | ชื่อคอลัมน์ | ชนิด | สถานะ | สูตร/เงื่อนไข |
|---:|---|---|---|---|
| 1 | Instance Id | Text | 🔑 |  |
| 2 | ID_รับงานคืนได้เงิน200 | Text |  |  |
| 3 | สถานะการเข้ารับสินค้า | Enum |  |  |
| 4 | วันที่เข้ารับ | Date |  | Editable_If |
| 5 | ชื่อ - นามสกุล | Text |  |  |
| 6 | ทะเบียนรถ | Text |  |  |
| 7 | Shipment (หลัก) | Number |  | Valid_If, Show_If |
| 8 | Shipment (รับคืน) | Number |  | Show_If |
| 9 | เลขที่เอกสารรับคืน | Text |  | Valid_If, Show_If |
| 10 | จำนวนสินค้า | Number |  | Show_If |
| 11 | Shipment No | Number |  | Valid_If, Show_If |
| 12 | Invoice No | EnumList |  | Valid_If, Show_If |
| 13 | ชื่อเจ้าของสินค้า | Text |  |  |
| 14 | รหัสลูกค้า | Text |  |  |
| 15 | ชื่อลูกค้าที่เข้ารับ | Text |  |  |
| 16 | รูปสินค้า | Image |  |  |
| 17 | รูปบิลรับคืน | Image |  |  |
| 18 | หมายเหตุ | LongText |  | Show_If |
| 19 | รูปจุดที่ส่งงาน | Image |  | Show_If |
| 20 | Lat / Long | LatLong |  |  |
| 21 | Email พนักงาน | Email |  | Editable_If |
| 22 | ราคา | Price |  | Editable_If, Show_If |
| 23 | สร้างPDFรับคืน | Yes/No |  | Editable_If, Show_If |
| 24 | TimeChange | ChangeCounter |  |  |
| 25 | ตรวจสอบก่อนบันทึกข้อมูล | Number |  | Valid_If |
| 26 | เดือน | Text |  |  |
| 27 | ID_พนักงาน | Ref |  | Editable_If, Show_If |
| 28 | LINK_IMAGE | Text |  |  |
| 29 | รายชื่อจุดส่งในตารางงานประจำวัน | LongText |  |  |
| 30 | New step | Ref |  |  |

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
| นิยามคงที่ | Yes |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

**Editable_If (เงื่อนไขที่แก้ไขได้):**

```
=USERROLE() = "ADMIN"
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"UseLongDateFormat": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": "=USERROLE() = \"ADMIN\"", "Reset_If": null, "Suggested_Values": null}
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
| นิยามคงที่ | Yes |
| ค้นหาได้ | No |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

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
| นิยามคงที่ | Yes |
| ค้นหาได้ | No |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

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
| นิยามคงที่ | Yes |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

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
| นิยามคงที่ | Yes |
| ค้นหาได้ | No |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

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
| นิยามคงที่ | Yes |
| ค้นหาได้ | No |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

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
| นิยามคงที่ | Yes |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

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
| นิยามคงที่ | Yes |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

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
| นิยามคงที่ | Yes |
| ค้นหาได้ | No |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

**Show_If (เงื่อนไขการแสดง):**

```
=IN([สถานะการเข้ารับสินค้า] ,{"(ได้เพิ่ม200) ไม่มีสินค้าคืน หรือ ร้านปิด","(ได้เพิ่ม50%) ของค่า เที่ยว","(ได้เพิ่ม200) ไม่มีในจุด ที่ส่งงานวันนี้","เบิกค่าขนส่งตาม ระยะทาง","ทำเบิกค่ายกขึ้น ชั้น"})
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": "=IN([สถานะการเข้ารับสินค้า] ,{\"(ได้เพิ่ม200) ไม่มีสินค้าคืน หรือ ร้านปิด\",\"(ได้เพิ่ม50%) ของค่า เที่ยว\",\"(ได้เพิ่ม200) ไม่มีในจุด ที่ส่งงานวันนี้\",\"เบิกค่าขนส่งตาม ระยะทาง\",\"ทำเบิกค่ายกขึ้น ชั้น\"})", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
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
| นิยามคงที่ | Yes |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

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
| นิยามคงที่ | Yes |
| ค้นหาได้ | No |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

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
| นิยามคงที่ | Yes |
| ค้นหาได้ | No |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

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
| นิยามคงที่ | Yes |
| ค้นหาได้ | No |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

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
| นิยามคงที่ | Yes |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

- 🔗 **อ้างอิง (Ref) ไปตาราง:** `ข้อมูลพนักงาน`

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

## คอลัมน์ทั่วไป (ไม่มีสูตรหรือเงื่อนไขพิเศษ)

- **2. ID_รับงานคืนได้เงิน200** — ชนิด `Text` (ค่าปกติ)
- **3. สถานะการเข้ารับสินค้า** — ชนิด `Enum` (ค่าปกติ)
- **5. ชื่อ - นามสกุล** — ชนิด `Text` (ค่าปกติ)
- **6. ทะเบียนรถ** — ชนิด `Text` (ค่าปกติ)
- **13. ชื่อเจ้าของสินค้า** — ชนิด `Text` (ค่าปกติ)
- **14. รหัสลูกค้า** — ชนิด `Text` (ค่าปกติ)
- **15. ชื่อลูกค้าที่เข้ารับ** — ชนิด `Text` (ค่าปกติ)
- **16. รูปสินค้า** — ชนิด `Image` (ค่าปกติ)
- **17. รูปบิลรับคืน** — ชนิด `Image` (ค่าปกติ)
- **20. Lat / Long** — ชนิด `LatLong` (ค่าปกติ)
- **24. TimeChange** — ชนิด `ChangeCounter` (ค่าปกติ)
- **26. เดือน** — ชนิด `Text` (ค่าปกติ)
- **28. LINK_IMAGE** — ชนิด `Text` (ค่าปกติ)
- **29. รายชื่อจุดส่งในตารางงานประจำวัน** — ชนิด `LongText` (ค่าปกติ)
- **30. New step** — ชนิด `Ref` (ค่าปกติ)

