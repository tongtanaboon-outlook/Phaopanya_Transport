# คอลัมน์ของตาราง Acknowledge_Logs

รวม **11 คอลัมน์** (จาก Schema `Acknowledge_Logs_Schema`)

| # | ชื่อคอลัมน์ | ชนิด | สถานะ | สูตร/เงื่อนไข |
|---:|---|---|---|---|
| 1 | _RowNumber | Number | 🔒 🙈 ⚙️ |  |
| 2 | ID_รับทราบ | Text | 🔑 🏷️ | InitValue |
| 3 | ID_ประกาศ | Ref |  | InitValue |
| 4 | วันที่และเวลารับทราบ | DateTime |  | InitValue |
| 5 | Email พนักงาน | Email |  | InitValue |
| 6 | ชื่อ - นามสกุล | Text |  | InitValue |
| 7 | ทะเบียนรถ | Text |  | InitValue |
| 8 | เลือกเพื่อยืนยัน | Enum |  |  |
| 9 | หมายเหตุ | LongText |  | Show_If |
| 10 | ลงชื่อพนักงาน | Signature |  |  |
| 11 | ข้อความประกาศ | Show | 🔒 | AppFormula, Show_If |

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

### 2. ID_รับทราบ

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

### 3. ID_ประกาศ

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

- 🔗 **อ้างอิง (Ref) ไปตาราง:** `Announcements`

**ค่าเริ่มต้น (Initial Value):**

```
=MAXROW( "Announcements", "วันที่ประกาศ", NOT(IN([ID_ประกาศ], SELECT(Acknowledge_Logs[ID_ประกาศ], [Email พนักงาน] = USEREMAIL()))) )
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"ReferencedTableName": "Announcements", "ReferencedRootTableName": "Announcements", "ReferencedType": "Text", "ReferencedTypeQualifier": " {\"MaxLength\":null,\"MinLength\":null,\"LongTextFormatting\":\"Plain Text\",\"IsMulticolumnKey\":false,\"Valid_If\":null,\"Error_Message_If_Invalid\":null,\"Show_If\":null,\"Required_If\":null,\"Editable_If\":null,\"Reset_If\":null,\"Suggested_Values\":null}", "ReferencedKeyColumn": "ID_ประกาศ", "IsAPartOf": false, "RelationshipName": null, "InputMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 4. วันที่และเวลารับทราบ

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

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MinValue": null, "MaxValue": null, "UseLongDateFormat": false, "IgnoreSeconds": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 5. Email พนักงาน

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

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 6. ชื่อ - นามสกุล

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

**ค่าเริ่มต้น (Initial Value):**

```
=LOOKUP(USEREMAIL(), "ข้อมูลพนักงาน", "Email พนักงาน", "ชื่อ -นามสกุล")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 7. ทะเบียนรถ

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

**ค่าเริ่มต้น (Initial Value):**

```
=LOOKUP(USEREMAIL(), "ข้อมูลพนักงาน", "Email พนักงาน", "ทะเบียนรถ")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 9. หมายเหตุ

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
=OR(

 [เลือกเพื่อยืนยัน] = "ติดขัดปัญหาไม่สามารถปฏิบัติตามได้",

 [ID_ประกาศ].[หัวข้อประกาศ] = "สอบถามและรับฟังความคิด เห็น"

)
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": "=OR(\n\n [เลือกเพื่อยืนยัน] = \"ติดขัดปัญหาไม่สามารถปฏิบัติตามได้\",\n\n [ID_ประกาศ].[หัวข้อประกาศ] = \"สอบถามและรับฟังความคิด เห็น\"\n\n)", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 11. ข้อความประกาศ

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Show |
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
| ข้อมูลอ่อนไหว | No Schema Name Announcements_Schema |
| Locale | en-GB |

**App Formula (สูตรคำนวณ):**

```
=CONCATENATE( "📢 ประกาศ/แจ้งเตือน" "เรื่อง: ", [ID_ประกาศ]. [หัวข้อประกาศ], " ---------------------- ", [ID_ประกาศ].[เนื้อหาประกาศ], " ---------------------- ", [ID_ประกาศ].[Note], )
```

**Show_If (เงื่อนไขการแสดง):**

```
=CONTEXT("ViewType") = "Form"
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"Category": "Page_Header", "Content": "=[ข้อความประกาศ]", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": "=CONTEXT(\"ViewType\") = \"Form\"", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

## คอลัมน์ทั่วไป (ไม่มีสูตรหรือเงื่อนไขพิเศษ)

- **8. เลือกเพื่อยืนยัน** — ชนิด `Enum` (ค่าปกติ)
- **10. ลงชื่อพนักงาน** — ชนิด `Signature` (ค่าปกติ)

