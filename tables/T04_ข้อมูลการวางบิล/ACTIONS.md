# Actions ของตาราง ข้อมูลการวางบิล

รวม **10 actions**

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

## Compose Email (Email ผู้อนุมัติ)

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | EMAIL |
| การแสดงผล | Display_Inline |
| ลำดับ | 1 |
| Bulk action | No |
| แก้ไขข้อมูล | No |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | Email ผู้อนุมัติ |
| ตั้งค่าคอลัมน์ | Email ผู้อนุมัติ |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
NOT(ISBLANK([Email ผู้อนุมัติ]))
```

<details><summary>With these properties (JSON)</summary>

```json
{"EmailTo":"[Email ผู้อนุมัติ]","Subject":null,"Body":null,"Prominence":"Display_Inline","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":false,"BulkApplicable":false}
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

## อนุมัติ

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | SET_COLUMN_VALUE |
| การแสดงผล | Display_Prominently |
| ลำดับ | 1 |
| Bulk action | Yes |
| แก้ไขข้อมูล | Yes |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | สถานะการอนุมัติ |
| ตั้งค่าคอลัมน์ | สถานะการอนุมัติ |
| ปิด sync อัตโนมัติ | No Display name "อนุมัติ" |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
=AND( [สถานะการอนุมัติ] <> "อนุมัติ", USERROLE() = "ADMIN")
```

**ตั้งค่าเป็น:**

```
"อนุมัติ"
```

<details><summary>With these properties (JSON)</summary>

```json
{"Assignments":[{"ColumnToEdit":"สถานะการ อนุมัติ","NewColumnValue":"\"อนุมัติ\""}],"ColumnToEdit":"สถานะ การ อนุมัติ","NewColumnValue":"\"อนุมัติ\"","InputParametersUsed":null,"Prominence":"Display_Prominently","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":true,"BulkApplicable":true}
```

</details>

## รอการอนุมัติ

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | SET_COLUMN_VALUE |
| การแสดงผล | Display_Inline |
| ลำดับ | 1 |
| Bulk action | Yes |
| แก้ไขข้อมูล | Yes |
| ต้องยืนยัน | Yes |
| ผูกกับคอลัมน์ | สถานะการอนุมัติ |
| ตั้งค่าคอลัมน์ | สถานะการอนุมัติ |
| ปิด sync อัตโนมัติ | No Display name "รอการอนุมัติ" |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
=AND( [สถานะการอนุมัติ] <> "รอการอนุมัติ", USERROLE() = "ADMIN")
```

**ตั้งค่าเป็น:**

```
="รอการอนุมัติ"
```

<details><summary>With these properties (JSON)</summary>

```json
{"Assignments":[{"ColumnToEdit":"สถานะการ อนุมัติ","NewColumnValue":"=\"รอการ อนุมัติ\""}],"ColumnToEdit":"สถานะการ อนุมัติ","NewColumnValue":"=\"รอการ อนุมัติ\"","InputParametersUsed":null,"Prominence":"Display_Inline","NeedsConfirmation":true,"ConfirmationMessage":"","ModifiesData":true,"BulkApplicable":true}
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

## ส่งรูปวางบิลหรือสลิปโอนเงิน

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | NAVIGATE_DIFFERENT_APP |
| การแสดงผล | Display_Prominently |
| ลำดับ | 1 |
| Bulk action | No Confirmation Message กดส่งรูปวางบิล เพื่อเข้าสู่ขั้นตอนการเพื่มรูปถ่าย |
| แก้ไขข้อมูล | No |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | จำนวนด่าน |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
true
```

<details><summary>With these properties (JSON)</summary>

```json
{"NavigateTarget":"=LINKTOAPP(\"1c544f2c-efb8-41ee-8cc5-ac5573f10e5c\") \n& LINKTOROW([ID_วางบิล], \"ข้อมูลการวาง บิล_Detail\")","Prominence":"Display_Prominently","NeedsConfirmation":false,"ConfirmationMessage":"กดส่งรูปวางบิล เพื่อเข้าสู่ ขั้นตอนการเพื่มรูป ถ่าย","ModifiesData":false,"BulkApplicable":false}
```

</details>

## ข้อมูลการวางบิลcsv

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

