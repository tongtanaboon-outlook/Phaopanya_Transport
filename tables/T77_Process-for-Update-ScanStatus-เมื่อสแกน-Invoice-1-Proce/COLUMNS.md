# คอลัมน์ของตาราง Process for Update ScanStatus เมื่อสแกน Invoice - 1 Process Table

รวม **19 คอลัมน์** (จาก Schema `Process for Update ScanStatus เมื่อสแกน Invoice - 1 Process Table_Schema`)

| # | ชื่อคอลัมน์ | ชนิด | สถานะ | สูตร/เงื่อนไข |
|---:|---|---|---|---|
| 1 | Instance Id | Text | 🔑 |  |
| 2 | ID_ScanDocs | Text |  |  |
| 3 | Scan_Invoice | Text |  | Valid_If, Show_If |
| 4 | Select_Invoice | Enum |  | Valid_If, Show_If |
| 5 | Scan_DateTime | DateTime |  |  |
| 6 | Scan_By | Email |  |  |
| 7 | Scan_Method | Enum |  | Reset_If |
| 8 | Invoice_No | Ref |  | Valid_If |
| 9 | ชื่อเจ้าของสินค้า | Text |  |  |
| 10 | ทะเบียนรถ | Text |  |  |
| 11 | Shipment No | Text |  |  |
| 12 | วันที่ส่งสินค้า | Date |  |  |
| 13 | หมายเหตุการรับเอกสาร | LongText |  | Show_If |
| 14 | จำนวน_ทั้งหมด | Number |  |  |
| 15 | จำนวน_สแกนแล้ว | Number |  |  |
| 16 | จำนวน_รอสแกน | Number |  |  |
| 17 | สรุปยอด | Text |  |  |
| 18 | เลือกวันที่ | Date |  |  |
| 19 | Update | Ref |  |  |

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
| นิยามคงที่ | Yes |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

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
| นิยามคงที่ | Yes |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

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
| นิยามคงที่ | Yes |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

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
| นิยามคงที่ | Yes |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

- 🔗 **อ้างอิง (Ref) ไปตาราง:** `ตารางงานประจำวัน`

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
| นิยามคงที่ | Yes |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

**Show_If (เงื่อนไขการแสดง):**

```
=ISNOTBLANK([Invoice_No])
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": "=ISNOTBLANK([Invoice_No])", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

## คอลัมน์ทั่วไป (ไม่มีสูตรหรือเงื่อนไขพิเศษ)

- **2. ID_ScanDocs** — ชนิด `Text` (ค่าปกติ)
- **5. Scan_DateTime** — ชนิด `DateTime` (ค่าปกติ)
- **6. Scan_By** — ชนิด `Email` (ค่าปกติ)
- **9. ชื่อเจ้าของสินค้า** — ชนิด `Text` (ค่าปกติ)
- **10. ทะเบียนรถ** — ชนิด `Text` (ค่าปกติ)
- **11. Shipment No** — ชนิด `Text` (ค่าปกติ)
- **12. วันที่ส่งสินค้า** — ชนิด `Date` (ค่าปกติ)
- **14. จำนวน_ทั้งหมด** — ชนิด `Number` (ค่าปกติ)
- **15. จำนวน_สแกนแล้ว** — ชนิด `Number` (ค่าปกติ)
- **16. จำนวน_รอสแกน** — ชนิด `Number` (ค่าปกติ)
- **17. สรุปยอด** — ชนิด `Text` (ค่าปกติ)
- **18. เลือกวันที่** — ชนิด `Date` (ค่าปกติ)
- **19. Update** — ชนิด `Ref` (ค่าปกติ)

