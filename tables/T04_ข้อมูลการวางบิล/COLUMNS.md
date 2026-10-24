# คอลัมน์ของตาราง ข้อมูลการวางบิล

รวม **45 คอลัมน์** (จาก Schema `ข้อมูลการวางบิล_Schema`)

| # | ชื่อคอลัมน์ | ชนิด | สถานะ | สูตร/เงื่อนไข |
|---:|---|---|---|---|
| 1 | _RowNumber | Number | 🔒 🙈 ⚙️ |  |
| 2 | ID_พนักงาน | Ref |  | InitValue, Editable_If, Show_If |
| 3 | ID_วางบิล | Text | 🔑 🏷️ 🔒 | InitValue |
| 4 | ชื่องาน | Text |  | Valid_If, Editable_If |
| 5 | วันที่ | Date |  | InitValue, Editable_If |
| 6 | ชื่อ - นามสกุล | Text | 🔒 | InitValue |
| 7 | ทะเบียนรถ | Text | 🔒 | InitValue |
| 8 | สถานที่รับงาน (ต้นทาง) | Text | 🔒 | InitValue, Reset_If |
| 9 | สถานที่ส่งงาน (ปลายทาง) | Text | 🔒 | InitValue, Reset_If |
| 10 | Email พนักงาน | Email |  | InitValue, Editable_If |
| 11 | พิมอธิบายทุกอย่างที่สำคัญ | LongText |  | Editable_If |
| 12 | Shipment No | Number |  | Valid_If, Required_If, Editable_If, Show_If |
| 13 | ระยะทางที่วิ่ง (KM) | Number |  | InitValue, Editable_If, Show_If, Reset_If |
| 14 | จำนวนจุดรับ / จุดส่ง | Number |  | Editable_If, Show_If, Reset_If |
| 15 | จำนวนร้านที่ยกขึ้นชั้น | Number |  | Editable_If, Show_If, Reset_If |
| 16 | ราคา | Price |  | InitValue, Editable_If, Show_If, Reset_If |
| 17 | Email ผู้อนุมัติ | Email |  | AppFormula |
| 18 | สถานะการอนุมัติ | Enum |  | InitValue, Editable_If |
| 19 | ราคาในระบบหลังส่งสินค้า | Price | 🔒 |  |
| 20 | รูปถ่ายหลังรถตอนขึ้นสินค้าเสร็จ | Image |  |  |
| 21 | รูปถ่ายบิลงาน | Image |  |  |
| 22 | รูปถ่ายบิลงานเพิ่ม1 | Image |  |  |
| 23 | รูปถ่ายบิลงานเพิ่ม2 | Image |  |  |
| 24 | เลือกเพิ่มเติม | Enum |  | Editable_If, Show_If, Reset_If |
| 25 | ยืนยันการกรอกข้อมูล | Enum |  | InitValue, Valid_If, Show_If |
| 26 | เดือน | Text | 🔒 | InitValue |
| 27 | ระบุการเติมน้ำมัน | Yes/No |  | Show_If |
| 28 | ราคาที่เติม | Decimal |  | Show_If |
| 29 | รูปถ่ายใบเสร็จน้ำมัน_ใบเล็ก | Image |  | Show_If |
| 30 | ระบุทางด่วนM-Flow | Yes/No |  | Show_If |
| 31 | จำนวนด่าน | Number |  | Show_If |
| 32 | รูปสลิปการโอน | Image |  | Show_If |
| 33 | ระบุการซ่อมบำรุง | Yes/No |  | Show_If |
| 34 | ราคาตามบิล | Number |  | Show_If |
| 35 | รูปถ่ายบิลซ่อมบำรุง | Image |  | Show_If |
| 36 | ราคาจุดเพิ่ม | Price | 🔒 | AppFormula, Show_If |
| 37 | ราคาตามระยะทาง | Price | 🔒 | AppFormula, Show_If |
| 38 | เรทดีเซล | Price | 🔒 | AppFormula |
| 39 | ราคาเพิ่ม | Price | 🔒 | AppFormula, Show_If |
| 40 | ข้อความแจ้งเตือน | Text | 🔒 | AppFormula, Show_If |
| 41 | ราคาหลังส่งสินค้า | Price | 🔒 | AppFormula |
| 42 | ราคาก่อนส่งสินค้า | Price | 🔒 | AppFormula |
| 43 | ราคาที่อนุมัติแล้ว | Price | 🔒 | AppFormula, Show_If |
| 44 | SM | Number | 🔒 | AppFormula |
| 45 | ราคาหลังส่งเอเธน | Price | 🔒 | AppFormula |

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

### 2. ID_พนักงาน

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

### 3. ID_วางบิล

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

