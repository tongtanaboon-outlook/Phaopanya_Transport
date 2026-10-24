# คอลัมน์ของตาราง ไม่ผ่านNew step Output

รวม **136 คอลัมน์** (จาก Schema `ไม่ผ่านNew step Output_Schema`)

| # | ชื่อคอลัมน์ | ชนิด | สถานะ | สูตร/เงื่อนไข |
|---:|---|---|---|---|
| 1 | Instance Id | Text | 🔑 |  |
| 2 | ID_ทำเบิกส่วนต่างScgวังน้อย | Text |  |  |
| 3 | ID_SCGนครหลวงJWDภูมิภาค | Ref |  |  |
| 4 | Shipment No | Number |  | Valid_If |
| 5 | วันที่ส่งสินค้า | Date |  | Valid_If |
| 6 | ชื่อ - นามสกุล | Text |  | Valid_If |
| 7 | ต้นทาง | LatLong |  |  |
| 8 | GoogleMapsRoutesAPI | LongText |  |  |
| 9 | แสดงแผนที่_GoogleMapsRoutesAPI | Url |  |  |
| 10 | ระยะทาง_GoogleMapAPI_Km | Decimal |  |  |
| 11 | Email พนักงาน | Email |  | Valid_If, Editable_If |
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
| 32 | ชื่องาน | Text |  | Valid_If |
| 33 | จำนวนจุดส่งก่อนเริ่มงาน | Number |  |  |
| 34 | จำนวนจุดส่งงานจริง | Number |  |  |
| 35 | ตรวจสอบข้อมูล | Number |  |  |
| 36 | ราคาในระบบก่อนส่งสินค้า | Decimal |  |  |
| 37 | ระยะทางในระบบก่อนส่งสินค้า | Decimal |  |  |
| 38 | สร้างPDFเบิกส่วนต่าง | Yes/No |  | Editable_If |
| 39 | สถานะ | Enum |  | Editable_If |
| 40 | เดือน | Text |  |  |
| 41 | ID_พนักงาน | Ref |  | Editable_If, Show_If |
| 42 | สร้างPDFเบิกตามระยะทาง | Yes/No |  |  |
| 43 | Candidate_2_ระยะทาง_Km | Number |  |  |
| 44 | Candidate_2_แสดงแผนที่ | Url |  |  |
| 45 | Candidate_3_ระยะทาง_Km | Number |  |  |
| 46 | Candidate_3_แสดงแผนที่ | Url |  |  |
| 47 | เรท น้ำมันดีเซล | Decimal |  |  |
| 48 | ราคาตามระยะทาง | Decimal |  |  |
| 49 | ราคาจุดเพิ่ม | Decimal |  |  |
| 50 | ทะเบียนรถ | Text |  |  |
| 51 | 01เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No | LongText |  |  |
| 52 | รูปบิลส่งสินค้า_01 | Image |  |  |
| 53 | รูปหน้าร้าน_บ้าน01 | Image |  |  |
| 54 | รูปส่งสินค้า01 | Image |  |  |
| 55 | 02เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No | LongText |  |  |
| 56 | รูปบิลส่งสินค้า_02 | Image |  |  |
| 57 | รูปหน้าร้าน_บ้าน02 | Image |  |  |
| 58 | รูปส่งสินค้า02 | Image |  |  |
| 59 | 03เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No | LongText |  |  |
| 60 | รูปบิลส่งสินค้า_03 | Image |  |  |
| 61 | รูปหน้าร้าน_บ้าน03 | Image |  |  |
| 62 | รูปส่งสินค้า03 | Image |  |  |
| 63 | 04เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No | LongText |  |  |
| 64 | รูปบิลส่งสินค้า_04 | Image |  |  |
| 65 | รูปหน้าร้าน_บ้าน04 | Image |  |  |
| 66 | รูปส่งสินค้า04 | Image |  |  |
| 67 | 05เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No | LongText |  |  |
| 68 | รูปบิลส่งสินค้า_05 | Image |  |  |
| 69 | รูปหน้าร้าน_บ้าน05 | Image |  |  |
| 70 | รูปส่งสินค้า05 | Image |  |  |
| 71 | 06เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No | LongText |  |  |
| 72 | รูปบิลส่งสินค้า_06 | Image |  |  |
| 73 | รูปหน้าร้าน_บ้าน06 | Image |  |  |
| 74 | รูปส่งสินค้า06 | Image |  |  |
| 75 | 07เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No | LongText |  |  |
| 76 | รูปบิลส่งสินค้า_07 | Image |  |  |
| 77 | รูปหน้าร้าน_บ้าน07 | Image |  |  |
| 78 | รูปส่งสินค้า07 | Image |  |  |
| 79 | 08เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No | LongText |  |  |
| 80 | รูปบิลส่งสินค้า_08 | Image |  |  |
| 81 | รูปหน้าร้าน_บ้าน08 | Image |  |  |
| 82 | รูปส่งสินค้า08 | Image |  |  |
| 83 | 09เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No | LongText |  |  |
| 84 | รูปบิลส่งสินค้า_09 | Image |  |  |
| 85 | รูปหน้าร้าน_บ้าน09 | Image |  |  |
| 86 | รูปส่งสินค้า09 | Image |  |  |
| 87 | 10เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No | LongText |  |  |
| 88 | รูปบิลส่งสินค้า_10 | Image |  |  |
| 89 | รูปหน้าร้าน_บ้าน10 | Image |  |  |
| 90 | รูปส่งสินค้า10 | Image |  |  |
| 91 | 11เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No | LongText |  |  |
| 92 | รูปบิลส่งสินค้า_11 | Image |  |  |
| 93 | รูปหน้าร้าน_บ้าน11 | Image |  |  |
| 94 | รูปส่งสินค้า11 | Image |  |  |
| 95 | 12เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No | LongText |  |  |
| 96 | รูปบิลส่งสินค้า_12 | Image |  |  |
| 97 | รูปหน้าร้าน_บ้าน12 | Image |  |  |
| 98 | รูปส่งสินค้า12 | Image |  |  |
| 99 | 13เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No | LongText |  |  |
| 100 | รูปบิลส่งสินค้า_13 | Image |  |  |
| 101 | รูปหน้าร้าน_บ้าน13 | Image |  |  |
| 102 | รูปส่งสินค้า13 | Image |  |  |
| 103 | 14เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No | LongText |  |  |
| 104 | รูปบิลส่งสินค้า_14 | Image |  |  |
| 105 | รูปหน้าร้าน_บ้าน14 | Image |  |  |
| 106 | รูปส่งสินค้า14 | Image |  |  |
| 107 | 15เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No | LongText |  |  |
| 108 | รูปบิลส่งสินค้า_15 | Image |  |  |
| 109 | รูปหน้าร้าน_บ้าน15 | Image |  |  |
| 110 | รูปส่งสินค้า15 | Image |  |  |
| 111 | 16เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No | LongText |  |  |
| 112 | รูปบิลส่งสินค้า_16 | Image |  |  |
| 113 | รูปหน้าร้าน_บ้าน16 | Image |  |  |
| 114 | รูปส่งสินค้า16 | Image |  |  |
| 115 | 17เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No | LongText |  |  |
| 116 | รูปบิลส่งสินค้า_17 | Image |  |  |
| 117 | รูปหน้าร้าน_บ้าน17 | Image |  |  |
| 118 | รูปส่งสินค้า17 | Image |  |  |
| 119 | 18เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No | LongText |  |  |
| 120 | รูปบิลส่งสินค้า_18 | Image |  |  |
| 121 | รูปหน้าร้าน_บ้าน18 | Image |  |  |
| 122 | รูปส่งสินค้า18 | Image |  |  |
| 123 | 19เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No | LongText |  |  |
| 124 | รูปบิลส่งสินค้า_19 | Image |  |  |
| 125 | รูปหน้าร้าน_บ้าน19 | Image |  |  |
| 126 | รูปส่งสินค้า19 | Image |  |  |
| 127 | 20เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No | LongText |  |  |
| 128 | รูปบิลส่งสินค้า_20 | Image |  |  |
| 129 | รูปหน้าร้าน_บ้าน20 | Image |  |  |
| 130 | รูปส่งสินค้า20 | Image |  |  |
| 131 | ราคาที่สมควรได้ | Decimal |  |  |
| 132 | ราคาหลังส่งสินค้า | Decimal |  |  |
| 133 | ขออนุมัติเบิกค่าขนส่งส่วนเพิ่ม | Decimal |  |  |
| 134 | QR code เส้นทางรวม | Image |  |  |
| 135 | จุดส่งงานลำดับสุดท้าย | LongText |  |  |
| 136 | ชื่อปลายทาง_INV_จุดสุดท้าย | LongText |  |  |

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
| นิยามคงที่ | No |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"MaxLength": null, "MinLength": null, "LongTextFormatting": "Plain Text", "IsMulticolumnKey": false, "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": null, "Reset_If": null, "Suggested_Values": null}
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
| นิยามคงที่ | Yes |
| ค้นหาได้ | No |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

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
| นิยามคงที่ | Yes |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

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
| นิยามคงที่ | Yes |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

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
| นิยามคงที่ | Yes |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

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
| นิยามคงที่ | Yes |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

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
| นิยามคงที่ | Yes |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

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
| นิยามคงที่ | Yes |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

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
| นิยามคงที่ | Yes |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

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
| นิยามคงที่ | Yes |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

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
| นิยามคงที่ | Yes |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

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
| นิยามคงที่ | Yes |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

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
| นิยามคงที่ | Yes |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

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
| นิยามคงที่ | Yes |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

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
| นิยามคงที่ | Yes |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

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
| นิยามคงที่ | Yes |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

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
| นิยามคงที่ | Yes |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

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
| นิยามคงที่ | Yes |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

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
| นิยามคงที่ | Yes |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

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
| นิยามคงที่ | Yes |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

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
| นิยามคงที่ | Yes |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

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
| นิยามคงที่ | Yes |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

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
| นิยามคงที่ | Yes |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

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
| นิยามคงที่ | Yes |
| ค้นหาได้ | No |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

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
| นิยามคงที่ | Yes |
| ค้นหาได้ | Yes |
| สแกนได้ | No |
| ข้อมูลอ่อนไหว | No |

