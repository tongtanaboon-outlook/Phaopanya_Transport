# คอลัมน์ของตาราง ทำเบิกส่วนต่างScgวังน้อย

รวม **136 คอลัมน์** (จาก Schema `ทำเบิกส่วนต่างScgวังน้อย_Schema`)

| # | ชื่อคอลัมน์ | ชนิด | สถานะ | สูตร/เงื่อนไข |
|---:|---|---|---|---|
| 1 | _RowNumber | Number | 🔒 🙈 ⚙️ |  |
| 2 | ID_ทำเบิกส่วนต่างScgวังน้อย | Text | 🔑 🏷️ 🔒 | InitValue |
| 3 | ID_SCGนครหลวงJWDภูมิภาค | Ref | 🔒 | InitValue |
| 4 | Shipment No | Number |  | Valid_If |
| 5 | วันที่ส่งสินค้า | Date | 🔒 | InitValue, Valid_If |
| 6 | ชื่อ - นามสกุล | Text | 🔒 | InitValue, Valid_If |
| 7 | ต้นทาง | LatLong | 🔒 | InitValue |
| 8 | GoogleMapsRoutesAPI | LongText |  |  |
| 9 | แสดงแผนที่_GoogleMapsRoutesAPI | Url |  |  |
| 10 | ระยะทาง_GoogleMapAPI_Km | Decimal |  |  |
| 11 | Email พนักงาน | Email |  | InitValue, Valid_If, Editable_If |
| 12 | Lat/Long_ปลายทาง_01 | Text |  | Valid_If |
| 13 | Lat/Long_ปลายทาง_02 | Text |  | Valid_If, Show_If |
| 14 | Lat/Long_ปลายทาง_03 | Text |  | Valid_If, Show_If |
| 15 | Lat/Long_ปลายทาง_04 | Text |  | Valid_If, Show_If |
| 16 | Lat/Long_ปลายทาง_05 | Text |  | Valid_If, Show_If |
| 17 | Lat/Long_ปลายทาง_06 | Text |  | Valid_If, Show_If |
| 18 | Lat/Long_ปลายทาง_07 | Text |  | Valid_If, Show_If |
| 19 | Lat/Long_ปลายทาง_08 | Text |  | Valid_If, Show_If |
| 20 | Lat/Long_ปลายทาง_09 | Text |  | Valid_If, Show_If |
| 21 | Lat/Long_ปลายทาง_10 | Text |  | Valid_If, Show_If |
| 22 | Lat/Long_ปลายทาง_11 | Text |  | Valid_If, Show_If |
| 23 | Lat/Long_ปลายทาง_12 | Text |  | Valid_If, Show_If |
| 24 | Lat/Long_ปลายทาง_13 | Text |  | Valid_If, Show_If |
| 25 | Lat/Long_ปลายทาง_14 | Text |  | Valid_If, Show_If |
| 26 | Lat/Long_ปลายทาง_15 | Text |  | Valid_If, Show_If |
| 27 | Lat/Long_ปลายทาง_16 | Text |  | Valid_If, Show_If |
| 28 | Lat/Long_ปลายทาง_17 | Text |  | Valid_If, Show_If |
| 29 | Lat/Long_ปลายทาง_18 | Text |  | Valid_If, Show_If |
| 30 | Lat/Long_ปลายทาง_19 | Text |  | Valid_If, Show_If |
| 31 | Lat/Long_ปลายทาง_20 | Text |  | Valid_If, Show_If |
| 32 | ชื่องาน | Text | 🔒 | InitValue, Valid_If |
| 33 | จำนวนจุดส่งก่อนเริ่มงาน | Number | 🔒 | InitValue |
| 34 | จำนวนจุดส่งงานจริง | Number | 🔒 | InitValue |
| 35 | ตรวจสอบข้อมูล | Number |  | AppFormula |
| 36 | ราคาในระบบก่อนส่งสินค้า | Decimal | 🔒 | InitValue |
| 37 | ระยะทางในระบบก่อนส่งสินค้า | Decimal | 🔒 | InitValue |
| 38 | สร้างPDFเบิกส่วนต่าง | Yes/No |  | Editable_If |
| 39 | สถานะ | Enum |  | InitValue, Editable_If |
| 40 | เดือน | Text | 🔒 | InitValue |
| 41 | ID_พนักงาน | Ref |  | InitValue, Editable_If, Show_If |
| 42 | สร้างPDFเบิกตามระยะทาง | Yes/No |  |  |
| 43 | Candidate_2_ระยะทาง_Km | Number |  |  |
| 44 | Candidate_2_แสดงแผนที่ | Url |  |  |
| 45 | Candidate_3_ระยะทาง_Km | Number |  |  |
| 46 | Candidate_3_แสดงแผนที่ | Url |  |  |
| 47 | เรท น้ำมันดีเซล | Decimal | 🔒 | AppFormula |
| 48 | ราคาตามระยะทาง | Decimal | 🔒 | AppFormula |
| 49 | ราคาจุดเพิ่ม | Decimal | 🔒 | AppFormula |
| 50 | ทะเบียนรถ | Text | 🔒 | AppFormula |
| 51 | 01เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No | LongText | 🔒 | AppFormula |
| 52 | รูปบิลส่งสินค้า_01 | Image | 🔒 | AppFormula |
| 53 | รูปหน้าร้าน_บ้าน01 | Image | 🔒 | AppFormula |
| 54 | รูปส่งสินค้า01 | Image | 🔒 | AppFormula |
| 55 | 02เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No | LongText | 🔒 | AppFormula |
| 56 | รูปบิลส่งสินค้า_02 | Image | 🔒 | AppFormula |
| 57 | รูปหน้าร้าน_บ้าน02 | Image | 🔒 | AppFormula |
| 58 | รูปส่งสินค้า02 | Image | 🔒 | AppFormula |
| 59 | 03เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No | LongText | 🔒 | AppFormula |
| 60 | รูปบิลส่งสินค้า_03 | Image | 🔒 | AppFormula |
| 61 | รูปหน้าร้าน_บ้าน03 | Image | 🔒 | AppFormula |
| 62 | รูปส่งสินค้า03 | Image | 🔒 | AppFormula |
| 63 | 04เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No | LongText | 🔒 | AppFormula |
| 64 | รูปบิลส่งสินค้า_04 | Image | 🔒 | AppFormula |
| 65 | รูปหน้าร้าน_บ้าน04 | Image | 🔒 | AppFormula |
| 66 | รูปส่งสินค้า04 | Image | 🔒 | AppFormula |
| 67 | 05เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No | LongText | 🔒 | AppFormula |
| 68 | รูปบิลส่งสินค้า_05 | Image | 🔒 | AppFormula |
| 69 | รูปหน้าร้าน_บ้าน05 | Image | 🔒 | AppFormula |
| 70 | รูปส่งสินค้า05 | Image | 🔒 | AppFormula |
| 71 | 06เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No | LongText | 🔒 | AppFormula |
| 72 | รูปบิลส่งสินค้า_06 | Image | 🔒 | AppFormula |
| 73 | รูปหน้าร้าน_บ้าน06 | Image | 🔒 | AppFormula |
| 74 | รูปส่งสินค้า06 | Image | 🔒 | AppFormula |
| 75 | 07เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No | LongText | 🔒 | AppFormula |
| 76 | รูปบิลส่งสินค้า_07 | Image | 🔒 | AppFormula |
| 77 | รูปหน้าร้าน_บ้าน07 | Image | 🔒 | AppFormula |
| 78 | รูปส่งสินค้า07 | Image | 🔒 | AppFormula |
| 79 | 08เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No | LongText | 🔒 | AppFormula |
| 80 | รูปบิลส่งสินค้า_08 | Image | 🔒 | AppFormula |
| 81 | รูปหน้าร้าน_บ้าน08 | Image | 🔒 | AppFormula |
| 82 | รูปส่งสินค้า08 | Image | 🔒 | AppFormula |
| 83 | 09เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No | LongText | 🔒 | AppFormula |
| 84 | รูปบิลส่งสินค้า_09 | Image | 🔒 | AppFormula |
| 85 | รูปหน้าร้าน_บ้าน09 | Image | 🔒 | AppFormula |
| 86 | รูปส่งสินค้า09 | Image | 🔒 | AppFormula |
| 87 | 10เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No | LongText | 🔒 | AppFormula |
| 88 | รูปบิลส่งสินค้า_10 | Image | 🔒 | AppFormula |
| 89 | รูปหน้าร้าน_บ้าน10 | Image | 🔒 | AppFormula |
| 90 | รูปส่งสินค้า10 | Image | 🔒 | AppFormula |
| 91 | 11เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No | LongText | 🔒 | AppFormula |
| 92 | รูปบิลส่งสินค้า_11 | Image | 🔒 | AppFormula |
| 93 | รูปหน้าร้าน_บ้าน11 | Image | 🔒 | AppFormula |
| 94 | รูปส่งสินค้า11 | Image | 🔒 | AppFormula |
| 95 | 12เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No | LongText | 🔒 | AppFormula |
| 96 | รูปบิลส่งสินค้า_12 | Image | 🔒 | AppFormula |
| 97 | รูปหน้าร้าน_บ้าน12 | Image | 🔒 | AppFormula |
| 98 | รูปส่งสินค้า12 | Image | 🔒 | AppFormula |
| 99 | 13เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No | LongText | 🔒 | AppFormula |
| 100 | รูปบิลส่งสินค้า_13 | Image | 🔒 | AppFormula |
| 101 | รูปหน้าร้าน_บ้าน13 | Image | 🔒 | AppFormula |
| 102 | รูปส่งสินค้า13 | Image | 🔒 | AppFormula |
| 103 | 14เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No | LongText | 🔒 | AppFormula |
| 104 | รูปบิลส่งสินค้า_14 | Image | 🔒 | AppFormula |
| 105 | รูปหน้าร้าน_บ้าน14 | Image | 🔒 | AppFormula |
| 106 | รูปส่งสินค้า14 | Image | 🔒 | AppFormula |
| 107 | 15เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No | LongText | 🔒 | AppFormula |
| 108 | รูปบิลส่งสินค้า_15 | Image | 🔒 | AppFormula |
| 109 | รูปหน้าร้าน_บ้าน15 | Image | 🔒 | AppFormula |
| 110 | รูปส่งสินค้า15 | Image | 🔒 | AppFormula |
| 111 | 16เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No | LongText | 🔒 | AppFormula |
| 112 | รูปบิลส่งสินค้า_16 | Image | 🔒 | AppFormula |
| 113 | รูปหน้าร้าน_บ้าน16 | Image | 🔒 | AppFormula |
| 114 | รูปส่งสินค้า16 | Image | 🔒 | AppFormula |
| 115 | 17เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No | LongText | 🔒 | AppFormula |
| 116 | รูปบิลส่งสินค้า_17 | Image | 🔒 | AppFormula |
| 117 | รูปหน้าร้าน_บ้าน17 | Image | 🔒 | AppFormula |
| 118 | รูปส่งสินค้า17 | Image | 🔒 | AppFormula |
| 119 | 18เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No | LongText | 🔒 | AppFormula |
| 120 | รูปบิลส่งสินค้า_18 | Image | 🔒 | AppFormula |
| 121 | รูปหน้าร้าน_บ้าน18 | Image | 🔒 | AppFormula |
| 122 | รูปส่งสินค้า18 | Image | 🔒 | AppFormula |
| 123 | 19เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No | LongText | 🔒 | AppFormula |
| 124 | รูปบิลส่งสินค้า_19 | Image | 🔒 | AppFormula |
| 125 | รูปหน้าร้าน_บ้าน19 | Image | 🔒 | AppFormula |
| 126 | รูปส่งสินค้า19 | Image | 🔒 | AppFormula |
| 127 | 20เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No | LongText | 🔒 | AppFormula |
| 128 | รูปบิลส่งสินค้า_20 | Image | 🔒 | AppFormula |
| 129 | รูปหน้าร้าน_บ้าน20 | Image | 🔒 | AppFormula |
| 130 | รูปส่งสินค้า20 | Image | 🔒 | AppFormula |
| 131 | ราคาที่สมควรได้ | Decimal | 🔒 | AppFormula |
| 132 | ราคาหลังส่งสินค้า | Decimal | 🔒 | AppFormula |
| 133 | ขออนุมัติเบิกค่าขนส่งส่วนเพิ่ม | Decimal | 🔒 | AppFormula |
| 134 | QR code เส้นทางรวม | Image | 🔒 | AppFormula |
| 135 | จุดส่งงานลำดับสุดท้าย | LongText | 🔒 | AppFormula |
| 136 | ชื่อปลายทาง_INV_จุดสุดท้าย | LongText | 🔒 | AppFormula |

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

