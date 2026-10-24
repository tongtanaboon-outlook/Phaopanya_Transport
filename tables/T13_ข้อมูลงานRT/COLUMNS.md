# คอลัมน์ของตาราง ข้อมูลงานRT

รวม **12 คอลัมน์** (จาก Schema `ข้อมูลงานRT_Schema`)

| # | ชื่อคอลัมน์ | ชนิด | สถานะ | สูตร/เงื่อนไข |
|---:|---|---|---|---|
| 1 | _RowNumber | Number | 🔒 🙈 ⚙️ |  |
| 2 | ID_RT | Text | 🔑 🏷️ | InitValue |
| 3 | Shipment (หลัก) | Number |  |  |
| 4 | Shipment (รับคืน) | Number |  |  |
| 5 | วันที่เข้ารับ | Date |  |  |
| 6 | เลขที่เอกสารรับคืน | Text |  |  |
| 7 | ชื่อลูกค้าที่เข้ารับ | Text |  |  |
| 8 | ชื่อ - นามสกุล | Text |  |  |
| 9 | ทะเบียนรถ | Text |  |  |
| 10 | รหัสลูกค้า | Text |  |  |
| 11 | เดือน | Text | 🔒 | AppFormula |
| 12 | Related แจ้งปัญหาระหว่างวันs | List | 🔒 ⚙️ | AppFormula |

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

### 2. ID_RT

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
=UNIQUEID()
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 11. เดือน

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
=IF( ISBLANK([วันที่เข้ารับ]), "", CONCATENATE( YEAR([วันที่เข้ารับ]) - IF(YEAR([วันที่เข้ารับ]) > 2500, 543, 0), "-", TEXT([วันที่เข้ารับ],"MM") ) )
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 12. Related แจ้งปัญหาระหว่างวันs

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
| ข้อมูลอ่อนไหว | No Schema Name FILTER_Schema |
| Locale | en-GB |

**App Formula (สูตรคำนวณ):**

```
=REF_ROWS("แจ้งปัญหาระหว่างวัน", "RT_Link")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"ElementType": "Ref", "ElementTypeQualifier": " {\"ReferencedTableName\":\"แจ้งปัญหาระหว่าง วัน\",\"ReferencedRootTableName\":\"แจ้งปัญหาระหว่าง วัน\",\"ReferencedType\":\"Text\",\"ReferencedTypeQualifier\":\"{\\\"MaxLength\\\":null,\\\"MinLength\\\":null,\\\"LongTextFor matting\\\":\\\"Plain Text\\\",\\\"IsMulticolumnKey\\\":false,\\\"Valid_If\\\":null,\\\"Error_Message_If_Invalid\\\":null,\\\"Show_If\\\":null,\\\"Required_If\\\":null,\\\"Editable_If\\\":null,\\\"Reset_If\\\":null,\\\"Suggested_Values\\\":null}\",\"ReferencedKeyColumn\":\"ID_แจ้งปัญหาระหว่าง วัน\",\"IsAPartOf\":false,\"RelationshipName\":null,\"InputMode\":\"Auto\",\"Valid_If\":null,\"Error_Message_If_Invalid\":null,\"Show_If\":null,\"Required_If\":null,\"Editable_If\":null,\"Reset_If\":null,\"Suggested_Values\":null}", "ItemSeparator": " , ", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

## คอลัมน์ทั่วไป (ไม่มีสูตรหรือเงื่อนไขพิเศษ)

- **3. Shipment (หลัก)** — ชนิด `Number` (ค่าปกติ)
- **4. Shipment (รับคืน)** — ชนิด `Number` (ค่าปกติ)
- **5. วันที่เข้ารับ** — ชนิด `Date` (ค่าปกติ)
- **6. เลขที่เอกสารรับคืน** — ชนิด `Text` (ค่าปกติ)
- **7. ชื่อลูกค้าที่เข้ารับ** — ชนิด `Text` (ค่าปกติ)
- **8. ชื่อ - นามสกุล** — ชนิด `Text` (ค่าปกติ)
- **9. ทะเบียนรถ** — ชนิด `Text` (ค่าปกติ)
- **10. รหัสลูกค้า** — ชนิด `Text` (ค่าปกติ)

