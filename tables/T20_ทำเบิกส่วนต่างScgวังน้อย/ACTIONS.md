# Actions ของตาราง ทำเบิกส่วนต่างScgวังน้อย

รวม **15 actions**

## Delete

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | DELETE_RECORD |
| การแสดงผล | Display_Prominently |
| ลำดับ | 1 |
| Bulk action | Yes |
| แก้ไขข้อมูล | Yes |
| ต้องยืนยัน | Yes |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ADVANCED |
| ไอคอน |  |

<details><summary>With these properties (JSON)</summary>

```json
{"InputParametersUsed":null,"Prominence":"Display_Prominently","NeedsConfirmation":true,"ConfirmationMessage":"","ModifiesData":true,"BulkApplicable":true}
```

</details>

## Edit

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | EDIT_RECORD |
| การแสดงผล | Display_Overlay |
| ลำดับ | 1 |
| Bulk action | No |
| แก้ไขข้อมูล | Yes |
| ต้องยืนยัน | No |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

<details><summary>With these properties (JSON)</summary>

```json
{"DesktopBehavior":"Open a form","DesktopEditBehavior":"Edit inplace","Prominence":"Display_Overlay","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":true,"BulkApplicable":false}
```

</details>

## Add

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | ADD_RECORD |
| การแสดงผล | Display_Overlay |
| ลำดับ | 1 |
| Bulk action | Yes |
| แก้ไขข้อมูล | Yes |
| ต้องยืนยัน | No |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

<details><summary>With these properties (JSON)</summary>

```json
{"Prominence":"Display_Overlay","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":true,"BulkApplicable":true}
```

</details>

## View Ref (_ComputedKey_ID_SCGนครหลวงJWDภูมิภาค)

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | NAVIGATE_APP |
| การแสดงผล | Display_Inline |
| ลำดับ | 1 |
| Bulk action | No |
| แก้ไขข้อมูล | No |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | ID_SCGนครหลวงJWDภูมิภาค |
| ตั้งค่าคอลัมน์ | ID_SCGนครหลวงJWDภูมิภาค |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
NOT(ISBLANK([ID_SCGนครหลวงJWDภูมิภาค]))
```

<details><summary>With these properties (JSON)</summary>

```json
{"NavigateTarget":"CONCATENATE(\"#page=detail&table=SCG%E0%B8%99%E0%B8%84%E0%B8%A3%E0%B8%AB%E0%B8%A5%E0%B8%A7%E0%B8%87JWD%E0%B8%A0%E0%B8%B9%E0%B8%A1%E0%B8%B4%E0%B8%A0%E0%B8%B2%E0%B8%84&row=\", ENCODEURL([ID_SCGนครหลวงJWDภูมิภาค]) )","Prominence":"Display_Inline","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":false,"BulkApplicable":false}
```

</details>

## View Map (ต้นทาง)

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | NAVIGATE_APP |
| การแสดงผล | Display_Inline |
| ลำดับ | 1 |
| Bulk action | No |
| แก้ไขข้อมูล | No |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | ต้นทาง |
| ตั้งค่าคอลัมน์ | ต้นทาง |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
NOT(ISBLANK([ต้นทาง]))
```

<details><summary>With these properties (JSON)</summary>

```json
{"NavigateTarget":"CONCATENATE(\"#page=map&table=%E0%B8%97%E0%B8%B3%E0%B9%80%E0%B8%9A%E0%B8%B4%E0%B8%81%E0%B8%AA%E0%B9%88%E0%B8%A7%E0%B8%99%E0%B8%95%E0%B9%88%E0%B8%B2%E0%B8%87Scg%E0%B8%A7%E0%B8%B1%E0%B8%87%E0%B8%99%E0%B9%89%E0%B8%AD%E0%B8%A2&mapcolumn=%E0%B8%95%E0%B9%89%E0%B8%99%E0%B8%97%E0%B8%B2%E0%B8%87&row=\", ENCODEURL([_THISROW]))","Prominence":"Display_Inline","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":false,"BulkApplicable":false}
```

</details>