### 4. ชื่องาน

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
=SELECT(
 ข้อมูลชื่อ งานต้นทางปลายทาง[ชื่องาน],
 AND
 (TRUE,NOT(IN([ชื่องาน], {"เบทาโกร","เหมา ตู้"}))
))
```

**Editable_If (เงื่อนไขที่แก้ไขได้):**

```
=OR(
USERROLE() = "ADMIN" ,[สถานะการอนุมัติ]<>"อนุมัติ" )
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": "=SELECT(\n ข้อมูลชื่อ งานต้นทางปลายทาง[ชื่องาน],\n AND\n (TRUE,NOT(IN([ชื่องาน], {\"เบทาโกร\",\"เหมา ตู้\"}))\n))", "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": "=OR(\nUSERROLE() = \"ADMIN\" ,[สถานะการอนุมัติ]<>\"อนุมัติ\" )", "Reset_If": null, "Suggested_Values": null}
```

</details>

### 5. วันที่

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
=USERROLE()= "ADMIN"
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"UseLongDateFormat": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": "=USERROLE()= \"ADMIN\"", "Reset_If": null, "Suggested_Values": null}
```

</details>

### 6. ชื่อ - นามสกุล

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

### 7. ทะเบียนรถ

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

### 8. สถานที่รับงาน (ต้นทาง)

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Text |
| Key | No |
| Label | No |
| Virtual | No |
| Read-Only | Yes |
| Hidden | No |
| รีเซ็ตเมื่อแก้ไข | =[_THISROW_BEFORE].[ชื่องาน] <> [_THISROW].[ชื่องาน] |
| คอลัมน์ระบบ | No |
| ส่วนหนึ่งของ Key | No |
| นิยามคงที่ | No |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**ค่าเริ่มต้น (Initial Value):**

```
=LOOKUP([_THISROW].[ชื่องาน],"ข้อมูลชื่องานต้นทางปลาย ทาง","ชื่องาน","สถานที่รับสินค้า (ต้นทาง)")
```

**Reset_If (เงื่อนไขรีเซ็ต):**

```
=[_THISROW_BEFORE].[ชื่องาน] <> [_THISROW].[ชื่องาน]
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": "=[_THISROW_BEFORE].[ชื่องาน] <> [_THISROW].[ชื่องาน]", "Suggested_Values": null}
```

</details>

### 9. สถานที่ส่งงาน (ปลายทาง)

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Text |
| Key | No |
| Label | No |
| Virtual | No |
| Read-Only | Yes |
| Hidden | No |
| รีเซ็ตเมื่อแก้ไข | =[_THISROW_BEFORE].[ชื่องาน] <> [_THISROW].[ชื่องาน] |
| คอลัมน์ระบบ | No |
| ส่วนหนึ่งของ Key | No |
| นิยามคงที่ | No |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**ค่าเริ่มต้น (Initial Value):**

```
=LOOKUP([_THISROW].[ชื่องาน],"ข้อมูลชื่องานต้นทางปลาย ทาง","ชื่องาน","สถานที่ส่งสินค้า (ปลายทาง)")
```

**Reset_If (เงื่อนไขรีเซ็ต):**

```
=[_THISROW_BEFORE].[ชื่องาน] <> [_THISROW].[ชื่องาน]
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": "=[_THISROW_BEFORE].[ชื่องาน] <> [_THISROW].[ชื่องาน]", "Suggested_Values": null}
```

</details>

### 10. Email พนักงาน

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

### 11. พิมอธิบายทุกอย่างที่สำคัญ

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

**Editable_If (เงื่อนไขที่แก้ไขได้):**

```
=OR(
 USERROLE() = "ADMIN" ,[สถานะการอนุมัติ]<>"อนุมัติ" )
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": "=OR(\n USERROLE() = \"ADMIN\" ,[สถานะการอนุมัติ]<>\"อนุมัติ\" )", "Reset_If": null, "Suggested_Values": null}
```

</details>

### 12. Shipment No

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
=AND(
 [_THIS] >= 100000000,
 [_THIS] <= 999999999,
 ISBLANK(
 ANY(SELECT(ข้อมูลการวาง บิล[Shipment No], [Shipment No] = [_THIS]))
 )
)
```

**Required_If (เงื่อนไขบังคับกรอก):**

```
=IN([ชื่องาน], LIST("ภูมิภาค","นครหลวง","04JB_นครหลวง_ภูมิภาค","Idem_04ID"))
```

**Editable_If (เงื่อนไขที่แก้ไขได้):**

```
=OR(
USERROLE() = "ADMIN" ,[สถานะการอนุมัติ]<>"อนุมัติ" )
```

**Show_If (เงื่อนไขการแสดง):**

```
=IN([ชื่องาน], LIST("ภูมิภาค","นครหลวง","04JB_นครหลวง_ภูมิภาค","สตีเบลเอลทรอน เอเซีย จํากัด","Idem_04ID","โอนคลัง บุญถาวร รังสิต","โอนคลัง บุญถาวร เกษตร_นวมินทร์","โอนคลัง ยนตรกิจ (ร่มเกล้า) YONTRAKIT","โอนคลัง (GQ) จีคิว","โอนคลัง พีโอเอส ดิสเพลย์","โอนคลัง CPF FOOD","โอนคลัง Mizuno","โอนคลัง ทีจีโฟน","โอนคลัง TRW","โอนคลัง BYD","โอนคลัง ซอยฮะ (โก เรีย)", "โอนคลัง โลจิสท์พลัส" , "โอนคลัง SIS" , "โอนคลัง พว.","คลังSCGJWDวังน้อย","Lyreco (Thailand)","น้ำมะปี๊ด(ปั้มบางจาก)FarmZaa"))
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxValue": null, "MinValue": null, "StepValue": null, "NumericDigits": null, "ShowThousandsSeparator": false, "NumberDisplayMode": "Auto", "Valid_If": "=AND(\n [_THIS] >= 100000000,\n [_THIS] <= 999999999,\n ISBLANK(\n ANY(SELECT(ข้อมูลการวาง บิล[Shipment No], [Shipment No] = [_THIS]))\n )\n)", "Error_Message_If_Invalid": null, "Show_If": "=IN([ชื่องาน], LIST(\"ภูมิภาค\",\"นครหลวง\",\"04JB_นครหลวง_ภูมิภาค\",\"สตีเบลเอลทรอน เอเซีย จํากัด\",\"Idem_04ID\",\"โอนคลัง บุญถาวร รังสิต\",\"โอนคลัง บุญถาวร เกษตร_นวมินทร์\",\"โอนคลัง ยนตรกิจ (ร่มเกล้า) YONTRAKIT\",\"โอนคลัง (GQ) จีคิว\",\"โอนคลัง พีโอเอส ดิสเพลย์\",\"โอนคลัง CPF FOOD\",\"โอนคลัง Mizuno\",\"โอนคลัง ทีจีโฟน\",\"โอนคลัง TRW\",\"โอนคลัง BYD\",\"โอนคลัง ซอยฮะ (โก เรีย)\", \"โอนคลัง โลจิสท์พลัส\" , \"โอนคลัง SIS\" , \"โอนคลัง พว.\",\"คลังSCGJWDวังน้อย\",\"Lyreco (Thailand)\",\"น้ำมะปี๊ด(ปั้มบางจาก)FarmZaa\"))", "Required_If": "=IN([ชื่องาน], LIST(\"ภูมิภาค\",\"นครหลวง\",\"04JB_นครหลวง_ภูมิภาค\",\"Idem_04ID\"))", "Editable_If": "=OR(\nUSERROLE() = \"ADMIN\" ,[สถานะการอนุมัติ]<>\"อนุมัติ\" )", "Reset_If": null, "Suggested_Values": null}
```

</details>

### 13. ระยะทางที่วิ่ง (KM)

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Number |
| Key | No |
| Label | No |
| Virtual | No |
| Read-Only | No |
| Hidden | No |
| รีเซ็ตเมื่อแก้ไข | =[_THISROW_BEFORE].[ชื่องาน] <> [_THISROW].[ชื่องาน] |
| คอลัมน์ระบบ | No |
| ส่วนหนึ่งของ Key | No |
| นิยามคงที่ | No |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**ค่าเริ่มต้น (Initial Value):**

```
=LOOKUP([_THISROW].[ชื่องาน], "ข้อมูลชื่องานต้นทางปลายทาง", "ชื่องาน", "ระยะทางคงที่")
```

**Editable_If (เงื่อนไขที่แก้ไขได้):**

```
=OR(
USERROLE() = "ADMIN" ,[สถานะการอนุมัติ]<>"อนุมัติ" )
```

**Show_If (เงื่อนไขการแสดง):**

```
=IN([ชื่องาน], LIST("เบทาโกร+เหมาตู้","ออเรนจ์โคร","ไอโรบอท","อิริคสัน","เอเทน","MeSpace","ฟ้าใส (SCG Express)","รูทรังสิต(SCG Express)","Thai paper (SCG Express)","โอนคลัง ไอโร บอท","นิคมหนองแค ส่งเอกสาร บีเจซี มูฟ","โอนคลัง (TVS) ชาญ ไพบูลย์","โอนคลัง ทีจีโฟน","โอนคลัง เอเธน","โอนคลัง พว.","โอนคลัง ซอยฮะ (โกเรีย)","โอนคลัง นำวิวัฒน์","โอนคลัง กระสอบ2(บางบัวทอง)","โอนคลัง โลจิสท์พลัส","โอนคลัง SIS"))
```

**Reset_If (เงื่อนไขรีเซ็ต):**

```
= [_THISROW_BEFORE].[ชื่องาน] <> [_THISROW].[ชื่องาน]
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxValue": null, "MinValue": null, "StepValue": null, "NumericDigits": null, "ShowThousandsSeparator": false, "NumberDisplayMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": "=IN([ชื่องาน], LIST(\"เบทาโกร+เหมาตู้\",\"ออเรนจ์โคร\",\"ไอโรบอท\",\"อิริคสัน\",\"เอเทน\",\"MeSpace\",\"ฟ้าใส (SCG Express)\",\"รูทรังสิต(SCG Express)\",\"Thai paper (SCG Express)\",\"โอนคลัง ไอโร บอท\",\"นิคมหนองแค ส่งเอกสาร บีเจซี มูฟ\",\"โอนคลัง (TVS) ชาญ ไพบูลย์\",\"โอนคลัง ทีจีโฟน\",\"โอนคลัง เอเธน\",\"โอนคลัง พว.\",\"โอนคลัง ซอยฮะ (โกเรีย)\",\"โอนคลัง นำวิวัฒน์\",\"โอนคลัง กระสอบ2(บางบัวทอง)\",\"โอนคลัง โลจิสท์พลัส\",\"โอนคลัง SIS\"))", "Required_If": null, "Editable_If": "=OR(\nUSERROLE() = \"ADMIN\" ,[สถานะการอนุมัติ]<>\"อนุมัติ\" )", "Reset_If": "= [_THISROW_BEFORE].[ชื่องาน] <> [_THISROW].[ชื่องาน]", "Suggested_Values": null}
```

</details>

### 14. จำนวนจุดรับ / จุดส่ง

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Number |
| Key | No |
| Label | No |
| Virtual | No |
| Read-Only | No |
| Hidden | No |
| รีเซ็ตเมื่อแก้ไข | =[_THISROW_BEFORE].[ชื่องาน] <> [_THISROW].[ชื่องาน] |
| คอลัมน์ระบบ | No |
| ส่วนหนึ่งของ Key | No |
| นิยามคงที่ | No |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**Editable_If (เงื่อนไขที่แก้ไขได้):**

```
=OR(
USERROLE() = "ADMIN" ,[สถานะการอนุมัติ]<>"อนุมัติ" )
```

**Show_If (เงื่อนไขการแสดง):**

```
=IN([ชื่องาน], LIST( "เบทาโกร+เหมาตู้","ออเรนจ์โคร", "ไอโร บอท"))
```

**Reset_If (เงื่อนไขรีเซ็ต):**

```
= [_THISROW_BEFORE].[ชื่องาน] <> [_THISROW].[ชื่องาน]
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxValue": null, "MinValue": null, "StepValue": null, "NumericDigits": null, "ShowThousandsSeparator": false, "NumberDisplayMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": "=IN([ชื่องาน], LIST( \"เบทาโกร+เหมาตู้\",\"ออเรนจ์โคร\", \"ไอโร บอท\"))", "Required_If": null, "Editable_If": "=OR(\nUSERROLE() = \"ADMIN\" ,[สถานะการอนุมัติ]<>\"อนุมัติ\" )", "Reset_If": "= [_THISROW_BEFORE].[ชื่องาน] <> [_THISROW].[ชื่องาน]", "Suggested_Values": null}
```

</details>

### 15. จำนวนร้านที่ยกขึ้นชั้น

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Number |
| Key | No |
| Label | No |
| Virtual | No |
| Read-Only | No |
| Hidden | No |
| รีเซ็ตเมื่อแก้ไข | =[_THISROW_BEFORE].[ชื่องาน] <> [_THISROW].[ชื่องาน] |
| คอลัมน์ระบบ | No |
| ส่วนหนึ่งของ Key | No |
| นิยามคงที่ | No |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**Editable_If (เงื่อนไขที่แก้ไขได้):**

```
=OR(
USERROLE() = "ADMIN" ,[สถานะการอนุมัติ]<>"อนุมัติ" )
```

**Show_If (เงื่อนไขการแสดง):**

```
=IN([ชื่องาน], LIST( "เอเทน","ออเรนจ์ โคร"))
```

**Reset_If (เงื่อนไขรีเซ็ต):**

```
= [_THISROW_BEFORE].[ชื่องาน] <> [_THISROW].[ชื่องาน]
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxValue": null, "MinValue": null, "StepValue": null, "NumericDigits": null, "ShowThousandsSeparator": false, "NumberDisplayMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": "=IN([ชื่องาน], LIST( \"เอเทน\",\"ออเรนจ์ โคร\"))", "Required_If": null, "Editable_If": "=OR(\nUSERROLE() = \"ADMIN\" ,[สถานะการอนุมัติ]<>\"อนุมัติ\" )", "Reset_If": "= [_THISROW_BEFORE].[ชื่องาน] <> [_THISROW].[ชื่องาน]", "Suggested_Values": null}
```

</details>

### 16. ราคา

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Price |
| Key | No |
| Label | No |
| Virtual | No |
| Read-Only | No |
| Hidden | No |
| รีเซ็ตเมื่อแก้ไข | =[_THISROW_BEFORE].[ชื่องาน] <> [_THISROW].[ชื่องาน] |
| คอลัมน์ระบบ | No |
| ส่วนหนึ่งของ Key | No |
| นิยามคงที่ | No |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**ค่าเริ่มต้น (Initial Value):**

```
=IFS( ISBLANK([ชื่องาน]), 0, ISNOTBLANK(LOOKUP([_THISROW].[ชื่องาน], "ข้อมูลชื่องาน ต้นทางปลายทาง", "ชื่องาน", "ราคาคงที่")), LOOKUP([_THISROW]. [ชื่องาน], "ข้อมูลชื่องานต้นทางปลายทาง", "ชื่องาน", "ราคาคงที่") + [ราคาจุดเพิ่ม], ISNOTBLANK(LOOKUP([_THISROW].[Shipment No], "ราคาในระบบก่อนส่งสินค้า", "Shipment No", "ราคา")), LOOKUP([_THISROW].[Shipment No], "ราคาในระบบก่อนส่งสินค้า","Shipment No", "ราคา"), TRUE, [ราคาตามระยะทาง] + [ราคาจุดเพิ่ม]+ [ราคาเพิ่ม] )
```

**Editable_If (เงื่อนไขที่แก้ไขได้):**

```
=USERROLE()= "ADMIN"
```

**Show_If (เงื่อนไขการแสดง):**

```
=OR(
USERROLE() = "ADMIN" ,[สถานะการอนุมัติ]<>"อนุมัติ" )
```

**Reset_If (เงื่อนไขรีเซ็ต):**

```
=[_THISROW_BEFORE].[ชื่องาน] <> [_THISROW].[ชื่องาน]
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"CurrencySymbol": "฿", "MaxValue": null, "MinValue": null, "StepValue": null, "DecimalDigits": 2, "NumericDigits": null, "ShowThousandsSeparator": true, "NumberDisplayMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": "=OR(\nUSERROLE() = \"ADMIN\" ,[สถานะการอนุมัติ]<>\"อนุมัติ\" )", "Required_If": null, "Editable_If": "=USERROLE()= \"ADMIN\"", "Reset_If": "=[_THISROW_BEFORE].[ชื่องาน] <> [_THISROW].[ชื่องาน]", "Suggested_Values": null}
```

</details>

### 17. Email ผู้อนุมัติ

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

**App Formula (สูตรคำนวณ):**

```
=IF([สถานะการอนุมัติ]="อนุมัติ", USEREMAIL(), [Email ผู้อนุมัติ])
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 18. สถานะการอนุมัติ

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

**ค่าเริ่มต้น (Initial Value):**

```
="รอการอนุมัติ”
```

**Editable_If (เงื่อนไขที่แก้ไขได้):**

```
=USERROLE()= "ADMIN"
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"EnumValues": ["อนุมัติ", "รอการ อนุมัติ"], "AllowOtherValues": false, "AutoCompleteOtherValues": true, "BaseType": "Text", "BaseTypeQualifier": " {\"MaxLength\":null,\"MinLength\":null,\"LongTextFormatting\":\"Plain Text\",\"IsMulticolumnKey\":false,\"Valid_If\":null,\"Error_Message_If_Invalid\":null,\"Show_If\":null,\"Required_If\":null,\"Editable_If\":null,\"Reset_If\":null,\"Suggested_Values\":null}", "EnumInputMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": "=USERROLE()= \"ADMIN\"", "Reset_If": null, "Suggested_Values": null}
```

</details>

### 24. เลือกเพิ่มเติม

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Enum |
| Key | No |
| Label | No |
| Virtual | No |
| Read-Only | No |
| Hidden | No |
| รีเซ็ตเมื่อแก้ไข | =[_THISROW_BEFORE].[ชื่องาน] <> [_THISROW].[ชื่องาน] |
| คอลัมน์ระบบ | No |
| ส่วนหนึ่งของ Key | No |
| นิยามคงที่ | No |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**Editable_If (เงื่อนไขที่แก้ไขได้):**

```
=OR(
USERROLE() = "ADMIN" ,[สถานะการอนุมัติ]<>"อนุมัติ" )
```

**Show_If (เงื่อนไขการแสดง):**

```
=[ชื่องาน] ="MeSpace"
```

**Reset_If (เงื่อนไขรีเซ็ต):**

```
= [_THISROW_BEFORE].[ชื่องาน] <> [_THISROW].[ชื่องาน]
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"EnumValues": ["งานMeSpace+แพ็คสินค้า", "จองรถ ก่อน14.00+แรงงาน1คน", "เพิ่ม แรงงาน1คน"], "AllowOtherValues": false, "AutoCompleteOtherValues": true, "BaseType": "Text", "BaseTypeQualifier": " {\"MaxLength\":null,\"MinLength\":null,\"LongTextFormatting\":\"Plain Text\",\"IsMulticolumnKey\":false,\"Valid_If\":null,\"Error_Message_If_Invalid\":null,\"Show_If\":null,\"Required_If\":null,\"Editable_If\":null,\"Reset_If\":null,\"Suggested_Values\":null}", "EnumInputMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": "=[ชื่องาน] =\"MeSpace\"", "Required_If": null, "Editable_If": "=OR(\nUSERROLE() = \"ADMIN\" ,[สถานะการอนุมัติ]<>\"อนุมัติ\" )", "Reset_If": "= [_THISROW_BEFORE].[ชื่องาน] <> [_THISROW].[ชื่องาน]", "Suggested_Values": null}
```

</details>

### 25. ยืนยันการกรอกข้อมูล

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

**ค่าเริ่มต้น (Initial Value):**

```
="ไม่ได้ตรวจสอบ"
```

**Valid_If (เงื่อนไขความถูกต้อง):**

```
=IF([ยืนยันการกรอกข้อมูล] = "ตรวจสอบข้อมูลเรียบร้อย" , TRUE , FALSE)
```

**Show_If (เงื่อนไขการแสดง):**

```
=ISNOTBLANK([รูปถ่ายบิลงาน])
```

**ข้อความเตือนเมื่อค่าไม่ถูกต้อง:**

```
="กรุณาตรวจสอบข้อมูลที่ กรอกเข้ามาอีกรอบ"
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"EnumValues": ["ไม่ได้ตรวจสอบ", "ตรวจสอบข้อมูล เรียบร้อย"], "AllowOtherValues": false, "AutoCompleteOtherValues": true, "BaseType": "Text", "BaseTypeQualifier": " {\"MaxLength\":null,\"MinLength\":null,\"LongTextFormatting\":\"Plain Text\",\"IsMulticolumnKey\":false,\"Valid_If\":null,\"Error_Message_If_Invalid\":null,\"Show_If\":null,\"Required_If\":null,\"Editable_If\":null,\"Reset_If\":null,\"Suggested_Values\":null}", "EnumInputMode": "Dropdown", "Valid_If": "=IF([ยืนยันการกรอกข้อมูล] = \"ตรวจสอบข้อมูลเรียบร้อย\" , TRUE , FALSE)", "Error_Message_If_Invalid": "=\"กรุณาตรวจสอบข้อมูลที่ กรอกเข้ามาอีกรอบ\"", "Show_If": "=ISNOTBLANK([รูปถ่ายบิลงาน])", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
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
=IF( ISBLANK([วันที่]), "", (YEAR([วันที่]) - IF(YEAR([วันที่]) > 2500, 543, 0)) & "-" & TEXT([วันที่], "MM") )
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 27. ระบุการเติมน้ำมัน

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

**Show_If (เงื่อนไขการแสดง):**

```
= OR(
 USERROLE() = "ADMIN",
 IN(
 USEREMAIL(),
 LIST(
 "emp11@example.com",
 "emp14@example.com",
 "emp10@example.com",
 "emp09@example.com",
 "emp04@example.com",
"emp12@example.com",
 "emp03@example.com",
 "emp08@example.com",
 "emp05@example.com",
 "emp13@example.com",
 "emp01@example.com",
"emp07@example.com",
 "emp02@example.com",
 "emp06@example.com"
 )
 )
)
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"YesLabel": "=มีการเติมน้ำมัน", "NoLabel": "=ไม่มีการเติม น้ำมัน", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": "= OR(\n USERROLE() = \"ADMIN\",\n IN(\n USEREMAIL(),\n LIST(\n \"emp11@example.com\",\n \"emp14@example.com\",\n \"emp10@example.com\",\n \"emp09@example.com\",\n \"emp04@example.com\",\n\"emp12@example.com\",\n \"emp03@example.com\",\n \"emp08@example.com\",\n \"emp05@example.com\",\n \"emp13@example.com\",\n \"emp01@example.com\",\n\"emp07@example.com\",\n \"emp02@example.com\",\n \"emp06@example.com\"\n )\n )\n)", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 28. ราคาที่เติม

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

**Show_If (เงื่อนไขการแสดง):**

```
=[ระบุการเติมน้ำมัน] = TRUE
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxValue": null, "MinValue": null, "StepValue": null, "DecimalDigits": 2, "NumericDigits": null, "ShowThousandsSeparator": true, "NumberDisplayMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": "=[ระบุการเติมน้ำมัน] = TRUE", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 29. รูปถ่ายใบเสร็จน้ำมัน_ใบเล็ก

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
=[ระบุการเติมน้ำมัน] = TRUE
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": "=[ระบุการเติมน้ำมัน] = TRUE", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 30. ระบุทางด่วนM-Flow

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

**Show_If (เงื่อนไขการแสดง):**

```
=AND(
 OR(
 USERROLE() = "ADMIN",
 IN(
 USEREMAIL(),
 LIST(
 "emp11@example.com",
 "emp14@example.com",
 "emp10@example.com",
 "emp09@example.com",
 "emp04@example.com",
"emp12@example.com",
 "emp03@example.com",
 "emp08@example.com",
 "emp05@example.com",
 "emp13@example.com",
 "emp01@example.com",
"emp07@example.com",
 "emp02@example.com",
 "emp06@example.com"
 )
 )
 ),
 ISNOTBLANK([ระบุการ เติม น้ำมัน])
)
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"YesLabel": "=ใช้ทางด่วน_M_Flow", "NoLabel": "=ไม่ใช้ ทางด่วน", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": "=AND(\n OR(\n USERROLE() = \"ADMIN\",\n IN(\n USEREMAIL(),\n LIST(\n \"emp11@example.com\",\n \"emp14@example.com\",\n \"emp10@example.com\",\n \"emp09@example.com\",\n \"emp04@example.com\",\n\"emp12@example.com\",\n \"emp03@example.com\",\n \"emp08@example.com\",\n \"emp05@example.com\",\n \"emp13@example.com\",\n \"emp01@example.com\",\n\"emp07@example.com\",\n \"emp02@example.com\",\n \"emp06@example.com\"\n )\n )\n ),\n ISNOTBLANK([ระบุการ เติม น้ำมัน])\n)", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 31. จำนวนด่าน

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
=[ระบุทางด่วนM-Flow] = TRUE
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxValue": null, "MinValue": null, "StepValue": null, "NumericDigits": null, "ShowThousandsSeparator": true, "NumberDisplayMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": "=[ระบุทางด่วนM-Flow] = TRUE", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 32. รูปสลิปการโอน

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
=[ระบุทางด่วนM-Flow] = TRUE
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": "=[ระบุทางด่วนM-Flow] = TRUE", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 33. ระบุการซ่อมบำรุง

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

**Show_If (เงื่อนไขการแสดง):**

```
=AND(
 OR(
 USERROLE() = "ADMIN",
 IN(
 USEREMAIL(),
LIST(
 "emp11@example.com",
 "emp14@example.com",
 "emp10@example.com",
 "emp09@example.com",
 "emp04@example.com",
"emp12@example.com",
 "emp03@example.com",
 "emp08@example.com",
 "emp05@example.com",
 "emp13@example.com",
 "emp01@example.com",
"emp07@example.com",
 "emp02@example.com",
 "emp06@example.com"
 )
 )
 ),
 ISNOTBLANK([ระบุทางด่วนM-Flow])
)
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"YesLabel": "=มีการเข้าซ่อม", "NoLabel": "=ไม่มีการเข้า ซ่อม", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": "=AND(\n OR(\n USERROLE() = \"ADMIN\",\n IN(\n USEREMAIL(),\nLIST(\n \"emp11@example.com\",\n \"emp14@example.com\",\n \"emp10@example.com\",\n \"emp09@example.com\",\n \"emp04@example.com\",\n\"emp12@example.com\",\n \"emp03@example.com\",\n \"emp08@example.com\",\n \"emp05@example.com\",\n \"emp13@example.com\",\n \"emp01@example.com\",\n\"emp07@example.com\",\n \"emp02@example.com\",\n \"emp06@example.com\"\n )\n )\n ),\n ISNOTBLANK([ระบุทางด่วนM-Flow])\n)", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 34. ราคาตามบิล

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
=[ระบุการซ่อมบำรุง] = TRUE
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxValue": null, "MinValue": null, "StepValue": null, "NumericDigits": null, "ShowThousandsSeparator": true, "NumberDisplayMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": "=[ระบุการซ่อมบำรุง] = TRUE", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 35. รูปถ่ายบิลซ่อมบำรุง

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
=[ระบุการซ่อมบำรุง] = TRUE
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": "=[ระบุการซ่อมบำรุง] = TRUE", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 36. ราคาจุดเพิ่ม

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
=IFS( AND([ชื่องาน] = "เบทาโกร+เหมาตู้",[จำนวนจุดรับ / จุดส่ง] >= 11), ([จำนวนจุดรับ / จุดส่ง] - 11) * 50, AND([ชื่องาน] = "ไอโรบอท", [จำนวนจุดรับ / จุดส่ง] >= 1), ([จำนวนจุดรับ / จุดส่ง] - 1) * 100, [ชื่องาน] = "ออเรนจ์โคร", (([จำนวนจุดรับ / จุดส่ง] - 1) * 100) + ([จำนวนร้านที่ยกขึ้นชั้น] * 300), [ชื่องาน] = "เอเทน", [จำนวนร้านที่ยกขึ้นชั้น] *250, TRUE, 0 )
```

**Show_If (เงื่อนไขการแสดง):**

```
=OR(USERROLE() = "Admin", [สถานะการอนุมัติ] = "อนุมัติ")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"CurrencySymbol": "฿", "MaxValue": null, "MinValue": null, "StepValue": null, "DecimalDigits": 2, "NumericDigits": null, "ShowThousandsSeparator": true, "NumberDisplayMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": "=OR(USERROLE() = \"Admin\", [สถานะการอนุมัติ] = \"อนุมัติ\")", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 37. ราคาตามระยะทาง

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
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**App Formula (สูตรคำนวณ):**

```
=ANY( SELECT( Price_Table[Price], AND( IN( [_THISROW].[ชื่องาน], SPLIT([ชื่องาน], ",") ), [เรทน้ำมัน_Minimum] <= [_THISROW]. [เรทดีเซล], [เรทน้ำมัน_Maximum] >= [_THISROW].[เรทดีเซล], [ระยะทาง_Minimum] <= [_THISROW].[ระยะทางที่วิ่ง (KM)], [ระยะทาง_Maximum] >= [_THISROW].[ระยะทางที่วิ่ง (KM)] ) ) )
```

**Show_If (เงื่อนไขการแสดง):**

```
=OR(USERROLE() = "Admin", [สถานะการอนุมัติ] = "อนุมัติ")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"CurrencySymbol": "฿", "MaxValue": null, "MinValue": null, "StepValue": null, "DecimalDigits": 2, "NumericDigits": null, "ShowThousandsSeparator": true, "NumberDisplayMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": "=OR(USERROLE() = \"Admin\", [สถานะการอนุมัติ] = \"อนุมัติ\")", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 38. เรทดีเซล

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
=IF( ISBLANK([_THISROW].[วันที่]), "", IF( ISNOTBLANK( ANY( SELECT( PriceOverride[UsePriceDate], AND( [StartDate] <= [_THISROW].[วันที่], [EndDate] >= [_THISROW].[วันที่], [JobName] = [_THISROW].[ชื่องาน] ) ) ) ), ANY( SELECT( ราคาน้ำมัน ดีเซล[ราคา/หน่วย], [วันที่] = ANY( SELECT( PriceOverride[UsePriceDate], AND( [StartDate] <= [_THISROW]. [วันที่], [EndDate] >= [_THISROW].[วันที่], [JobName] = [_THISROW].[ชื่องาน] ) ) ) ) ), IF( ISNOTBLANK( ANY( SELECT( PriceOverride[UsePriceDate], AND( [StartDate] <= [_THISROW]. [วันที่], [EndDate] >= [_THISROW].[วันที่], ISBLANK([JobName]) ) )) ), ANY( SELECT( ราคาน้ำมันดีเซล[ราคา/หน่วย], [วันที่] = ANY( SELECT( PriceOverride[UsePriceDate], AND( [StartDate] <= [_THISROW].[วันที่], [EndDate] >= [_THISROW].[วันที่], ISBLANK([JobName]) ) ) ) ) ), ANY( SELECT( ราคาน้ำมัน ดีเซล[ราคา/หน่วย], [วันที่] = DATE( CONCATENATE( YEAR(EOMONTH([_THISROW].[วันที่], -1)), "-", RIGHT("0" & MONTH(EOMONTH([_THISROW].[วันที่], -1)), 2), "-25" ) ) ) ) ) ) )
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"CurrencySymbol": "฿", "MaxValue": null, "MinValue": null, "StepValue": null, "DecimalDigits": 2, "NumericDigits": null, "ShowThousandsSeparator": true, "NumberDisplayMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 39. ราคาเพิ่ม

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
=IF([เลือกเพิ่มเติม] = "เพิ่มแรงงาน1คน",500, IF([เลือกเพิ่มเติม] = "จองรถก่อน14.00+แรงงาน1คน",1200, IF([เลือกเพิ่มเติม] = "งานMeSpace+แพ็คสินค้า",2400,0)))
```

**Show_If (เงื่อนไขการแสดง):**

```
=[ชื่องาน] ="MeSpace"
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"CurrencySymbol": "฿", "MaxValue": null, "MinValue": null, "StepValue": null, "DecimalDigits": 2, "NumericDigits": null, "ShowThousandsSeparator": true, "NumberDisplayMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": "=[ชื่องาน] =\"MeSpace\"", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 40. ข้อความแจ้งเตือน

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
=IF([ยืนยันการกรอกข้อมูล] = "ตรวจสอบข้อมูลเรียบร้อย", "✅ ยืนยันสำเร็จ กลับไปบันทึกข้อมูลได้", "")
```

**Show_If (เงื่อนไขการแสดง):**

```
=TRUE
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": "=TRUE", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 41. ราคาหลังส่งสินค้า

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
=LOOKUP([_THISROW].[Shipment No],"ราคาในระบบก่อนส่ง สินค้า","Shipment No","ราคาหลังส่งสินค้า")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"CurrencySymbol": "฿", "MaxValue": null, "MinValue": null, "StepValue": null, "DecimalDigits": 2, "NumericDigits": null, "ShowThousandsSeparator": true, "NumberDisplayMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 42. ราคาก่อนส่งสินค้า

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
=LOOKUP([_THISROW].[Shipment No],"ราคาในระบบก่อนส่ง สินค้า","Shipment No","ราคา")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"CurrencySymbol": "฿", "MaxValue": null, "MinValue": null, "StepValue": null, "DecimalDigits": 2, "NumericDigits": null, "ShowThousandsSeparator": true, "NumberDisplayMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 43. ราคาที่อนุมัติแล้ว

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
=IF( [สถานะการอนุมัติ] = "อนุมัติ", [ราคา], 0 )
```

**Show_If (เงื่อนไขการแสดง):**

```
=OR(USERROLE() = "Admin", [สถานะการอนุมัติ] = "อนุมัติ")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"CurrencySymbol": "฿", "MaxValue": null, "MinValue": null, "StepValue": null, "DecimalDigits": 2, "NumericDigits": null, "ShowThousandsSeparator": true, "NumberDisplayMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": "=OR(USERROLE() = \"Admin\", [สถานะการอนุมัติ] = \"อนุมัติ\")", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 44. SM

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
=LEFT([พิมอธิบายทุกอย่างที่สำคัญ], FIND("//", [พิมอธิบายทุกอย่างที่สำคัญ]) - 1)
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxValue": null, "MinValue": null, "StepValue": null, "NumericDigits": null, "ShowThousandsSeparator": false, "NumberDisplayMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 45. ราคาหลังส่งเอเธน

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
| ข้อมูลอ่อนไหว | No Schema Name ตารางงานประจำวัน_Schema |
| Locale | en-GB |

**App Formula (สูตรคำนวณ):**

```
=IF( [ชื่องาน] = "เอเทน", LOOKUP( [SM], "ราคาในระบบก่อนส่ง สินค้า", "Shipment No", "ราคาหลังส่งสินค้า" ), "" )
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"CurrencySymbol": "฿", "MaxValue": null, "MinValue": null, "StepValue": null, "DecimalDigits": 2, "NumericDigits": null, "ShowThousandsSeparator": true, "NumberDisplayMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

## คอลัมน์ทั่วไป (ไม่มีสูตรหรือเงื่อนไขพิเศษ)

- **19. ราคาในระบบหลังส่งสินค้า** — ชนิด `Price` (Read-Only=Yes)
- **20. รูปถ่ายหลังรถตอนขึ้นสินค้าเสร็จ** — ชนิด `Image` (ค่าปกติ)
- **21. รูปถ่ายบิลงาน** — ชนิด `Image` (ค่าปกติ)
- **22. รูปถ่ายบิลงานเพิ่ม1** — ชนิด `Image` (ค่าปกติ)
- **23. รูปถ่ายบิลงานเพิ่ม2** — ชนิด `Image` (ค่าปกติ)