### 2. ID_ทำเบิกส่วนต่างScgวังน้อย

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

### 3. ID_SCGนครหลวงJWDภูมิภาค

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

- 🔗 **อ้างอิง (Ref) ไปตาราง:** `SCGนครหลวงJWDภูมิภาค`

**ค่าเริ่มต้น (Initial Value):**

```
=LOOKUP( NUMBER( [_THISROW].[Shipment No]), "SCGนครหลวงJWDภูมิภาค", "Shipment No", "ID_SCGนครหลวงJWDภูมิภาค" )
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"ReferencedTableName": "SCGนครหลวงJWDภูมิภาค", "ReferencedRootTableName": "SCGนครหลวงJWDภูมิภาค", "ReferencedType": "Text", "ReferencedTypeQualifier": " {\"MaxLength\":null,\"MinLength\":null,\"LongTextFormatting\":\"Plain Text\",\"IsMulticolumnKey\":false,\"Valid_If\":null,\"Error_Message_If_Invalid\":null,\"Show_If\":null,\"Required_If\":null,\"Editable_If\":null,\"Reset_If\":null,\"Suggested_Values\":null}", "ReferencedKeyColumn": "ID_SCGนครหลวงJWDภูมิภาค", "IsAPartOf": false, "RelationshipName": null, "InputMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 4. Shipment No

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
 SORT(
 UNIQUE(
 LIST([_THIS]) + 
 SELECT(
 SCGนครหลวงJWDภูมิภาค[Shipment No],
 AND(
 [วันที่ส่งสินค้า]>= EOMONTH(TODAY(), -2) + 1,
 NOT(IN([Shipment No], ทำเบิกส่วนต่างScgวังน้อย[Shipment No]))
 )
 )
 )
 ),
 SORT(
 UNIQUE(
 LIST([_THIS]) + 
 SELECT(
 SCGนครหลวงJWDภูมิภาค[Shipment No],
 AND(
 [Email พนักงาน] = USEREMAIL(),
 [วันที่ส่งสินค้า] >= TODAY() - 1,
 NOT(IN([Shipment No], ทำเบิกส่วนต่างScgวังน้อย[Shipment No]))
 )
 )
 )
 )
)
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxValue": null, "MinValue": null, "StepValue": null, "NumericDigits": null, "ShowThousandsSeparator": false, "NumberDisplayMode": "Auto", "Valid_If": "=IF(USERROLE() = \"ADMIN\",\n SORT(\n UNIQUE(\n LIST([_THIS]) + \n SELECT(\n SCGนครหลวงJWDภูมิภาค[Shipment No],\n AND(\n [วันที่ส่งสินค้า]>= EOMONTH(TODAY(), -2) + 1,\n NOT(IN([Shipment No], ทำเบิกส่วนต่างScgวังน้อย[Shipment No]))\n )\n )\n )\n ),\n SORT(\n UNIQUE(\n LIST([_THIS]) + \n SELECT(\n SCGนครหลวงJWDภูมิภาค[Shipment No],\n AND(\n [Email พนักงาน] = USEREMAIL(),\n [วันที่ส่งสินค้า] >= TODAY() - 1,\n NOT(IN([Shipment No], ทำเบิกส่วนต่างScgวังน้อย[Shipment No]))\n )\n )\n )\n )\n)", "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 5. วันที่ส่งสินค้า

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Date |
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
=[ID_SCGนครหลวงJWDภูมิภาค].[วันที่ส่งสินค้า]
```

**Valid_If (เงื่อนไขความถูกต้อง):**

```
=[ตรวจสอบข้อมูล] =1
```

**ข้อความเตือนเมื่อค่าไม่ถูกต้อง:**

```
="Shipment นี้มีจุดส่งที่ไม่ผ่าน การตรวจสอบ กรุณาติดต่อผู้ดูแล ระบบ"
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"UseLongDateFormat": false, "Valid_If": "=[ตรวจสอบข้อมูล] =1", "Error_Message_If_Invalid": "=\"Shipment นี้มีจุดส่งที่ไม่ผ่าน การตรวจสอบ กรุณาติดต่อผู้ดูแล ระบบ\"", "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
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
=[ID_SCGนครหลวงJWDภูมิภาค].[ชื่อ - นามสกุล]
```

**Valid_If (เงื่อนไขความถูกต้อง):**

```
=[ตรวจสอบข้อมูล] =1
```

**ข้อความเตือนเมื่อค่าไม่ถูกต้อง:**

```
="Shipment นี้มีจุดส่งที่ไม่ผ่าน การตรวจสอบ กรุณาติดต่อผู้ดูแล ระบบ"
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": "=[ตรวจสอบข้อมูล] =1", "Error_Message_If_Invalid": "=\"Shipment นี้มีจุดส่งที่ไม่ผ่าน การตรวจสอบ กรุณาติดต่อผู้ดูแล ระบบ\"", "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 7. ต้นทาง

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
="14.164671, 100.625358"
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"RealTime": false, "PublishIfRowKey": null, "KMLFileUrl": null, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 11. Email พนักงาน

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

**Valid_If (เงื่อนไขความถูกต้อง):**

```
=IF(

 USERROLE() = "ADMIN",

 ข้อมูล พนักงาน[Email พนักงาน],

 LIST(USEREMAIL())

)
```

**Editable_If (เงื่อนไขที่แก้ไขได้):**

```
=USERROLE() = "ADMIN"
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"Valid_If": "=IF(\n\n USERROLE() = \"ADMIN\",\n\n ข้อมูล พนักงาน[Email พนักงาน],\n\n LIST(USEREMAIL())\n\n)", "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": "=USERROLE() = \"ADMIN\"", "Reset_If": null, "Suggested_Values": null}
```

</details>

### 12. Lat/Long_ปลายทาง_01

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
| ค้นหาได้ | No |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**Valid_If (เงื่อนไขความถูกต้อง):**

```
=SELECT(
 SCGนครหลวงJWDภูมิภาค[จุดส่งสินค้าปลายทาง], 
 [Shipment No] = [_THISROW].[Shipment No]
)
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": "=SELECT(\n SCGนครหลวงJWDภูมิภาค[จุดส่งสินค้าปลายทาง], \n [Shipment No] = [_THISROW].[Shipment No]\n)", "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 13. Lat/Long_ปลายทาง_02

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
| ค้นหาได้ | No |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**Valid_If (เงื่อนไขความถูกต้อง):**

```
=SELECT(
 SCGนครหลวงJWDภูมิภาค[จุดส่งสินค้าปลายทาง], 
 AND(
 [Shipment No] = [_THISROW].[Shipment No], 
 NOT(IN([จุดส่งสินค้าปลายทาง], SPLIT(TEXT(
 [_THISROW].[Lat/Long_ปลายทาง_01]
 ), " , "))
 )
))
```

**Show_If (เงื่อนไขการแสดง):**

