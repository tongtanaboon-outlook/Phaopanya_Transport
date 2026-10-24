# คอลัมน์ของตาราง ScanDocs

รวม **18 คอลัมน์** (จาก Schema `ScanDocs_Schema`)

| # | ชื่อคอลัมน์ | ชนิด | สถานะ | สูตร/เงื่อนไข |
|---:|---|---|---|---|
| 1 | _RowNumber | Number | 🔒 🙈 ⚙️ |  |
| 2 | ID_ScanDocs | Text | 🔑 🏷️ 🔒 | InitValue |
| 3 | Scan_Invoice | Text |  | Valid_If, Show_If |
| 4 | Select_Invoice | Enum |  | Valid_If, Show_If |
| 5 | Scan_DateTime | DateTime |  | InitValue |
| 6 | Scan_By | Email |  | InitValue |
| 7 | Scan_Method | Enum |  | InitValue, Reset_If |
| 8 | Invoice_No | Ref |  | AppFormula, Valid_If |
| 9 | ชื่อเจ้าของสินค้า | Text |  | InitValue |
| 10 | ทะเบียนรถ | Text |  | InitValue |
| 11 | Shipment No | Text |  | InitValue |
| 12 | วันที่ส่งสินค้า | Date |  | InitValue |
| 13 | หมายเหตุการรับเอกสาร | LongText |  | Show_If |
| 14 | จำนวน_ทั้งหมด | Number | 🔒 | AppFormula |
| 15 | จำนวน_สแกนแล้ว | Number | 🔒 | AppFormula |
| 16 | จำนวน_รอสแกน | Number | 🔒 | AppFormula |
| 17 | สรุปยอด | Text | 🔒 | AppFormula |
| 18 | เลือกวันที่ | Date | 🔒 | AppFormula |

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

### 2. ID_ScanDocs

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
UNIQUEID()
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 3. Scan_Invoice

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
| สแกนได้ | Yes |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**Valid_If (เงื่อนไขความถูกต้อง):**

```
=AND(
 IN([_THIS], ตารางงานประจำวัน[Invoice No]),
 LOOKUP([_THIS], "ตารางงาน ประจำวัน", "Invoice No", "Plan Delivery") = [_THISROW].[เลือกวันที่],
 LOOKUP([_THIS], "ตารางงานประจำวัน", "Invoice No", "จำนวน_Invoice_ที่ต้องสแกน") > 0,
 ISBLANK(
 SELECT(ScanDocs[ID_ScanDocs], 
 OR([Scan_Invoice] = [_THIS], [Select_Invoice] = [_THIS])
 )
 )
)
```

**Show_If (เงื่อนไขการแสดง):**

```
=ISBLANK([Select_Invoice])
```

**ข้อความเตือนเมื่อค่าไม่ถูกต้อง:**