**Editable_If (เงื่อนไขที่แก้ไขได้):**

```
=USERROLE()="ADMIN"
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"EnumValues": ["รอตรวจสอบ", "ผ่านการตรวจสอบ", "ไม่ผ่านการตรวจสอบ"], "AllowOtherValues": false, "AutoCompleteOtherValues": true, "BaseType": "Text", "BaseTypeQualifier": " {\"MaxLength\":null,\"MinLength\":null,\"LongTextFormatting\":\"Plain Text\",\"IsMulticolumnKey\":false,\"Valid_If\":null,\"Error_Message_If_Invalid\":null,\"Show_If\":null,\"Required_If\":null,\"Editable_If\":null,\"Reset_If\":null,\"Suggested_Values\":null}", "EnumInputMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": null, "Required_If": null, "Editable_If": "=USERROLE()=\"ADMIN\"", "Reset_If": null, "Suggested_Values": null}
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
=USERROLE() = "ADMIN"
```

<details><summary>Type Qualifier (JSON เต็ม)</summary>

```json
{"ReferencedTableName": "ข้อมูลพนักงาน", "ReferencedRootTableName": "ข้อมูลพนักงาน", "ReferencedType": "Text", "ReferencedTypeQualifier": " {\"MaxLength\":null,\"MinLength\":null,\"LongTextFormatting\":\"Plain Text\",\"IsMulticolumnKey\":false,\"Valid_If\":null,\"Error_Message_If_Invalid\":null,\"Show_If\":null,\"Required_If\":null,\"Editable_If\":null,\"Reset_If\":null,\"Suggested_Values\":null}", "ReferencedKeyColumn": "ID_พนักงาน", "IsAPartOf": false, "RelationshipName": null, "InputMode": "Auto", "Valid_If": null, "Error_Message_If_Invalid": null, "Show_If": "=USERROLE() = \"ADMIN\"", "Required_If": null, "Editable_If": "=USERROLE() = \"ADMIN\"", "Reset_If": null, "Suggested_Values": null}
```