## Compose Email (Email พนักงาน)

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | EMAIL |
| การแสดงผล | Display_Inline |
| ลำดับ | 1 |
| Bulk action | No |
| แก้ไขข้อมูล | No |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | Email พนักงาน |
| ตั้งค่าคอลัมน์ | Email พนักงาน |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
NOT(ISBLANK([Email พนักงาน]))
```

<details><summary>With these properties (JSON)</summary>

```json
{"EmailTo":"[Email พนักงาน]","Subject":null,"Body":null,"Prominence":"Display_Inline","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":false,"BulkApplicable":false}
```

</details>

## อัพเดตค่าสถานะผ่านการตรวจสอบ

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | SET_COLUMN_VALUE |
| การแสดงผล | Display_Prominently |
| ลำดับ | 1 |
| Bulk action | Yes |
| แก้ไขข้อมูล | Yes |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | สร้างแผนที่Google Map & QR Code |
| ตั้งค่าคอลัมน์ | สถานะ |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
=USERROLE() = "ADMIN"
```

**ตั้งค่าเป็น:**

```
="ผ่านการตรวจสอบ"
```

<details><summary>With these properties (JSON)</summary>

```json
{"Assignments": [{"ColumnToEdit":"สถานะ","NewColumnValue":"=\"ผ่านการตรวจสอบ\""}],"ColumnToEdit":"สถานะ","NewColumnValue":"=\"ผ่านการตรวจ สอบ\"","InputParametersUsed":null,"Prominence":"Display_Prominently","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":true,"BulkApplicable":true}
```

</details>

## Open Url (แสดงแผนที่_GoogleMapsRoutesAPI)

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | NAVIGATE_URL |
| การแสดงผล | Display_Inline |
| ลำดับ | 1 |
| Bulk action | No |
| แก้ไขข้อมูล | No |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | แสดงแผนที่_GoogleMapsRoutesAPI |
| ตั้งค่าคอลัมน์ | แสดงแผนที่_GoogleMapsRoutesAPI |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
NOT(ISBLANK([แสดงแผนที่_GoogleMapsRoutesAPI]))
```

<details><summary>With these properties (JSON)</summary>

```json
{"NavigateTarget":"[แสดงแผนที่_GoogleMapsRoutesAPI]","LaunchExternal":false,"Prominence":"Display_Inline","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":false,"BulkApplicable":false}
```

</details>

## อัพเดตสถานะไม่ผ่านการตรวจสอบ

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | SET_COLUMN_VALUE |
| การแสดงผล | Display_Prominently |
| ลำดับ | 1 |
| Bulk action | Yes |
| แก้ไขข้อมูล | Yes |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | สถานะ |
| ตั้งค่าคอลัมน์ | สถานะ |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
=USERROLE() = "ADMIN"
```

**ตั้งค่าเป็น:**

```
="ไม่ผ่านการตรวจสอบ"
```

<details><summary>With these properties (JSON)</summary>

```json
{"Assignments": [{"ColumnToEdit":"สถานะ","NewColumnValue":"=\"ไม่ผ่านการ ตรวจสอบ\""}],"ColumnToEdit":"สถานะ","NewColumnValue":"=\"ไม่ผ่านการตรวจ สอบ\"","InputParametersUsed":null,"Prominence":"Display_Prominently","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":true,"BulkApplicable":true}
```

</details>

## ปุ่มเปิดYes 2

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | SET_COLUMN_VALUE |
| การแสดงผล | Display_Prominently |
| ลำดับ | 1 |
| Bulk action | Yes |
| แก้ไขข้อมูล | Yes |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | สร้างPDFเบิกส่วนต่าง |
| ตั้งค่าคอลัมน์ | สร้างPDFเบิกส่วนต่าง |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
=USERROLE() = "ADMIN"
```

**ตั้งค่าเป็น:**

```
=TRUE
```

<details><summary>With these properties (JSON)</summary>

```json
{"Assignments":[{"ColumnToEdit":"สร้างPDFเบิกส่วน ต่าง","NewColumnValue":"=TRUE"}],"ColumnToEdit":"สร้างPDFเบิกส่วน ต่าง","NewColumnValue":"=TRUE","InputParametersUsed":null,"Prominence":"Display_Prominently","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":true,"BulkApplicable":true}
```

</details>

## ทำเบิกส่วนต่างScgวังน้อยcsv

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | EXPORT_VIEW |
| การแสดงผล | Display_Prominently |
| ลำดับ | 1 |
| Bulk action | No |
| แก้ไขข้อมูล | No |
| ต้องยืนยัน | No |
| ปิด sync อัตโนมัติ | No Display name โหลดไฟล์csv |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
true
```