```
="Invoice นี้ไม่ถูกต้อง, ไม่ใช่งานวันที่เลือก หรือสแกนรับไป แล้ว"
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": "=AND(\n IN([_THIS], ตารางงานประจำวัน[Invoice No]),\n LOOKUP([_THIS], \"ตารางงาน ประจำวัน\", \"Invoice No\", \"Plan Delivery\") = [_THISROW].[เลือกวันที่],\n LOOKUP([_THIS], \"ตารางงานประจำวัน\", \"Invoice No\", \"จำนวน_Invoice_ที่ต้องสแกน\") > 0,\n ISBLANK(\n SELECT(ScanDocs[ID_ScanDocs], \n OR([Scan_Invoice] = [_THIS], [Select_Invoice] = [_THIS])\n )\n )\n)", "Error_Message_If_Invalid": "=\"Invoice นี้ไม่ถูกต้อง, ไม่ใช่งานวันที่เลือก หรือสแกนรับไป แล้ว\"", "Show_If": "=ISBLANK([Select_Invoice])", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 4. Select_Invoice

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

**Valid_If (เงื่อนไขความถูกต้อง):**

```
=SELECT(
 ตารางงานประจำวัน[Invoice No],
 AND(
 [Plan Delivery] = [_THISROW].[เลือกวันที่],
 OR(ISBLANK([ScanStatus]), [ScanStatus] <> "สแกนรับแล้ว"),
[จำนวน_Invoice_ที่ต้องสแกน] > 0 
 )
)
-ScanDocs[Scan_Invoice]
-ScanDocs[Select_Invoice]
```

**Show_If (เงื่อนไขการแสดง):**

```
=ISBLANK([Scan_Invoice])
```

**ข้อความเตือนเมื่อค่าไม่ถูกต้อง:**

```
="เลข Invoice ไม่ถูกต้อง, ไม่ใช่งานของวันนี้/เมื่อวาน หรือถูกสแกนรับไป แล้ว"
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"EnumValues": [], "AllowOtherValues": true, "AutoCompleteOtherValues": true, "BaseType": "Text", "BaseTypeQualifier": " {\"MaxLength\":null,\"MinLength\":null,\"LongTextFormatting\":\"Plain Text\",\"IsMulticolumnKey\":false,\"Valid_If\":null,\"Error_Message_If_Invalid\":null,\"Show_If\":null,\"Required_If\":null,\"Editable_If\":null,\"Reset_If\":null,\"Suggested_Values\":null}", "EnumInputMode": "Auto", "Valid_If": "=SELECT(\n ตารางงานประจำวัน[Invoice No],\n AND(\n [Plan Delivery] = [_THISROW].[เลือกวันที่],\n OR(ISBLANK([ScanStatus]), [ScanStatus] <> \"สแกนรับแล้ว\"),\n[จำนวน_Invoice_ที่ต้องสแกน] > 0 \n )\n)\n-ScanDocs[Scan_Invoice]\n-ScanDocs[Select_Invoice]", "Error_Message_If_Invalid": "=\"เลข Invoice ไม่ถูกต้อง, ไม่ใช่งานของวันนี้/เมื่อวาน หรือถูกสแกนรับไป แล้ว\"", "Show_If": "=ISBLANK([Scan_Invoice])", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 5. Scan_DateTime

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

### 6. Scan_By

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
| ข้อมูลอ่อนไหว | Yes |
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

### 7. Scan_Method

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Enum |
| Key | No |
| Label | No |
| Virtual | No |
| Read-Only | No |
| Hidden | No |
| รีเซ็ตเมื่อแก้ไข | =ISBLANK([_THIS]) |
| คอลัมน์ระบบ | No |
| ส่วนหนึ่งของ Key | No |
| นิยามคงที่ | No |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**ค่าเริ่มต้น (Initial Value):**

```
=IF(ISNOTBLANK([Select_Invoice]), "Manual", "Barcode")
```

**Reset_If (เงื่อนไขรีเซ็ต):**

```
=ISBLANK([_THIS])
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"EnumValues": ["Barcode", "Manual"], "AllowOtherValues": false, "AutoCompleteOtherValues": true, "BaseType": "Text", "BaseTypeQualifier": " {\"MaxLength\":null,\"MinLength\":null,\"LongTextFormatting\":\"Plain Text\",\"IsMulticolumnKey\":false,\"Valid_If\":null,\"Error_Message_If_Invalid\":null,\"Show_If\":null,\"Required_If\":null,\"Editable_If\":null,\"Reset_If\":null,\"Suggested_Values\":null}", "EnumInputMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": "=ISBLANK([_THIS])", "Suggested_Values": null}
```

</details>

### 8. Invoice_No

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

**App Formula (สูตรคำนวณ):**

```
=ANY( SELECT(ตารางงานประจำวัน[ID_งานประจำวัน], [Invoice No]= IF(ISNOTBLANK([Scan_Invoice]), [Scan_Invoice], [Select_Invoice]) ) )
```

**Valid_If (เงื่อนไขความถูกต้อง):**