```
=ISNOTBLANK([Lat/Long_ปลายทาง_01])
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": "=SELECT(\n SCGนครหลวงJWDภูมิภาค[จุดส่งสินค้าปลายทาง], \n AND(\n [Shipment No] = [_THISROW].[Shipment No], \n NOT(IN([จุดส่งสินค้าปลายทาง], SPLIT(TEXT(\n [_THISROW].[Lat/Long_ปลายทาง_01]\n ), \" , \"))\n )\n))", "Error_Message_If_Invalid": null, "Show_If": "=ISNOTBLANK([Lat/Long_ปลายทาง_01])", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 14. Lat/Long_ปลายทาง_03

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
| ค้นหาได้ | No |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**Valid_If (เงื่อนไขความถูกต้อง):**

```
=SELECT(
 SCGนครหลวงJWDภูมิภาค[จุดส่งสินค้าปลายทาง], 
 AND(
 [Shipment No] = [_THISROW].[Shipment No], 
 NOT(IN([จุดส่งสินค้าปลายทาง], SPLIT(TEXT(
 [_THISROW].[Lat/Long_ปลายทาง_01] & " , " & 
 [_THISROW].[Lat/Long_ปลายทาง_02] 
 ), " , "))
 )
))
```

**Show_If (เงื่อนไขการแสดง):**

```
=ISNOTBLANK([Lat/Long_ปลายทาง_02])
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": "=SELECT(\n SCGนครหลวงJWDภูมิภาค[จุดส่งสินค้าปลายทาง], \n AND(\n [Shipment No] = [_THISROW].[Shipment No], \n NOT(IN([จุดส่งสินค้าปลายทาง], SPLIT(TEXT(\n [_THISROW].[Lat/Long_ปลายทาง_01] & \" , \" & \n [_THISROW].[Lat/Long_ปลายทาง_02] \n ), \" , \"))\n )\n))", "Error_Message_If_Invalid": null, "Show_If": "=ISNOTBLANK([Lat/Long_ปลายทาง_02])", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 15. Lat/Long_ปลายทาง_04

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
| ค้นหาได้ | No |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**Valid_If (เงื่อนไขความถูกต้อง):**

```
=SELECT(
 SCGนครหลวงJWDภูมิภาค[จุดส่งสินค้าปลายทาง], 
 AND(
 [Shipment No] = [_THISROW].[Shipment No], 
 NOT(IN([จุดส่งสินค้าปลายทาง], SPLIT(TEXT(
 [_THISROW].[Lat/Long_ปลายทาง_01] & " , " & 
 [_THISROW].[Lat/Long_ปลายทาง_02] & " , " & 
 [_THISROW].[Lat/Long_ปลายทาง_03]
 ), " , "))
 )
))
```

**Show_If (เงื่อนไขการแสดง):**

```
=ISNOTBLANK([Lat/Long_ปลายทาง_03])
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": "=SELECT(\n SCGนครหลวงJWDภูมิภาค[จุดส่งสินค้าปลายทาง], \n AND(\n [Shipment No] = [_THISROW].[Shipment No], \n NOT(IN([จุดส่งสินค้าปลายทาง], SPLIT(TEXT(\n [_THISROW].[Lat/Long_ปลายทาง_01] & \" , \" & \n [_THISROW].[Lat/Long_ปลายทาง_02] & \" , \" & \n [_THISROW].[Lat/Long_ปลายทาง_03]\n ), \" , \"))\n )\n))", "Error_Message_If_Invalid": null, "Show_If": "=ISNOTBLANK([Lat/Long_ปลายทาง_03])", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 16. Lat/Long_ปลายทาง_05

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
| ค้นหาได้ | No |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**Valid_If (เงื่อนไขความถูกต้อง):**

```
=SELECT(
 SCGนครหลวงJWDภูมิภาค[จุดส่งสินค้าปลายทาง], 
 AND(
 [Shipment No] = [_THISROW].[Shipment No], 
 NOT(IN([จุดส่งสินค้าปลายทาง], SPLIT(TEXT(
 [_THISROW].[Lat/Long_ปลายทาง_01] & " , " & 
 [_THISROW].[Lat/Long_ปลายทาง_02] & " , " & 
 [_THISROW].[Lat/Long_ปลายทาง_03] & " , " & 
 [_THISROW].[Lat/Long_ปลายทาง_04]
 ), " , "))
 )
))
```

**Show_If (เงื่อนไขการแสดง):**

```
=ISNOTBLANK([Lat/Long_ปลายทาง_04])
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": "=SELECT(\n SCGนครหลวงJWDภูมิภาค[จุดส่งสินค้าปลายทาง], \n AND(\n [Shipment No] = [_THISROW].[Shipment No], \n NOT(IN([จุดส่งสินค้าปลายทาง], SPLIT(TEXT(\n [_THISROW].[Lat/Long_ปลายทาง_01] & \" , \" & \n [_THISROW].[Lat/Long_ปลายทาง_02] & \" , \" & \n [_THISROW].[Lat/Long_ปลายทาง_03] & \" , \" & \n [_THISROW].[Lat/Long_ปลายทาง_04]\n ), \" , \"))\n )\n))", "Error_Message_If_Invalid": null, "Show_If": "=ISNOTBLANK([Lat/Long_ปลายทาง_04])", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 17. Lat/Long_ปลายทาง_06

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
| ค้นหาได้ | No |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**Valid_If (เงื่อนไขความถูกต้อง):**

```
=SELECT(
 SCGนครหลวงJWDภูมิภาค[จุดส่งสินค้าปลายทาง], 
 AND(
 [Shipment No] = [_THISROW].[Shipment No], 
 NOT(IN([จุดส่งสินค้าปลายทาง], SPLIT(TEXT(
 [_THISROW].[Lat/Long_ปลายทาง_01] & " , " & 
 [_THISROW].[Lat/Long_ปลายทาง_02] & " , " & 
 [_THISROW].[Lat/Long_ปลายทาง_03] & " , " & 
 [_THISROW].[Lat/Long_ปลายทาง_04] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_05]
 ), " , "))
 )
))
```

**Show_If (เงื่อนไขการแสดง):**

```
=ISNOTBLANK([Lat/Long_ปลายทาง_05])
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": "=SELECT(\n SCGนครหลวงJWDภูมิภาค[จุดส่งสินค้าปลายทาง], \n AND(\n [Shipment No] = [_THISROW].[Shipment No], \n NOT(IN([จุดส่งสินค้าปลายทาง], SPLIT(TEXT(\n [_THISROW].[Lat/Long_ปลายทาง_01] & \" , \" & \n [_THISROW].[Lat/Long_ปลายทาง_02] & \" , \" & \n [_THISROW].[Lat/Long_ปลายทาง_03] & \" , \" & \n [_THISROW].[Lat/Long_ปลายทาง_04] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_05]\n ), \" , \"))\n )\n))", "Error_Message_If_Invalid": null, "Show_If": "=ISNOTBLANK([Lat/Long_ปลายทาง_05])", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 18. Lat/Long_ปลายทาง_07

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
| ค้นหาได้ | No |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**Valid_If (เงื่อนไขความถูกต้อง):**

```
=SELECT(
 SCGนครหลวงJWDภูมิภาค[จุดส่งสินค้าปลายทาง], 
 AND(
 [Shipment No] = [_THISROW].[Shipment No], 
 NOT(IN([จุดส่งสินค้าปลายทาง], SPLIT(TEXT(
 [_THISROW].[Lat/Long_ปลายทาง_01] & " , " & 
 [_THISROW].[Lat/Long_ปลายทาง_02] & " , " & 
 [_THISROW].[Lat/Long_ปลายทาง_03] & " , " & 
 [_THISROW].[Lat/Long_ปลายทาง_04] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_05] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_06] 
 ), " , "))
 )
))
```

**Show_If (เงื่อนไขการแสดง):**

```
=ISNOTBLANK([Lat/Long_ปลายทาง_06])
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": "=SELECT(\n SCGนครหลวงJWDภูมิภาค[จุดส่งสินค้าปลายทาง], \n AND(\n [Shipment No] = [_THISROW].[Shipment No], \n NOT(IN([จุดส่งสินค้าปลายทาง], SPLIT(TEXT(\n [_THISROW].[Lat/Long_ปลายทาง_01] & \" , \" & \n [_THISROW].[Lat/Long_ปลายทาง_02] & \" , \" & \n [_THISROW].[Lat/Long_ปลายทาง_03] & \" , \" & \n [_THISROW].[Lat/Long_ปลายทาง_04] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_05] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_06] \n ), \" , \"))\n )\n))", "Error_Message_If_Invalid": null, "Show_If": "=ISNOTBLANK([Lat/Long_ปลายทาง_06])", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 19. Lat/Long_ปลายทาง_08

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
| ค้นหาได้ | No |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**Valid_If (เงื่อนไขความถูกต้อง):**

```
=SELECT(
 SCGนครหลวงJWDภูมิภาค[จุดส่งสินค้าปลายทาง], 
 AND(
 [Shipment No] = [_THISROW].[Shipment No], 
 NOT(IN([จุดส่งสินค้าปลายทาง], SPLIT(TEXT(
 [_THISROW].[Lat/Long_ปลายทาง_01] & " , " & 
 [_THISROW].[Lat/Long_ปลายทาง_02] & " , " & 
 [_THISROW].[Lat/Long_ปลายทาง_03] & " , " & 
 [_THISROW].[Lat/Long_ปลายทาง_04] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_05] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_06] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_07]
 ), " , "))
 )
))
```

**Show_If (เงื่อนไขการแสดง):**

```
=ISNOTBLANK([Lat/Long_ปลายทาง_07])
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": "=SELECT(\n SCGนครหลวงJWDภูมิภาค[จุดส่งสินค้าปลายทาง], \n AND(\n [Shipment No] = [_THISROW].[Shipment No], \n NOT(IN([จุดส่งสินค้าปลายทาง], SPLIT(TEXT(\n [_THISROW].[Lat/Long_ปลายทาง_01] & \" , \" & \n [_THISROW].[Lat/Long_ปลายทาง_02] & \" , \" & \n [_THISROW].[Lat/Long_ปลายทาง_03] & \" , \" & \n [_THISROW].[Lat/Long_ปลายทาง_04] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_05] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_06] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_07]\n ), \" , \"))\n )\n))", "Error_Message_If_Invalid": null, "Show_If": "=ISNOTBLANK([Lat/Long_ปลายทาง_07])", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 20. Lat/Long_ปลายทาง_09

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
| ค้นหาได้ | No |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**Valid_If (เงื่อนไขความถูกต้อง):**

```
=SELECT(
 SCGนครหลวงJWDภูมิภาค[จุดส่งสินค้าปลายทาง], 
 AND(
 [Shipment No] = [_THISROW].[Shipment No], 
 NOT(IN([จุดส่งสินค้าปลายทาง], SPLIT(TEXT(
 [_THISROW].[Lat/Long_ปลายทาง_01] & " , " & 
 [_THISROW].[Lat/Long_ปลายทาง_02] & " , " & 
 [_THISROW].[Lat/Long_ปลายทาง_03] & " , " & 
 [_THISROW].[Lat/Long_ปลายทาง_04] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_05] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_06] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_07] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_08]
 ), " , "))
 )
))
```

**Show_If (เงื่อนไขการแสดง):**

```
=ISNOTBLANK([Lat/Long_ปลายทาง_08])
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": "=SELECT(\n SCGนครหลวงJWDภูมิภาค[จุดส่งสินค้าปลายทาง], \n AND(\n [Shipment No] = [_THISROW].[Shipment No], \n NOT(IN([จุดส่งสินค้าปลายทาง], SPLIT(TEXT(\n [_THISROW].[Lat/Long_ปลายทาง_01] & \" , \" & \n [_THISROW].[Lat/Long_ปลายทาง_02] & \" , \" & \n [_THISROW].[Lat/Long_ปลายทาง_03] & \" , \" & \n [_THISROW].[Lat/Long_ปลายทาง_04] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_05] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_06] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_07] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_08]\n ), \" , \"))\n )\n))", "Error_Message_If_Invalid": null, "Show_If": "=ISNOTBLANK([Lat/Long_ปลายทาง_08])", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 21. Lat/Long_ปลายทาง_10

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
| ค้นหาได้ | No |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**Valid_If (เงื่อนไขความถูกต้อง):**

```
=SELECT(
 SCGนครหลวงJWDภูมิภาค[จุดส่งสินค้าปลายทาง], 
 AND(
 [Shipment No] = [_THISROW].[Shipment No], 
 NOT(IN([จุดส่งสินค้าปลายทาง], SPLIT(TEXT(
 [_THISROW].[Lat/Long_ปลายทาง_01] & " , " & 
 [_THISROW].[Lat/Long_ปลายทาง_02] & " , " & 
 [_THISROW].[Lat/Long_ปลายทาง_03] & " , " & 
 [_THISROW].[Lat/Long_ปลายทาง_04] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_05] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_06] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_07] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_08] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_09] 
 ), " , "))
 )
))
```

**Show_If (เงื่อนไขการแสดง):**

```
=ISNOTBLANK([Lat/Long_ปลายทาง_09])
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": "=SELECT(\n SCGนครหลวงJWDภูมิภาค[จุดส่งสินค้าปลายทาง], \n AND(\n [Shipment No] = [_THISROW].[Shipment No], \n NOT(IN([จุดส่งสินค้าปลายทาง], SPLIT(TEXT(\n [_THISROW].[Lat/Long_ปลายทาง_01] & \" , \" & \n [_THISROW].[Lat/Long_ปลายทาง_02] & \" , \" & \n [_THISROW].[Lat/Long_ปลายทาง_03] & \" , \" & \n [_THISROW].[Lat/Long_ปลายทาง_04] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_05] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_06] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_07] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_08] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_09] \n ), \" , \"))\n )\n))", "Error_Message_If_Invalid": null, "Show_If": "=ISNOTBLANK([Lat/Long_ปลายทาง_09])", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 22. Lat/Long_ปลายทาง_11

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
| ค้นหาได้ | No |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**Valid_If (เงื่อนไขความถูกต้อง):**

```
=SELECT(
 SCGนครหลวงJWDภูมิภาค[จุดส่งสินค้าปลายทาง], 
 AND(
 [Shipment No] = [_THISROW].[Shipment No], 
 NOT(IN([จุดส่งสินค้าปลายทาง], SPLIT(TEXT(
 [_THISROW].[Lat/Long_ปลายทาง_01] & " , " & 
 [_THISROW].[Lat/Long_ปลายทาง_02] & " , " & 
 [_THISROW].[Lat/Long_ปลายทาง_03] & " , " & 
 [_THISROW].[Lat/Long_ปลายทาง_04] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_05] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_06] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_07] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_08] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_09] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_10]
 ), " , "))
 )
))
```

**Show_If (เงื่อนไขการแสดง):**

```
=ISNOTBLANK([Lat/Long_ปลายทาง_10])
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": "=SELECT(\n SCGนครหลวงJWDภูมิภาค[จุดส่งสินค้าปลายทาง], \n AND(\n [Shipment No] = [_THISROW].[Shipment No], \n NOT(IN([จุดส่งสินค้าปลายทาง], SPLIT(TEXT(\n [_THISROW].[Lat/Long_ปลายทาง_01] & \" , \" & \n [_THISROW].[Lat/Long_ปลายทาง_02] & \" , \" & \n [_THISROW].[Lat/Long_ปลายทาง_03] & \" , \" & \n [_THISROW].[Lat/Long_ปลายทาง_04] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_05] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_06] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_07] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_08] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_09] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_10]\n ), \" , \"))\n )\n))", "Error_Message_If_Invalid": null, "Show_If": "=ISNOTBLANK([Lat/Long_ปลายทาง_10])", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 23. Lat/Long_ปลายทาง_12

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
| ค้นหาได้ | No |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**Valid_If (เงื่อนไขความถูกต้อง):**

```
=SELECT(
 SCGนครหลวงJWDภูมิภาค[จุดส่งสินค้าปลายทาง], 
 AND(
 [Shipment No] = [_THISROW].[Shipment No], 
 NOT(IN([จุดส่งสินค้าปลายทาง], SPLIT(TEXT(
 [_THISROW].[Lat/Long_ปลายทาง_01] & " , " & 
 [_THISROW].[Lat/Long_ปลายทาง_02] & " , " & 
 [_THISROW].[Lat/Long_ปลายทาง_03] & " , " & 
 [_THISROW].[Lat/Long_ปลายทาง_04] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_05] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_06] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_07] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_08] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_09] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_10] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_11]
 ), " , "))
 )
))
```

**Show_If (เงื่อนไขการแสดง):**

```
=ISNOTBLANK([Lat/Long_ปลายทาง_11])
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": "=SELECT(\n SCGนครหลวงJWDภูมิภาค[จุดส่งสินค้าปลายทาง], \n AND(\n [Shipment No] = [_THISROW].[Shipment No], \n NOT(IN([จุดส่งสินค้าปลายทาง], SPLIT(TEXT(\n [_THISROW].[Lat/Long_ปลายทาง_01] & \" , \" & \n [_THISROW].[Lat/Long_ปลายทาง_02] & \" , \" & \n [_THISROW].[Lat/Long_ปลายทาง_03] & \" , \" & \n [_THISROW].[Lat/Long_ปลายทาง_04] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_05] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_06] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_07] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_08] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_09] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_10] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_11]\n ), \" , \"))\n )\n))", "Error_Message_If_Invalid": null, "Show_If": "=ISNOTBLANK([Lat/Long_ปลายทาง_11])", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 24. Lat/Long_ปลายทาง_13

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
| ค้นหาได้ | No |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**Valid_If (เงื่อนไขความถูกต้อง):**

```
=SELECT(
 SCGนครหลวงJWDภูมิภาค[จุดส่งสินค้าปลายทาง], 
 AND(
 [Shipment No] = [_THISROW].[Shipment No], 
 NOT(IN([จุดส่งสินค้าปลายทาง], SPLIT(TEXT(
 [_THISROW].[Lat/Long_ปลายทาง_01] & " , " & 
 [_THISROW].[Lat/Long_ปลายทาง_02] & " , " & 
 [_THISROW].[Lat/Long_ปลายทาง_03] & " , " & 
 [_THISROW].[Lat/Long_ปลายทาง_04] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_05] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_06] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_07] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_08] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_09] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_10] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_11] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_12] 
 ), " , "))
 )
))
```

**Show_If (เงื่อนไขการแสดง):**

```
=ISNOTBLANK([Lat/Long_ปลายทาง_12])
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": "=SELECT(\n SCGนครหลวงJWDภูมิภาค[จุดส่งสินค้าปลายทาง], \n AND(\n [Shipment No] = [_THISROW].[Shipment No], \n NOT(IN([จุดส่งสินค้าปลายทาง], SPLIT(TEXT(\n [_THISROW].[Lat/Long_ปลายทาง_01] & \" , \" & \n [_THISROW].[Lat/Long_ปลายทาง_02] & \" , \" & \n [_THISROW].[Lat/Long_ปลายทาง_03] & \" , \" & \n [_THISROW].[Lat/Long_ปลายทาง_04] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_05] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_06] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_07] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_08] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_09] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_10] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_11] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_12] \n ), \" , \"))\n )\n))", "Error_Message_If_Invalid": null, "Show_If": "=ISNOTBLANK([Lat/Long_ปลายทาง_12])", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 25. Lat/Long_ปลายทาง_14

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
| ค้นหาได้ | No |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**Valid_If (เงื่อนไขความถูกต้อง):**

```
=SELECT(
 SCGนครหลวงJWDภูมิภาค[จุดส่งสินค้าปลายทาง], 
 AND(
 [Shipment No] = [_THISROW].[Shipment No], 
 NOT(IN([จุดส่งสินค้าปลายทาง], SPLIT(TEXT(
 [_THISROW].[Lat/Long_ปลายทาง_01] & " , " & 
 [_THISROW].[Lat/Long_ปลายทาง_02] & " , " & 
 [_THISROW].[Lat/Long_ปลายทาง_03] & " , " & 
 [_THISROW].[Lat/Long_ปลายทาง_04] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_05] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_06] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_07] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_08] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_09] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_10] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_11] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_12] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_13] 
 ), " , "))
 )
))
```

**Show_If (เงื่อนไขการแสดง):**

```
=ISNOTBLANK([Lat/Long_ปลายทาง_13])
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": "=SELECT(\n SCGนครหลวงJWDภูมิภาค[จุดส่งสินค้าปลายทาง], \n AND(\n [Shipment No] = [_THISROW].[Shipment No], \n NOT(IN([จุดส่งสินค้าปลายทาง], SPLIT(TEXT(\n [_THISROW].[Lat/Long_ปลายทาง_01] & \" , \" & \n [_THISROW].[Lat/Long_ปลายทาง_02] & \" , \" & \n [_THISROW].[Lat/Long_ปลายทาง_03] & \" , \" & \n [_THISROW].[Lat/Long_ปลายทาง_04] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_05] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_06] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_07] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_08] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_09] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_10] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_11] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_12] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_13] \n ), \" , \"))\n )\n))", "Error_Message_If_Invalid": null, "Show_If": "=ISNOTBLANK([Lat/Long_ปลายทาง_13])", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 26. Lat/Long_ปลายทาง_15

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
| ค้นหาได้ | No |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**Valid_If (เงื่อนไขความถูกต้อง):**

```
=SELECT(
 SCGนครหลวงJWDภูมิภาค[จุดส่งสินค้าปลายทาง], 
 AND(
 [Shipment No] = [_THISROW].[Shipment No], 
 NOT(IN([จุดส่งสินค้าปลายทาง], SPLIT(TEXT(
 [_THISROW].[Lat/Long_ปลายทาง_01] & " , " & 
 [_THISROW].[Lat/Long_ปลายทาง_02] & " , " & 
 [_THISROW].[Lat/Long_ปลายทาง_03] & " , " & 
 [_THISROW].[Lat/Long_ปลายทาง_04] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_05] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_06] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_07] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_08] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_09] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_10] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_11] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_12] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_13] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_14] 
 ), " , "))
 )
))
```

**Show_If (เงื่อนไขการแสดง):**

```
=ISNOTBLANK([Lat/Long_ปลายทาง_14])
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": "=SELECT(\n SCGนครหลวงJWDภูมิภาค[จุดส่งสินค้าปลายทาง], \n AND(\n [Shipment No] = [_THISROW].[Shipment No], \n NOT(IN([จุดส่งสินค้าปลายทาง], SPLIT(TEXT(\n [_THISROW].[Lat/Long_ปลายทาง_01] & \" , \" & \n [_THISROW].[Lat/Long_ปลายทาง_02] & \" , \" & \n [_THISROW].[Lat/Long_ปลายทาง_03] & \" , \" & \n [_THISROW].[Lat/Long_ปลายทาง_04] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_05] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_06] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_07] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_08] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_09] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_10] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_11] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_12] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_13] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_14] \n ), \" , \"))\n )\n))", "Error_Message_If_Invalid": null, "Show_If": "=ISNOTBLANK([Lat/Long_ปลายทาง_14])", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 27. Lat/Long_ปลายทาง_16

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
| ค้นหาได้ | No |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**Valid_If (เงื่อนไขความถูกต้อง):**

```
=SELECT(
 SCGนครหลวงJWDภูมิภาค[จุดส่งสินค้าปลายทาง], 
 AND(
 [Shipment No] = [_THISROW].[Shipment No], 
 NOT(IN([จุดส่งสินค้าปลายทาง], SPLIT(TEXT(
 [_THISROW].[Lat/Long_ปลายทาง_01] & " , " & 
 [_THISROW].[Lat/Long_ปลายทาง_02] & " , " & 
 [_THISROW].[Lat/Long_ปลายทาง_03] & " , " & 
 [_THISROW].[Lat/Long_ปลายทาง_04] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_05] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_06] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_07] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_08] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_09] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_10] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_11] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_12] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_13] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_14] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_15]
 ), " , "))
 )
))
```

**Show_If (เงื่อนไขการแสดง):**

```
=ISNOTBLANK([Lat/Long_ปลายทาง_15])
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": "=SELECT(\n SCGนครหลวงJWDภูมิภาค[จุดส่งสินค้าปลายทาง], \n AND(\n [Shipment No] = [_THISROW].[Shipment No], \n NOT(IN([จุดส่งสินค้าปลายทาง], SPLIT(TEXT(\n [_THISROW].[Lat/Long_ปลายทาง_01] & \" , \" & \n [_THISROW].[Lat/Long_ปลายทาง_02] & \" , \" & \n [_THISROW].[Lat/Long_ปลายทาง_03] & \" , \" & \n [_THISROW].[Lat/Long_ปลายทาง_04] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_05] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_06] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_07] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_08] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_09] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_10] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_11] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_12] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_13] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_14] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_15]\n ), \" , \"))\n )\n))", "Error_Message_If_Invalid": null, "Show_If": "=ISNOTBLANK([Lat/Long_ปลายทาง_15])", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 28. Lat/Long_ปลายทาง_17

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
| ค้นหาได้ | No |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**Valid_If (เงื่อนไขความถูกต้อง):**

```
=SELECT(
 SCGนครหลวงJWDภูมิภาค[จุดส่งสินค้าปลายทาง], 
 AND(
 [Shipment No] = [_THISROW].[Shipment No], 
 NOT(IN([จุดส่งสินค้าปลายทาง], SPLIT(TEXT(
 [_THISROW].[Lat/Long_ปลายทาง_01] & " , " & 
 [_THISROW].[Lat/Long_ปลายทาง_02] & " , " & 
 [_THISROW].[Lat/Long_ปลายทาง_03] & " , " & 
 [_THISROW].[Lat/Long_ปลายทาง_04] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_05] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_06] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_07] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_08] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_09] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_10] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_11] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_12] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_13] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_14] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_15] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_16] 
 ), " , "))
 )
))
```

**Show_If (เงื่อนไขการแสดง):**

```
=ISNOTBLANK([Lat/Long_ปลายทาง_16])
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": "=SELECT(\n SCGนครหลวงJWDภูมิภาค[จุดส่งสินค้าปลายทาง], \n AND(\n [Shipment No] = [_THISROW].[Shipment No], \n NOT(IN([จุดส่งสินค้าปลายทาง], SPLIT(TEXT(\n [_THISROW].[Lat/Long_ปลายทาง_01] & \" , \" & \n [_THISROW].[Lat/Long_ปลายทาง_02] & \" , \" & \n [_THISROW].[Lat/Long_ปลายทาง_03] & \" , \" & \n [_THISROW].[Lat/Long_ปลายทาง_04] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_05] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_06] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_07] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_08] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_09] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_10] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_11] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_12] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_13] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_14] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_15] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_16] \n ), \" , \"))\n )\n))", "Error_Message_If_Invalid": null, "Show_If": "=ISNOTBLANK([Lat/Long_ปลายทาง_16])", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 29. Lat/Long_ปลายทาง_18

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
| ค้นหาได้ | No |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**Valid_If (เงื่อนไขความถูกต้อง):**

```
=SELECT(
 SCGนครหลวงJWDภูมิภาค[จุดส่งสินค้าปลายทาง], 
 AND(
 [Shipment No] = [_THISROW].[Shipment No], 
 NOT(IN([จุดส่งสินค้าปลายทาง], SPLIT(TEXT(
 [_THISROW].[Lat/Long_ปลายทาง_01] & " , " & 
 [_THISROW].[Lat/Long_ปลายทาง_02] & " , " & 
 [_THISROW].[Lat/Long_ปลายทาง_03] & " , " & 
 [_THISROW].[Lat/Long_ปลายทาง_04] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_05] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_06] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_07] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_08] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_09] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_10] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_11] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_12] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_13] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_14] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_15] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_16] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_17] 
 ), " , "))
 )
))
```

**Show_If (เงื่อนไขการแสดง):**

```
=ISNOTBLANK([Lat/Long_ปลายทาง_17])
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": "=SELECT(\n SCGนครหลวงJWDภูมิภาค[จุดส่งสินค้าปลายทาง], \n AND(\n [Shipment No] = [_THISROW].[Shipment No], \n NOT(IN([จุดส่งสินค้าปลายทาง], SPLIT(TEXT(\n [_THISROW].[Lat/Long_ปลายทาง_01] & \" , \" & \n [_THISROW].[Lat/Long_ปลายทาง_02] & \" , \" & \n [_THISROW].[Lat/Long_ปลายทาง_03] & \" , \" & \n [_THISROW].[Lat/Long_ปลายทาง_04] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_05] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_06] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_07] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_08] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_09] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_10] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_11] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_12] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_13] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_14] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_15] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_16] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_17] \n ), \" , \"))\n )\n))", "Error_Message_If_Invalid": null, "Show_If": "=ISNOTBLANK([Lat/Long_ปลายทาง_17])", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 30. Lat/Long_ปลายทาง_19

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
| ค้นหาได้ | No |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**Valid_If (เงื่อนไขความถูกต้อง):**

```
=SELECT(
 SCGนครหลวงJWDภูมิภาค[จุดส่งสินค้าปลายทาง], 
 AND(
 [Shipment No] = [_THISROW].[Shipment No], 
 NOT(IN([จุดส่งสินค้าปลายทาง], SPLIT(TEXT(
 [_THISROW].[Lat/Long_ปลายทาง_01] & " , " & 
 [_THISROW].[Lat/Long_ปลายทาง_02] & " , " & 
 [_THISROW].[Lat/Long_ปลายทาง_03] & " , " & 
 [_THISROW].[Lat/Long_ปลายทาง_04] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_05] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_06] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_07] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_08] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_09] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_10] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_11] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_12] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_13] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_14] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_15] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_16] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_17] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_18]
 ), " , "))
 )
))
```

**Show_If (เงื่อนไขการแสดง):**

```
=ISNOTBLANK([Lat/Long_ปลายทาง_18])
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": "=SELECT(\n SCGนครหลวงJWDภูมิภาค[จุดส่งสินค้าปลายทาง], \n AND(\n [Shipment No] = [_THISROW].[Shipment No], \n NOT(IN([จุดส่งสินค้าปลายทาง], SPLIT(TEXT(\n [_THISROW].[Lat/Long_ปลายทาง_01] & \" , \" & \n [_THISROW].[Lat/Long_ปลายทาง_02] & \" , \" & \n [_THISROW].[Lat/Long_ปลายทาง_03] & \" , \" & \n [_THISROW].[Lat/Long_ปลายทาง_04] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_05] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_06] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_07] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_08] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_09] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_10] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_11] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_12] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_13] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_14] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_15] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_16] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_17] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_18]\n ), \" , \"))\n )\n))", "Error_Message_If_Invalid": null, "Show_If": "=ISNOTBLANK([Lat/Long_ปลายทาง_18])", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 31. Lat/Long_ปลายทาง_20

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
| ค้นหาได้ | No |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**Valid_If (เงื่อนไขความถูกต้อง):**

```
=SELECT(
 SCGนครหลวงJWDภูมิภาค[จุดส่งสินค้าปลายทาง], 
 AND(
 [Shipment No] = [_THISROW].[Shipment No], 
 NOT(IN([จุดส่งสินค้าปลายทาง], SPLIT(TEXT(
 [_THISROW].[Lat/Long_ปลายทาง_01] & " , " & 
 [_THISROW].[Lat/Long_ปลายทาง_02] & " , " & 
 [_THISROW].[Lat/Long_ปลายทาง_03] & " , " & 
 [_THISROW].[Lat/Long_ปลายทาง_04] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_05] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_06] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_07] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_08] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_09] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_10] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_11] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_12] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_13] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_14] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_15] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_16] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_17] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_18] & " , " & 
 [_THISROW]. [Lat/Long_ปลายทาง_19]
 ), " , "))
 )
))
```

**Show_If (เงื่อนไขการแสดง):**

```
=ISNOTBLANK([Lat/Long_ปลายทาง_19])
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": "=SELECT(\n SCGนครหลวงJWDภูมิภาค[จุดส่งสินค้าปลายทาง], \n AND(\n [Shipment No] = [_THISROW].[Shipment No], \n NOT(IN([จุดส่งสินค้าปลายทาง], SPLIT(TEXT(\n [_THISROW].[Lat/Long_ปลายทาง_01] & \" , \" & \n [_THISROW].[Lat/Long_ปลายทาง_02] & \" , \" & \n [_THISROW].[Lat/Long_ปลายทาง_03] & \" , \" & \n [_THISROW].[Lat/Long_ปลายทาง_04] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_05] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_06] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_07] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_08] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_09] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_10] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_11] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_12] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_13] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_14] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_15] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_16] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_17] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_18] & \" , \" & \n [_THISROW]. [Lat/Long_ปลายทาง_19]\n ), \" , \"))\n )\n))", "Error_Message_If_Invalid": null, "Show_If": "=ISNOTBLANK([Lat/Long_ปลายทาง_19])", "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 32. ชื่องาน

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
=IF( IN( LOOKUP([_THISROW].[Shipment No], "ราคาในระบบก่อน ส่งสินค้า", "Shipment No", "Truck Type"), {"นครหลวง", "ภูมิภาค", "04JB_นครหลวง_ภูมิภาค", "Idem_04ID","น้ำมะปี๊ด(ปั้ม บางจาก)FarmZaa"} ), LOOKUP([_THISROW].[Shipment No], "ราคาในระบบก่อนส่งสินค้า", "Shipment No", "Truck Type"), "" )
```

**Valid_If (เงื่อนไขความถูกต้อง):**

```
=[ตรวจสอบข้อมูล] = 1
```

**ข้อความเตือนเมื่อค่าไม่ถูกต้อง:**

```
="Shipment นี้มีจุดส่งที่ไม่ผ่านการตรวจสอบ กรุณาติดต่อผู้ดูแล ระบบ"
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": "=[ตรวจสอบข้อมูล] = 1", "Error_Message_If_Invalid": "=\"Shipment นี้มีจุดส่งที่ไม่ผ่านการตรวจสอบ กรุณาติดต่อผู้ดูแล ระบบ\"", "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 33. จำนวนจุดส่งก่อนเริ่มงาน

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Number |
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
=COUNT( UNIQUE( SELECT( ตารางงานประจำวัน[ชื่อปลายทาง], [Shipment No] = [_THISROW].[Shipment No] ) ) )
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxValue": null, "MinValue": null, "StepValue": null, "NumericDigits": null, "ShowThousandsSeparator": true, "NumberDisplayMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 34. จำนวนจุดส่งงานจริง

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Number |
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
=COUNT( SELECT( SCGนครหลวงJWDภูมิภาค[Shipment No], [Shipment No] = [_THISROW].[Shipment No]) )
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxValue": null, "MinValue": null, "StepValue": null, "NumericDigits": null, "ShowThousandsSeparator": false, "NumberDisplayMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 35. ตรวจสอบข้อมูล

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
| ค้นหาได้ | No |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |
| Locale | en-GB |

**App Formula (สูตรคำนวณ):**

```
=IF( AND( ISNOTBLANK([ชื่องาน]), COUNT( SELECT( SCGนครหลวงJWDภูมิภาค[Shipment No], [Shipment No] = [_THISROW].[Shipment No] ) ) > 0, COUNT( SELECT( SCGนครหลวงJWDภูมิภาค[Shipment No], [Shipment No] = [_THISROW].[Shipment No] ) ) = COUNT( SELECT( SCGนครหลวงJWDภูมิภาค[Shipment No], AND( [Shipment No] = [_THISROW].[Shipment No], ISNOTBLANK([ชื่องาน]), [LAT] <> "0.000000", [LONG] <> "0.000000", ISNOTBLANK([จุดส่งสินค้าปลายทาง]), [ระยะทางจากคลัง_Km] > 0 ) ) ), COUNT( SELECT( SCGนครหลวงJWDภูมิภาค[Shipment No], AND( [Shipment No] = [_THISROW].[Shipment No], [ผลการตรวจสอบงานส่ง] = "FAIL" ) ) )= 0 ), 1, 0 )
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxValue": null, "MinValue": null, "StepValue": null, "NumericDigits": null, "ShowThousandsSeparator": true, "NumberDisplayMode": "Auto", "Valid_If": "", "Error_Message_If_Invalid": "", "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 36. ราคาในระบบก่อนส่งสินค้า

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
=LOOKUP([_THISROW].[Shipment No],"ราคาในระบบก่อนส่ง สินค้า","Shipment No","ราคา")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxValue": null, "MinValue": null, "StepValue": null, "DecimalDigits": 2, "NumericDigits": null, "ShowThousandsSeparator": true, "NumberDisplayMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 37. ระยะทางในระบบก่อนส่งสินค้า

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
=LOOKUP([_THISROW].[Shipment No],"ราคาในระบบก่อนส่ง สินค้า","Shipment No","ระยะทาง (km)")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxValue": null, "MinValue": null, "StepValue": null, "DecimalDigits": 2, "NumericDigits": null, "ShowThousandsSeparator": false, "NumberDisplayMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 38. สร้างPDFเบิกส่วนต่าง

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
=USERROLE()="ADMIN"
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"YesLabel": "", "NoLabel": "", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": "=USERROLE()=\"ADMIN\"", "Reset_If": null, "Suggested_Values": null}
```

</details>

### 39. สถานะ

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
="รอตรวจสอบ"
```

**Editable_If (เงื่อนไขที่แก้ไขได้):**

```
=USERROLE()="ADMIN"
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"EnumValues": ["รอตรวจสอบ", "ผ่านการตรวจสอบ", "ไม่ผ่านการตรวจสอบ"], "AllowOtherValues": false, "AutoCompleteOtherValues": true, "BaseType": "Text", "BaseTypeQualifier": " {\"MaxLength\":null,\"MinLength\":null,\"LongTextFormatting\":\"Plain Text\",\"IsMulticolumnKey\":false,\"Valid_If\":null,\"Error_Message_If_Invalid\":null,\"Show_If\":null,\"Required_If\":null,\"Editable_If\":null,\"Reset_If\":null,\"Suggested_Values\":null}", "EnumInputMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": "=USERROLE()=\"ADMIN\"", "Reset_If": null, "Suggested_Values": null}
```

</details>

### 40. เดือน

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

### 41. ID_พนักงาน

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
=USERROLE() = "ADMIN"
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"ReferencedTableName": "ข้อมูลพนักงาน", "ReferencedRootTableName": "ข้อมูลพนักงาน", "ReferencedType": "Text", "ReferencedTypeQualifier": " {\"MaxLength\":null,\"MinLength\":null,\"LongTextFormatting\":\"Plain Text\",\"IsMulticolumnKey\":false,\"Valid_If\":null,\"Error_Message_If_Invalid\":null,\"Show_If\":null,\"Required_If\":null,\"Editable_If\":null,\"Reset_If\":null,\"Suggested_Values\":null}", "ReferencedKeyColumn": "ID_พนักงาน", "IsAPartOf": false, "RelationshipName": null, "InputMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": "=USERROLE() = \"ADMIN\"", "Required_If": null, "Editable_If": "=USERROLE() = \"ADMIN\"", "Reset_If": null, "Suggested_Values": null}
```

</details>

### 47. เรท น้ำมันดีเซล

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Decimal |
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
=IF( ISBLANK([_THISROW].[วันที่ส่งสินค้า]), "", IF( ISNOTBLANK( ANY( SELECT( PriceOverride[UsePriceDate], AND( [StartDate] <= [_THISROW].[วันที่ส่งสินค้า], [EndDate] >= [_THISROW].[วันที่ส่งสินค้า], [JobName] = [_THISROW].[ชื่องาน] ) ) ) ), ANY( SELECT( ราคาน้ำมันดีเซล[ราคา/หน่วย], [วันที่] = ANY( SELECT( PriceOverride[UsePriceDate], AND( [StartDate] <= [_THISROW]. [วันที่ส่งสินค้า], [EndDate] >= [_THISROW].[วันที่ส่งสินค้า], [JobName] = [_THISROW].[ชื่องาน] ) ) ) ) ), IF( ISNOTBLANK( ANY( SELECT( PriceOverride[UsePriceDate], AND( [StartDate] <= [_THISROW].[วันที่ส่งสินค้า], [EndDate] >= [_THISROW].[วันที่ส่งสินค้า], ISBLANK([JobName]) ) ) ) ), ANY( SELECT( ราคาน้ำมัน ดีเซล[ราคา/หน่วย], [วันที่] = ANY( SELECT( PriceOverride[UsePriceDate], AND( [StartDate] <= [_THISROW]. [วันที่ส่งสินค้า], [EndDate] >= [_THISROW].[วันที่ส่งสินค้า], ISBLANK([JobName]) ) ) ) ) ), ANY( SELECT( ราคาน้ำมัน ดีเซล[ราคา/หน่วย], [วันที่] = DATE( CONCATENATE( YEAR(EOMONTH([_THISROW].[วันที่ส่งสินค้า], -1)), "-", RIGHT("0" & MONTH(EOMONTH([_THISROW].[วันที่ส่งสินค้า], -1)), 2), "-25" )) ) ) ) ) )
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxValue": null, "MinValue": null, "StepValue": null, "DecimalDigits": 2, "NumericDigits": null, "ShowThousandsSeparator": true, "NumberDisplayMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 48. ราคาตามระยะทาง

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Decimal |
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
=IF( ISNOTBLANK( ANY( SELECT( Price_Table[Price], AND( IN([_THISROW].[ชื่องาน], SPLIT([ชื่องาน], ",")), [เรทน้ำมัน_Minimum] <= [_THISROW].[เรท น้ำมันดีเซล], [เรทน้ำมัน_Maximum] >= [_THISROW].[เรท น้ำมันดีเซล], [ระยะทาง_Minimum] <= NUMBER([_THISROW].[ระยะทาง_GoogleMapAPI_Km]), [ระยะทาง_Maximum] >= NUMBER([_THISROW].[ระยะทาง_GoogleMapAPI_Km]) ) ) ) ), ANY( SELECT( Price_Table[Price], AND( IN([_THISROW].[ชื่องาน],SPLIT([ชื่องาน], ",")), [เรทน้ำมัน_Minimum] <= [_THISROW].[เรท น้ำมันดีเซล], [เรทน้ำมัน_Maximum] >= [_THISROW].[เรท น้ำมันดีเซล], [ระยะทาง_Minimum] <= NUMBER([_THISROW].[ระยะทาง_GoogleMapAPI_Km]), [ระยะทาง_Maximum] >= NUMBER([_THISROW].[ระยะทาง_GoogleMapAPI_Km]) ) ) ), 0 )
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxValue": null, "MinValue": null, "StepValue": null, "DecimalDigits": 2, "NumericDigits": null, "ShowThousandsSeparator": true, "NumberDisplayMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 49. ราคาจุดเพิ่ม

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Decimal |
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
=IF( AND( [ชื่องาน] = "Idem_04ID", ISNOTBLANK([จำนวนจุดส่งงานจริง]), [จำนวนจุดส่งงานจริง] > 11 ), ([จำนวนจุดส่งงานจริง] - 11) * 50, IF( AND( IN( [ชื่องาน], {"นครหลวง", "ภูมิภาค", "04JB_นครหลวง_ภูมิภาค"} ), ISNOTBLANK([จำนวนจุดส่งงานจริง]),[จำนวนจุดส่งงานจริง] > 10 ), ([จำนวนจุดส่งงานจริง] - 10) * 50, 0 ) )
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxValue": null, "MinValue": null, "StepValue": null, "DecimalDigits": 2, "NumericDigits": null, "ShowThousandsSeparator": true, "NumberDisplayMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 50. ทะเบียนรถ

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
=[ID_SCGนครหลวงJWDภูมิภาค].[ทะเบียนรถ]
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 51. 01เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No

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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_01],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลาย ทาง","เจ้าของสินค้า//ชื่อปลายทาง//Lat_Long//Inv No")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 52. รูปบิลส่งสินค้า_01

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_01],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูปถ่ายบิลส่งสินค้า")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 53. รูปหน้าร้าน_บ้าน01

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_01],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูปหน้าร้าน / บ้าน")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 54. รูปส่งสินค้า01

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_01],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูป สินค้าตอนส่ง")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 55. 02เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No

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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_02],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลาย ทาง","เจ้าของสินค้า//ชื่อปลายทาง//Lat_Long//Inv No")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 56. รูปบิลส่งสินค้า_02

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_02],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูปถ่ายบิลส่งสินค้า")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 57. รูปหน้าร้าน_บ้าน02

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_02],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูปหน้าร้าน / บ้าน")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 58. รูปส่งสินค้า02

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_02],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูป สินค้าตอนส่ง")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 59. 03เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No

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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_03],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลาย ทาง","เจ้าของสินค้า//ชื่อปลายทาง//Lat_Long//Inv No")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 60. รูปบิลส่งสินค้า_03

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_03],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูปถ่ายบิลส่งสินค้า")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 61. รูปหน้าร้าน_บ้าน03

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_03],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูปหน้าร้าน / บ้าน")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 62. รูปส่งสินค้า03

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_03],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูป สินค้าตอนส่ง")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 63. 04เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No

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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_04],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลาย ทาง","เจ้าของสินค้า//ชื่อปลายทาง//Lat_Long//Inv No")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 64. รูปบิลส่งสินค้า_04

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_04],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูปถ่ายบิลส่งสินค้า")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 65. รูปหน้าร้าน_บ้าน04

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_04],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูปหน้าร้าน / บ้าน")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 66. รูปส่งสินค้า04

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_04],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูป สินค้าตอนส่ง")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 67. 05เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No

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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_05],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลาย ทาง","เจ้าของสินค้า//ชื่อปลายทาง//Lat_Long//Inv No")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 68. รูปบิลส่งสินค้า_05

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_05],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูปถ่ายบิลส่งสินค้า")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 69. รูปหน้าร้าน_บ้าน05

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_05],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูปหน้าร้าน / บ้าน")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 70. รูปส่งสินค้า05

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_05],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูป สินค้าตอนส่ง")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 71. 06เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No

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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_06],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลาย ทาง","เจ้าของสินค้า//ชื่อปลายทาง//Lat_Long//Inv No")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 72. รูปบิลส่งสินค้า_06

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_06],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูปถ่ายบิลส่งสินค้า")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 73. รูปหน้าร้าน_บ้าน06

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_06],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูปหน้าร้าน / บ้าน")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 74. รูปส่งสินค้า06

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_06],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูป สินค้าตอนส่ง")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 75. 07เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No

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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_07],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลาย ทาง","เจ้าของสินค้า//ชื่อปลายทาง//Lat_Long//Inv No")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 76. รูปบิลส่งสินค้า_07

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_07],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูปถ่ายบิลส่งสินค้า")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 77. รูปหน้าร้าน_บ้าน07

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_07],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูปหน้าร้าน / บ้าน")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 78. รูปส่งสินค้า07

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_07],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูป สินค้าตอนส่ง")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 79. 08เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No

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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_08],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลาย ทาง","เจ้าของสินค้า//ชื่อปลายทาง//Lat_Long//Inv No")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 80. รูปบิลส่งสินค้า_08

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_08],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูปถ่ายบิลส่งสินค้า")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 81. รูปหน้าร้าน_บ้าน08

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_08],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูปหน้าร้าน / บ้าน")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 82. รูปส่งสินค้า08

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_08],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูป สินค้าตอนส่ง")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 83. 09เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No

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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_09],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลาย ทาง","เจ้าของสินค้า//ชื่อปลายทาง//Lat_Long//Inv No")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 84. รูปบิลส่งสินค้า_09

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_09],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูปถ่ายบิลส่งสินค้า")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 85. รูปหน้าร้าน_บ้าน09

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_09],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูปหน้าร้าน / บ้าน")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 86. รูปส่งสินค้า09

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_09],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูป สินค้าตอนส่ง")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 87. 10เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No

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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_10],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลาย ทาง","เจ้าของสินค้า//ชื่อปลายทาง//Lat_Long//Inv No")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 88. รูปบิลส่งสินค้า_10

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_10],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูปถ่ายบิลส่งสินค้า")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 89. รูปหน้าร้าน_บ้าน10

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_10],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูปหน้าร้าน / บ้าน")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 90. รูปส่งสินค้า10

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_10],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูป สินค้าตอนส่ง")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 91. 11เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No

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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_11],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลาย ทาง","เจ้าของสินค้า//ชื่อปลายทาง//Lat_Long//Inv No")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 92. รูปบิลส่งสินค้า_11

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_11],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูปถ่ายบิลส่งสินค้า")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 93. รูปหน้าร้าน_บ้าน11

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_11],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูปหน้าร้าน / บ้าน")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 94. รูปส่งสินค้า11

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_11],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูป สินค้าตอนส่ง")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 95. 12เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No

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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_12],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลาย ทาง","เจ้าของสินค้า//ชื่อปลายทาง//Lat_Long//Inv No")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 96. รูปบิลส่งสินค้า_12

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_12],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูปถ่ายบิลส่งสินค้า")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 97. รูปหน้าร้าน_บ้าน12

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_12],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูปหน้าร้าน / บ้าน")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 98. รูปส่งสินค้า12

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_12],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูป สินค้าตอนส่ง")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 99. 13เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No

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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_13],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลาย ทาง","เจ้าของสินค้า//ชื่อปลายทาง//Lat_Long//Inv No")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 100. รูปบิลส่งสินค้า_13

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_13],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูปถ่ายบิลส่งสินค้า")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 101. รูปหน้าร้าน_บ้าน13

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_13],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูปหน้าร้าน / บ้าน")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 102. รูปส่งสินค้า13

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_13],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูป สินค้าตอนส่ง")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 103. 14เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No

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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_14],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลาย ทาง","เจ้าของสินค้า//ชื่อปลายทาง//Lat_Long//Inv No")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 104. รูปบิลส่งสินค้า_14

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_14],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูปถ่ายบิลส่งสินค้า")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 105. รูปหน้าร้าน_บ้าน14

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_14],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูปหน้าร้าน / บ้าน")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 106. รูปส่งสินค้า14

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_14],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูป สินค้าตอนส่ง")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 107. 15เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No

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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_15],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลาย ทาง","เจ้าของสินค้า//ชื่อปลายทาง//Lat_Long//Inv No")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 108. รูปบิลส่งสินค้า_15

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_15],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูปถ่ายบิลส่งสินค้า")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 109. รูปหน้าร้าน_บ้าน15

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_15],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูปหน้าร้าน / บ้าน")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 110. รูปส่งสินค้า15

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_15],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูป สินค้าตอนส่ง")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 111. 16เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No

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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_16],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลาย ทาง","เจ้าของสินค้า//ชื่อปลายทาง//Lat_Long//Inv No")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 112. รูปบิลส่งสินค้า_16

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_16],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูปถ่ายบิลส่งสินค้า")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 113. รูปหน้าร้าน_บ้าน16

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_16],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูปหน้าร้าน / บ้าน")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 114. รูปส่งสินค้า16

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_16],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูป สินค้าตอนส่ง")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 115. 17เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No

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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_17],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลาย ทาง","เจ้าของสินค้า//ชื่อปลายทาง//Lat_Long//Inv No")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 116. รูปบิลส่งสินค้า_17

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_17],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูปถ่ายบิลส่งสินค้า")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 117. รูปหน้าร้าน_บ้าน17

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_17],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูปหน้าร้าน / บ้าน")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 118. รูปส่งสินค้า17

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_17],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูป สินค้าตอนส่ง")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 119. 18เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No

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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_18],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลาย ทาง","เจ้าของสินค้า//ชื่อปลายทาง//Lat_Long//Inv No")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 120. รูปบิลส่งสินค้า_18

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_18],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูปถ่ายบิลส่งสินค้า")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 121. รูปหน้าร้าน_บ้าน18

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_18],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูปหน้าร้าน / บ้าน")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 122. รูปส่งสินค้า18

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_18],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูป สินค้าตอนส่ง")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 123. 19เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No

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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_19],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลาย ทาง","เจ้าของสินค้า//ชื่อปลายทาง//Lat_Long//Inv No")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 124. รูปบิลส่งสินค้า_19

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_19],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูปถ่ายบิลส่งสินค้า")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 125. รูปหน้าร้าน_บ้าน19

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_19],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูปหน้าร้าน / บ้าน")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 126. รูปส่งสินค้า19

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_19],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูป สินค้าตอนส่ง")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 127. 20เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No

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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_20],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลาย ทาง","เจ้าของสินค้า//ชื่อปลายทาง//Lat_Long//Inv No")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 128. รูปบิลส่งสินค้า_20

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_20],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูปถ่ายบิลส่งสินค้า")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 129. รูปหน้าร้าน_บ้าน20

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_20],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูปหน้าร้าน / บ้าน")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 130. รูปส่งสินค้า20

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=LOOKUP([_THISROW].[Lat/Long_ปลายทาง_20],"SCGนครหลวงJWDภูมิภาค","จุดส่งสินค้าปลายทาง","รูป สินค้าตอนส่ง")
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 131. ราคาที่สมควรได้

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Decimal |
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
=[ราคาตามระยะทาง]+[ราคาจุดเพิ่ม]
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxValue": null, "MinValue": null, "StepValue": null, "DecimalDigits": 2, "NumericDigits": null, "ShowThousandsSeparator": true, "NumberDisplayMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 132. ราคาหลังส่งสินค้า

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Decimal |
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
=IF( ISNOTBLANK( LOOKUP([_THISROW].[Shipment No], "ราคา ในระบบก่อนส่งสินค้า", "Shipment No", "ราคาหลังส่งสินค้า") ), LOOKUP([_THISROW].[Shipment No], "ราคาในระบบก่อนส่งสินค้า","Shipment No", "ราคาหลังส่งสินค้า"), 0 )
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxValue": null, "MinValue": null, "StepValue": null, "DecimalDigits": 2, "NumericDigits": null, "ShowThousandsSeparator": true, "NumberDisplayMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 133. ขออนุมัติเบิกค่าขนส่งส่วนเพิ่ม

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Decimal |
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
=IF( AND( ISNOTBLANK([ราคาที่สมควรได้]), ISNOTBLANK([ราคาหลังส่งสินค้า]) ), [ราคาที่สมควรได้] - [ราคาหลังส่งสินค้า], 0 )
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxValue": null, "MinValue": null, "StepValue": null, "DecimalDigits": 2, "NumericDigits": null, "ShowThousandsSeparator": true, "NumberDisplayMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 134. QR code เส้นทางรวม

| คุณสมบัติ | ค่า |
|---|---|
| ชนิดข้อมูล | Image |
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
=CONCATENATE( "https://api.qrserver.com/v1/create-qr-code/? size=150x150&data=",ENCODEURL(CONCATENATE([แสดงแผนที่_GoogleMapsRoutesAPI] )))
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"AllowDrawing": false, "FolderLocation": null, "Valid_If": null, "Error_ Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 135. จุดส่งงานลำดับสุดท้าย

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
=IF( ISNOTBLANK([20เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No]), [20เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No], IF( ISNOTBLANK([19เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No]), [19เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No], IF( ISNOTBLANK([18เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No]), [18เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No], IF( ISNOTBLANK([17เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No]), [17เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No], IF( ISNOTBLANK([16เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No]), [16เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No], IF( ISNOTBLANK([15เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No]), [15เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No], IF( ISNOTBLANK([14เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No]), [14เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No], IF( ISNOTBLANK([13เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No]), [13เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No], IF( ISNOTBLANK([12เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No]), [12เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No], IF( ISNOTBLANK([11เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No]), [11เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No], IF( ISNOTBLANK([10เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No]), [10เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No], IF( ISNOTBLANK([09เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No]), [09เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No], IF( ISNOTBLANK([08เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No]), [08เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No], IF( ISNOTBLANK([07เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No]), [07เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No], IF( ISNOTBLANK([06เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No]), [06เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No], IF( ISNOTBLANK([05เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No]), [05เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No], IF( ISNOTBLANK([04เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No]), [04เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No], IF( ISNOTBLANK([03เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No]), [03เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No], IF( ISNOTBLANK([02เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No]), [02เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No], [01เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No] ) ) ) ) ) ) ) )) ) ) ) ) ) ) ) ) ) )
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

### 136. ชื่อปลายทาง_INV_จุดสุดท้าย

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
| ข้อมูลอ่อนไหว | No Schema Name ข้อมูลงานRW_Schema |
| Locale | en-GB |

**App Formula (สูตรคำนวณ):**

```
=CONCATENATE( ปลายทาง , MID( [จุดส่งงานลำดับสุดท้าย], FIND("ปลายทาง ", [จุดส่งงานลำดับสุดท้าย]) + LEN("ปลายทาง "), FIND("Lat/Lng", [จุดส่งงานลำดับสุดท้าย]) - FIND("ปลายทาง ", [จุดส่งงานลำดับสุดท้าย]) - LEN("ปลายทาง ") ), INV: , TRIM( MID( [จุดส่งงานลำดับสุดท้าย], FIND("INV.", [จุดส่งงานลำดับสุดท้าย]) + 5, LEN([จุดส่งงานลำดับสุดท้าย]) ) ) )
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
```

</details>

## คอลัมน์ทั่วไป (ไม่มีสูตรหรือเงื่อนไขพิเศษ)

- **8. GoogleMapsRoutesAPI** — ชนิด `LongText` (ค่าปกติ)
- **9. แสดงแผนที่_GoogleMapsRoutesAPI** — ชนิด `Url` (ค่าปกติ)
- **10. ระยะทาง_GoogleMapAPI_Km** — ชนิด `Decimal` (ค่าปกติ)
- **42. สร้างPDFเบิกตามระยะทาง** — ชนิด `Yes/No` (ค่าปกติ)
- **43. Candidate_2_ระยะทาง_Km** — ชนิด `Number` (ค่าปกติ)
- **44. Candidate_2_แสดงแผนที่** — ชนิด `Url` (ค่าปกติ)
- **45. Candidate_3_ระยะทาง_Km** — ชนิด `Number` (ค่าปกติ)
- **46. Candidate_3_แสดงแผนที่** — ชนิด `Url` (ค่าปกติ)