<details><summary>With these properties (JSON)</summary>

```json
{"CsvLocale":"en-GB","Prominence":"Display_Prominently","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":false,"BulkApplicable":false}
```

</details>

## View Ref (ID_พนักงาน)

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | NAVIGATE_APP |
| การแสดงผล | Display_Inline |
| ลำดับ | 1 |
| Bulk action | No |
| แก้ไขข้อมูล | No |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | ID_พนักงาน |
| ตั้งค่าคอลัมน์ | ID_พนักงาน |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
NOT(ISBLANK([ID_พนักงาน]))
```

<details><summary>With these properties (JSON)</summary>

```json
{"NavigateTarget":"CONCATENATE(\"#page=detail&table=%E0%B8%82%E0%B9%89%E0%B8%AD%E0%B8%A1%E0%B8%B9%E0%B8%A5%E0%B8%9E%E0%B8%99%E0%B8%B1%E0%B8%81%E0%B8%87%E0%B8%B2%E0%B8%99&row=\", ENCODEURL([ID_พนักงาน]) )","Prominence":"Display_Inline","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":false,"BulkApplicable":false}
```

</details>

## ปุ่มเปิดYes_ราคาตามระยะทาง

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | SET_COLUMN_VALUE |
| การแสดงผล | Display_Prominently |
| ลำดับ | 1 |
| Bulk action | Yes |
| แก้ไขข้อมูล | Yes |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | สร้างPDFเบิกส่วนต่าง |
| ตั้งค่าคอลัมน์ | สร้างPDFเบิกตามระยะทาง |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
=USERROLE() = "ADMIN"
```

**ตั้งค่าเป็น:**

```
=TRUE
```

<details><summary>With these properties (JSON)</summary>

```json
{"Assignments":[{"ColumnToEdit":"สร้างPDFเบิกตามระยะ ทาง","NewColumnValue":"=TRUE"}],"ColumnToEdit":"สร้างPDFเบิกตามระยะ ทาง","NewColumnValue":"=TRUE","InputParametersUsed":null,"Prominence":"Display_Prominently","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":true,"BulkApplicable":true}
```

</details>

## Open Url (Candidate_2_แสดงแผนที่)

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | NAVIGATE_URL |
| การแสดงผล | Display_Inline |
| ลำดับ | 1 |
| Bulk action | No |
| แก้ไขข้อมูล | No |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | Candidate_2_แสดงแผนที่ |
| ตั้งค่าคอลัมน์ | Candidate_2_แสดงแผนที่ |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
NOT(ISBLANK([Candidate_2_แสดงแผนที่]))
```

<details><summary>With these properties (JSON)</summary>

```json
{"NavigateTarget":"[Candidate_2_แสดงแผนที่]","LaunchExternal":false,"Prominence":"Display_Inline","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":false,"BulkApplicable":false}
```

</details>

## Open Url (Candidate_3_แสดงแผนที่)

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | NAVIGATE_URL |
| การแสดงผล | Display_Inline |
| ลำดับ | 1 |
| Bulk action | No |
| แก้ไขข้อมูล | No |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | Candidate_3_แสดงแผนที่ |
| ตั้งค่าคอลัมน์ | Candidate_3_แสดงแผนที่ |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
NOT(ISBLANK([Candidate_3_แสดงแผนที่]))
```

<details><summary>With these properties (JSON)</summary>

```json
{"NavigateTarget":"[Candidate_3_แสดงแผนที่]","LaunchExternal":false,"Prominence":"Display_Inline","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":false,"BulkApplicable":false}
```

</details>