</details>

## คอลัมน์ทั่วไป (ไม่มีสูตรหรือเงื่อนไขพิเศษ)

- **2. ID_ทำเบิกส่วนต่างScgวังน้อย** — ชนิด `Text` (ค่าปกติ)
- **3. ID_SCGนครหลวงJWDภูมิภาค** — ชนิด `Ref` (ค่าปกติ)
- **7. ต้นทาง** — ชนิด `LatLong` (ค่าปกติ)
- **8. GoogleMapsRoutesAPI** — ชนิด `LongText` (ค่าปกติ)
- **9. แสดงแผนที่_GoogleMapsRoutesAPI** — ชนิด `Url` (ค่าปกติ)
- **10. ระยะทาง_GoogleMapAPI_Km** — ชนิด `Decimal` (ค่าปกติ)
- **33. จำนวนจุดส่งก่อนเริ่มงาน** — ชนิด `Number` (ค่าปกติ)
- **34. จำนวนจุดส่งงานจริง** — ชนิด `Number` (ค่าปกติ)
- **35. ตรวจสอบข้อมูล** — ชนิด `Number` (ค่าปกติ)
- **36. ราคาในระบบก่อนส่งสินค้า** — ชนิด `Decimal` (ค่าปกติ)
- **37. ระยะทางในระบบก่อนส่งสินค้า** — ชนิด `Decimal` (ค่าปกติ)
- **40. เดือน** — ชนิด `Text` (ค่าปกติ)
- **42. สร้างPDFเบิกตามระยะทาง** — ชนิด `Yes/No` (ค่าปกติ)
- **43. Candidate_2_ระยะทาง_Km** — ชนิด `Number` (ค่าปกติ)
- **44. Candidate_2_แสดงแผนที่** — ชนิด `Url` (ค่าปกติ)
- **45. Candidate_3_ระยะทาง_Km** — ชนิด `Number` (ค่าปกติ)
- **46. Candidate_3_แสดงแผนที่** — ชนิด `Url` (ค่าปกติ)
- **47. เรท น้ำมันดีเซล** — ชนิด `Decimal` (ค่าปกติ)
- **48. ราคาตามระยะทาง** — ชนิด `Decimal` (ค่าปกติ)
- **49. ราคาจุดเพิ่ม** — ชนิด `Decimal` (ค่าปกติ)
- **50. ทะเบียนรถ** — ชนิด `Text` (ค่าปกติ)
- **51. 01เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No** — ชนิด `LongText` (ค่าปกติ)
- **52. รูปบิลส่งสินค้า_01** — ชนิด `Image` (ค่าปกติ)
- **53. รูปหน้าร้าน_บ้าน01** — ชนิด `Image` (ค่าปกติ)
- **54. รูปส่งสินค้า01** — ชนิด `Image` (ค่าปกติ)
- **55. 02เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No** — ชนิด `LongText` (ค่าปกติ)
- **56. รูปบิลส่งสินค้า_02** — ชนิด `Image` (ค่าปกติ)
- **57. รูปหน้าร้าน_บ้าน02** — ชนิด `Image` (ค่าปกติ)
- **58. รูปส่งสินค้า02** — ชนิด `Image` (ค่าปกติ)
- **59. 03เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No** — ชนิด `LongText` (ค่าปกติ)
- **60. รูปบิลส่งสินค้า_03** — ชนิด `Image` (ค่าปกติ)
- **61. รูปหน้าร้าน_บ้าน03** — ชนิด `Image` (ค่าปกติ)
- **62. รูปส่งสินค้า03** — ชนิด `Image` (ค่าปกติ)
- **63. 04เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No** — ชนิด `LongText` (ค่าปกติ)
- **64. รูปบิลส่งสินค้า_04** — ชนิด `Image` (ค่าปกติ)
- **65. รูปหน้าร้าน_บ้าน04** — ชนิด `Image` (ค่าปกติ)
- **66. รูปส่งสินค้า04** — ชนิด `Image` (ค่าปกติ)
- **67. 05เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No** — ชนิด `LongText` (ค่าปกติ)
- **68. รูปบิลส่งสินค้า_05** — ชนิด `Image` (ค่าปกติ)
- **69. รูปหน้าร้าน_บ้าน05** — ชนิด `Image` (ค่าปกติ)
- **70. รูปส่งสินค้า05** — ชนิด `Image` (ค่าปกติ)
- **71. 06เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No** — ชนิด `LongText` (ค่าปกติ)
- **72. รูปบิลส่งสินค้า_06** — ชนิด `Image` (ค่าปกติ)
- **73. รูปหน้าร้าน_บ้าน06** — ชนิด `Image` (ค่าปกติ)
- **74. รูปส่งสินค้า06** — ชนิด `Image` (ค่าปกติ)
- **75. 07เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No** — ชนิด `LongText` (ค่าปกติ)
- **76. รูปบิลส่งสินค้า_07** — ชนิด `Image` (ค่าปกติ)
- **77. รูปหน้าร้าน_บ้าน07** — ชนิด `Image` (ค่าปกติ)
- **78. รูปส่งสินค้า07** — ชนิด `Image` (ค่าปกติ)
- **79. 08เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No** — ชนิด `LongText` (ค่าปกติ)
- **80. รูปบิลส่งสินค้า_08** — ชนิด `Image` (ค่าปกติ)
- **81. รูปหน้าร้าน_บ้าน08** — ชนิด `Image` (ค่าปกติ)
- **82. รูปส่งสินค้า08** — ชนิด `Image` (ค่าปกติ)
- **83. 09เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No** — ชนิด `LongText` (ค่าปกติ)
- **84. รูปบิลส่งสินค้า_09** — ชนิด `Image` (ค่าปกติ)
- **85. รูปหน้าร้าน_บ้าน09** — ชนิด `Image` (ค่าปกติ)
- **86. รูปส่งสินค้า09** — ชนิด `Image` (ค่าปกติ)
- **87. 10เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No** — ชนิด `LongText` (ค่าปกติ)
- **88. รูปบิลส่งสินค้า_10** — ชนิด `Image` (ค่าปกติ)
- **89. รูปหน้าร้าน_บ้าน10** — ชนิด `Image` (ค่าปกติ)
- **90. รูปส่งสินค้า10** — ชนิด `Image` (ค่าปกติ)
- **91. 11เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No** — ชนิด `LongText` (ค่าปกติ)
- **92. รูปบิลส่งสินค้า_11** — ชนิด `Image` (ค่าปกติ)
- **93. รูปหน้าร้าน_บ้าน11** — ชนิด `Image` (ค่าปกติ)
- **94. รูปส่งสินค้า11** — ชนิด `Image` (ค่าปกติ)
- **95. 12เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No** — ชนิด `LongText` (ค่าปกติ)
- **96. รูปบิลส่งสินค้า_12** — ชนิด `Image` (ค่าปกติ)
- **97. รูปหน้าร้าน_บ้าน12** — ชนิด `Image` (ค่าปกติ)
- **98. รูปส่งสินค้า12** — ชนิด `Image` (ค่าปกติ)
- **99. 13เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No** — ชนิด `LongText` (ค่าปกติ)
- **100. รูปบิลส่งสินค้า_13** — ชนิด `Image` (ค่าปกติ)
- **101. รูปหน้าร้าน_บ้าน13** — ชนิด `Image` (ค่าปกติ)
- **102. รูปส่งสินค้า13** — ชนิด `Image` (ค่าปกติ)
- **103. 14เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No** — ชนิด `LongText` (ค่าปกติ)
- **104. รูปบิลส่งสินค้า_14** — ชนิด `Image` (ค่าปกติ)
- **105. รูปหน้าร้าน_บ้าน14** — ชนิด `Image` (ค่าปกติ)
- **106. รูปส่งสินค้า14** — ชนิด `Image` (ค่าปกติ)
- **107. 15เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No** — ชนิด `LongText` (ค่าปกติ)
- **108. รูปบิลส่งสินค้า_15** — ชนิด `Image` (ค่าปกติ)
- **109. รูปหน้าร้าน_บ้าน15** — ชนิด `Image` (ค่าปกติ)
- **110. รูปส่งสินค้า15** — ชนิด `Image` (ค่าปกติ)
- **111. 16เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No** — ชนิด `LongText` (ค่าปกติ)
- **112. รูปบิลส่งสินค้า_16** — ชนิด `Image` (ค่าปกติ)
- **113. รูปหน้าร้าน_บ้าน16** — ชนิด `Image` (ค่าปกติ)
- **114. รูปส่งสินค้า16** — ชนิด `Image` (ค่าปกติ)
- **115. 17เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No** — ชนิด `LongText` (ค่าปกติ)
- **116. รูปบิลส่งสินค้า_17** — ชนิด `Image` (ค่าปกติ)
- **117. รูปหน้าร้าน_บ้าน17** — ชนิด `Image` (ค่าปกติ)
- **118. รูปส่งสินค้า17** — ชนิด `Image` (ค่าปกติ)
- **119. 18เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No** — ชนิด `LongText` (ค่าปกติ)
- **120. รูปบิลส่งสินค้า_18** — ชนิด `Image` (ค่าปกติ)
- **121. รูปหน้าร้าน_บ้าน18** — ชนิด `Image` (ค่าปกติ)
- **122. รูปส่งสินค้า18** — ชนิด `Image` (ค่าปกติ)
- **123. 19เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No** — ชนิด `LongText` (ค่าปกติ)
- **124. รูปบิลส่งสินค้า_19** — ชนิด `Image` (ค่าปกติ)
- **125. รูปหน้าร้าน_บ้าน19** — ชนิด `Image` (ค่าปกติ)
- **126. รูปส่งสินค้า19** — ชนิด `Image` (ค่าปกติ)
- **127. 20เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No** — ชนิด `LongText` (ค่าปกติ)
- **128. รูปบิลส่งสินค้า_20** — ชนิด `Image` (ค่าปกติ)
- **129. รูปหน้าร้าน_บ้าน20** — ชนิด `Image` (ค่าปกติ)
- **130. รูปส่งสินค้า20** — ชนิด `Image` (ค่าปกติ)
- **131. ราคาที่สมควรได้** — ชนิด `Decimal` (ค่าปกติ)
- **132. ราคาหลังส่งสินค้า** — ชนิด `Decimal` (ค่าปกติ)
- **133. ขออนุมัติเบิกค่าขนส่งส่วนเพิ่ม** — ชนิด `Decimal` (ค่าปกติ)
- **134. QR code เส้นทางรวม** — ชนิด `Image` (ค่าปกติ)
- **135. จุดส่งงานลำดับสุดท้าย** — ชนิด `LongText` (ค่าปกติ)
- **136. ชื่อปลายทาง_INV_จุดสุดท้าย** — ชนิด `LongText` (ค่าปกติ)