```
=AND(
 ISNOTBLANK([_THIS]),
 IN(
 LOOKUP([_THIS], "ตารางงานประจำวัน", "ID_งานประจำวัน", "Plan Delivery"),
 LIST(TODAY(), TODAY() - 1)
 ),
 ISBLANK(
 SELECT(ScanDocs[ID_ScanDocs], 
 AND(
 [Invoice_No] = [_THIS], 
 [ID_ScanDocs] <> [_THISROW]. [ID_ScanDocs]
 )
 )
 )
)
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"ReferencedTableName": "ตารางงานประจำวัน", "ReferencedRootTableName": "ตารางงานประจำวัน", "ReferencedType": "Text", "ReferencedTypeQualifier": " {\"MaxLength\":null,\"MinLength\":null,\"LongTextFormatting\":\"Plain Text\",\"IsMulticolumnKey\":false,\"Valid_If\":null,\"Error_Message_If_Invalid\":null,\"Show_If\":null,\"Required_If\":null,\"Editable_If\":null,\"Reset_If\":null,\"Suggested_Values\":null}", "ReferencedKeyColumn": "ID_งานประจำ วัน", "IsAPartOf": false, "RelationshipName": null, "InputMode": "Auto", "Valid_If": "=AND(\n ISNOTBLANK([_THIS]),\n IN(\n LOOKUP([_THIS], \"ตารางงานประจำวัน\", \"ID_งานประจำวัน\", \"Plan Delivery\"),\n LIST(TODAY(), TODAY() - 1)\n ),\n ISBLANK(\n SELECT(ScanDocs[ID_ScanDocs], \n AND(\n [Invoice_No] = [_THIS], \n [ID_ScanDocs] <> [_THISROW]. [ID_ScanDocs]\n )\n )\n )\n)", "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 9. ชื่อเจ้าของสินค้า

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
=[Invoice_No].[ชื่อเจ้าของสินค้า]
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 10. ทะเบียนรถ

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
=[Invoice_No].[ทะเบียนรถ]
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 11. Shipment No

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
=[Invoice_No].[Shipment No]
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 12. วันที่ส่งสินค้า

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
=[Invoice_No].[Plan Delivery]
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"UseLongDateFormat": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 13. หมายเหตุการรับเอกสาร

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
=ISNOTBLANK([Invoice_No])
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": "=ISNOTBLANK([Invoice_No])", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 14. จำนวน_ทั้งหมด

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
=COUNT( UNIQUE( SELECT( ตารางงานประจำวัน[Invoice No], [Plan Delivery] = [_THISROW].[เลือกวันที่] ) ) )
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxValue": null, "MinValue": null, "StepValue": null, "NumericDigits": null, "ShowThousandsSeparator": true, "NumberDisplayMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 15. จำนวน_สแกนแล้ว

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
=COUNT( UNIQUE( SELECT( ตารางงานประจำวัน[Invoice No], AND( [Plan Delivery] = [_THISROW].[เลือกวันที่], [ScanStatus] = "สแกนรับแล้ว" ) ) ) )
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxValue": null, "MinValue": null, "StepValue": null, "NumericDigits": null, "ShowThousandsSeparator": true, "NumberDisplayMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 16. จำนวน_รอสแกน

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
=[จำนวน_ทั้งหมด] - [จำนวน_สแกนแล้ว]
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxValue": null, "MinValue": null, "StepValue": null, "NumericDigits": null, "ShowThousandsSeparator": true, "NumberDisplayMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 17. สรุปยอด

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
= "📋 " & [จำนวน_ทั้งหมด] & " ✅ " & [จำนวน_สแกนแล้ว] & " ⏳ " & [จำนวน_รอสแกน]
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 18. เลือกวันที่

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Date |
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
| ข้อมูลอ่อนไหว | No Schema Name สรุป_เจ้าของสินค้า_Schema |
| Locale | en-GB |

**App Formula (สูตรคำนวณ):**

```
=IF( TOTALHOURS(NOW() - TODAY()) >= 16, TODAY(), TODAY() -1 )
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"UseLongDateFormat": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

