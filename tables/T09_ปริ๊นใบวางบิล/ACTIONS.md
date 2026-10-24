# Actions ของตาราง ปริ๊นใบวางบิล

รวม **21 actions**

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

## Clear

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | SET_COLUMN_VALUE |
| การแสดงผล | Do_Not_Display |
| ลำดับ | 1 |
| Bulk action | Yes |
| แก้ไขข้อมูล | Yes |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | ชื่องาน |
| ตั้งค่าคอลัมน์ | ชื่องาน |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
=USERROLE() = ADMIN
```

**ตั้งค่าเป็น:**

```
=""
```

<details><summary>With these properties (JSON)</summary>

```json
{"Assignments":[{"ColumnToEdit":"ชื่อ งาน","NewColumnValue":"=\"\""},{"ColumnToEdit":"ปริ๊นใบวางบิล แยกตามชื่องาน","NewColumnValue":"=\"\""}],"ColumnToEdit":"ชื่องาน","NewColumnValue":"=\"\"","InputParametersUsed":null,"Prominence":"Do_Not_Display","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":true,"BulkApplicable":true}
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

## ไอโรบอท

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | SET_COLUMN_VALUE |
| การแสดงผล | Do_Not_Display |
| ลำดับ | 1 |
| Bulk action | Yes |
| แก้ไขข้อมูล | Yes |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | ชื่องาน |
| ตั้งค่าคอลัมน์ | ชื่องาน |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
true
```

**ตั้งค่าเป็น:**

```
="ไอโรบอท"
```

<details><summary>With these properties (JSON)</summary>

```json
{"Assignments":[{"ColumnToEdit":"ชื่อ งาน","NewColumnValue":"=\"ไอโรบอท\""},{"ColumnToEdit":"ปริ๊นใบวางบิลแยกตามชื่อ งาน","NewColumnValue":"=TRUE"}],"ColumnToEdit":"ชื่อ งาน","NewColumnValue":"=\"ไอโร บอท\"","InputParametersUsed":null,"Prominence":"Do_Not_Display","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":true,"BulkApplicable":true}
```

</details>

## รับเอกสาร (งานพี่เหน่ง)

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | SET_COLUMN_VALUE |
| การแสดงผล | Do_Not_Display |
| ลำดับ | 1 |
| Bulk action | Yes |
| แก้ไขข้อมูล | Yes |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | ชื่องาน |
| ตั้งค่าคอลัมน์ | ชื่องาน |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
true
```

**ตั้งค่าเป็น:**

```
="รับเอกสาร (งานพี่เหน่ง)"
```

<details><summary>With these properties (JSON)</summary>

```json
{"Assignments":[{"ColumnToEdit":"ชื่อ งาน","NewColumnValue":"=\"รับเอกสาร (งานพี่เหน่ง)\""}, {"ColumnToEdit":"ปริ๊นใบวางบิลแยกตามชื่อ งาน","NewColumnValue":"=TRUE"}],"ColumnToEdit":"ชื่อ งาน","NewColumnValue":"=\"รับเอกสาร (งานพี่ เหน่ง)\"","InputParametersUsed":null,"Prominence":"Do_Not_Display","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":true,"BulkApplicable":true}
```

</details>

## โอนคลัง เอเธน

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | SET_COLUMN_VALUE |
| การแสดงผล | Do_Not_Display |
| ลำดับ | 1 |
| Bulk action | Yes |
| แก้ไขข้อมูล | Yes |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | ชื่องาน |
| ตั้งค่าคอลัมน์ | ชื่องาน |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
true
```

**ตั้งค่าเป็น:**

```
="โอนคลัง เอเธน"
```

<details><summary>With these properties (JSON)</summary>

```json
{"Assignments":[{"ColumnToEdit":"ชื่อ งาน","NewColumnValue":"=\"โอนคลัง เอเธน\""}, {"ColumnToEdit":"ปริ๊นใบวางบิลแยกตามชื่อ งาน","NewColumnValue":"=TRUE"}],"ColumnToEdit":"ชื่อ งาน","NewColumnValue":"=\"โอนคลัง เอ เธน\"","InputParametersUsed":null,"Prominence":"Do_Not_Display","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":true,"BulkApplicable":true}
```

</details>

## โอนคลัง กระสอบ2(บางบัวทอง)

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | SET_COLUMN_VALUE |
| การแสดงผล | Do_Not_Display |
| ลำดับ | 1 |
| Bulk action | Yes |
| แก้ไขข้อมูล | Yes |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | ชื่องาน |
| ตั้งค่าคอลัมน์ | ชื่องาน |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
true
```

**ตั้งค่าเป็น:**

```
="โอนคลัง กระสอบ2(บางบัวทอง)"
```

<details><summary>With these properties (JSON)</summary>

```json
{"Assignments":[{"ColumnToEdit":"ชื่อ งาน","NewColumnValue":"=\"โอนคลัง กระสอบ2(บางบัวทอง)\""}, {"ColumnToEdit":"ปริ๊นใบวางบิลแยกตามชื่อ งาน","NewColumnValue":"=TRUE"}],"ColumnToEdit":"ชื่อ งาน","NewColumnValue":"=\"โอนคลัง กระสอบ2(บางบัวทอง)\"","InputParametersUsed":null,"Prominence":"Do_Not_Display","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":true,"BulkApplicable":true}
```

</details>

## คลังSCGJWDวังน้อย

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | SET_COLUMN_VALUE |
| การแสดงผล | Do_Not_Display |
| ลำดับ | 1 |
| Bulk action | Yes |
| แก้ไขข้อมูล | Yes |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | ชื่องาน |
| ตั้งค่าคอลัมน์ | ชื่องาน |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
true
```

**ตั้งค่าเป็น:**

```
="คลังSCGJWDวังน้อย"
```

<details><summary>With these properties (JSON)</summary>

```json
{"Assignments":[{"ColumnToEdit":"ชื่อ งาน","NewColumnValue":"=\"คลังSCGJWDวังน้อย\""}, {"ColumnToEdit":"ปริ๊นใบวางบิลแยกตามชื่อ งาน","NewColumnValue":"=TRUE"}],"ColumnToEdit":"ชื่อ งาน","NewColumnValue":"=\"คลังSCGJWDวังน้อย\"","InputParametersUsed":null,"Prominence":"Do_Not_Display","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":true,"BulkApplicable":true}
```

</details>

## MeSpace

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | SET_COLUMN_VALUE |
| การแสดงผล | Do_Not_Display |
| ลำดับ | 1 |
| Bulk action | Yes |
| แก้ไขข้อมูล | Yes |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | ชื่องาน |
| ตั้งค่าคอลัมน์ | ชื่องาน |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
true
```

**ตั้งค่าเป็น:**

```
="MeSpace"
```

<details><summary>With these properties (JSON)</summary>

```json
{"Assignments":[{"ColumnToEdit":"ชื่อ งาน","NewColumnValue":"=\"MeSpace\""},{"ColumnToEdit":"ปริ๊นใบวางบิลแยกตามชื่อ งาน","NewColumnValue":"=TRUE"}],"ColumnToEdit":"ชื่อ งาน","NewColumnValue":"=\"MeSpace\"","InputParametersUsed":null,"Prominence":"Do_Not_Display","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":true,"BulkApplicable":true}
```

</details>

## โอนคลัง มโนยนต์ (นวนคร)

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | SET_COLUMN_VALUE |
| การแสดงผล | Do_Not_Display |
| ลำดับ | 1 |
| Bulk action | Yes |
| แก้ไขข้อมูล | Yes |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | ชื่องาน |
| ตั้งค่าคอลัมน์ | ชื่องาน |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
true
```

**ตั้งค่าเป็น:**

```
="โอนคลัง มโนยนต์ (นวนคร)"
```

<details><summary>With these properties (JSON)</summary>

```json
{"Assignments":[{"ColumnToEdit":"ชื่อ งาน","NewColumnValue":"=\"โอนคลัง มโนยนต์ (นวนคร)\""}, {"ColumnToEdit":"ปริ๊นใบวางบิลแยกตามชื่อ งาน","NewColumnValue":"=TRUE"}],"ColumnToEdit":"ชื่อ งาน","NewColumnValue":"=\"โอนคลัง มโนยนต์ (นว นคร)\"","InputParametersUsed":null,"Prominence":"Do_Not_Display","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":true,"BulkApplicable":true}
```

</details>

## โอนคลัง (GQ) จีคิว

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | SET_COLUMN_VALUE |
| การแสดงผล | Do_Not_Display |
| ลำดับ | 1 |
| Bulk action | Yes |
| แก้ไขข้อมูล | Yes |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | ชื่องาน |
| ตั้งค่าคอลัมน์ | ชื่องาน |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
true
```

**ตั้งค่าเป็น:**

```
="โอนคลัง (GQ) จีคิว"
```

<details><summary>With these properties (JSON)</summary>

```json
{"Assignments":[{"ColumnToEdit":"ชื่อ งาน","NewColumnValue":"=\"โอนคลัง (GQ) จีคิว\""}, {"ColumnToEdit":"ปริ๊นใบวางบิลแยกตามชื่อ งาน","NewColumnValue":"=TRUE"}],"ColumnToEdit":"ชื่อ งาน","NewColumnValue":"=\"โอนคลัง (GQ) จี คิว\"","InputParametersUsed":null,"Prominence":"Do_Not_Display","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":true,"BulkApplicable":true}
```

</details>

## ปริ๊นวางบิลทุกงาน

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | COMPOSITE |
| การแสดงผล | Display_Prominently |
| ลำดับ | 1 |
| Bulk action | Yes |
| แก้ไขข้อมูล | Yes |
| ต้องยืนยัน | No |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
true
```

<details><summary>With these properties (JSON)</summary>

```json
{"Actions":[{"ActionName":"ไอโรบอท"},{"ActionName":"Clear"}, {"ActionName":"รับเอกสาร (งานพี่เหน่ง)"},{"ActionName":"Clear"},{"ActionName":"โอนคลัง เอเธน"},{"ActionName":"Clear"}, {"ActionName":"โอนคลัง กระสอบ2(บางบัวทอง)"}, {"ActionName":"Clear"},{"ActionName":"คลังSCGJWDวังน้อย"}, {"ActionName":"Clear"},{"ActionName":"MeSpace"}, {"ActionName":"Clear"},{"ActionName":"โอนคลัง มโนยนต์ (นว นคร)"},{"ActionName":"Clear"},{"ActionName":"โอนคลัง (GQ) จี คิว"},{"ActionName":"Clear"},{"ActionName":"รับเอกสาร (งานพี่ เหน่ง) สตีเบล"},{"ActionName":"Clear"},{"ActionName":"เบทา โกร+เหมาตู้"},{"ActionName":"Clear"},{"ActionName":"Thai paper(SCG Express)"},{"ActionName":"Clear"}, {"ActionName":"LINEMAN (6W) (SCG Express)"}, {"ActionName":"Clear"},{"ActionName":"โอนคลัง บุญถาวร เกษตร_นวมินทร์"},{"ActionName":"เคลียหน้า จอ"}],"Prominence":"Display_Prominently","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":true,"BulkApplicable":true}
```

</details>

## เคลียหน้าจอ

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | SET_COLUMN_VALUE |
| การแสดงผล | Display_Prominently |
| ลำดับ | 1 |
| Bulk action | Yes |
| แก้ไขข้อมูล | Yes |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | ชื่องาน |
| ตั้งค่าคอลัมน์ | ชื่องาน |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
true
```

**ตั้งค่าเป็น:**

```
=""
```

<details><summary>With these properties (JSON)</summary>

```json
{"Assignments":[{"ColumnToEdit":"ชื่อ งาน","NewColumnValue":"=\"\""}, {"ColumnToEdit":"StartDate","NewColumnValue":"=\"\""}, {"ColumnToEdit":"EndDate","NewColumnValue":"=\"\""}, {"ColumnToEdit":"ปริ๊นใบวางบิลแยกตามชื่อ งาน","NewColumnValue":"=\"\""},{"ColumnToEdit":"Export to xlsx","NewColumnValue":"=\"\""},{"ColumnToEdit":"Export to xlsxTo Athens","NewColumnValue":"=\"\""},{"ColumnToEdit":"วันที่ ออกเอกสาร","NewColumnValue":"=\"\""}],"ColumnToEdit":"ชื่อ งาน","NewColumnValue":"=\"\"","InputParametersUsed":null,"Prominence":"Display_Prominently","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":true,"BulkApplicable":true}
```

</details>

## รับเอกสาร (งานพี่เหน่ง) สตีเบล

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | SET_COLUMN_VALUE |
| การแสดงผล | Do_Not_Display |
| ลำดับ | 1 |
| Bulk action | Yes |
| แก้ไขข้อมูล | Yes |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | ชื่องาน |
| ตั้งค่าคอลัมน์ | ชื่องาน |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
true
```

**ตั้งค่าเป็น:**

```
="รับเอกสาร (งานพี่เหน่ง) สตีเบล"
```

<details><summary>With these properties (JSON)</summary>

```json
{"Assignments":[{"ColumnToEdit":"ชื่อ งาน","NewColumnValue":"=\"รับเอกสาร (งานพี่เหน่ง) สตีเบล\""}, {"ColumnToEdit":"ปริ๊นใบวางบิลแยกตามชื่อ งาน","NewColumnValue":"=TRUE"}],"ColumnToEdit":"ชื่อ งาน","NewColumnValue":"=\"รับเอกสาร (งานพี่เหน่ง) สตี เบล\"","InputParametersUsed":null,"Prominence":"Do_Not_Display","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":true,"BulkApplicable":true}
```

</details>

## CLEAR_ปริ๊นใบวางบิล_Action

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | SET_COLUMN_VALUE |
| การแสดงผล | Do_Not_Display |
| ลำดับ | 1 |
| Bulk action | Yes |
| แก้ไขข้อมูล | Yes |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | ชื่องาน |
| ตั้งค่าคอลัมน์ | ชื่องาน |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
true
```

**ตั้งค่าเป็น:**

```
=""
```

<details><summary>With these properties (JSON)</summary>

```json
{"Assignments":[{"ColumnToEdit":"ชื่อ งาน","NewColumnValue":"=\"\""}, {"ColumnToEdit":"StartDate","NewColumnValue":"=\"\""}, {"ColumnToEdit":"EndDate","NewColumnValue":"=\"\""}, {"ColumnToEdit":"Export to xlsx","NewColumnValue":"=\"\""}],"ColumnToEdit":"ชื่อ งาน","NewColumnValue":"=\"\"","InputParametersUsed":null,"Prominence":"Do_Not_Display","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":true,"BulkApplicable":true}
```

</details>

## ปริ๊นใบวางบิลcsv

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

## เบทาโกร+เหมาตู้

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | SET_COLUMN_VALUE |
| การแสดงผล | Do_Not_Display |
| ลำดับ | 1 |
| Bulk action | Yes |
| แก้ไขข้อมูล | Yes |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | ชื่องาน |
| ตั้งค่าคอลัมน์ | ชื่องาน |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
true
```

**ตั้งค่าเป็น:**

```
="เบทาโกร+เหมาตู้"
```

<details><summary>With these properties (JSON)</summary>

```json
{"Assignments":[{"ColumnToEdit":"ชื่อ งาน","NewColumnValue":"=\"เบทาโกร+เหมาตู้\""}, {"ColumnToEdit":"ปริ๊นใบวางบิลแยกตามชื่อ งาน","NewColumnValue":"=TRUE"}],"ColumnToEdit":"ชื่อ งาน","NewColumnValue":"=\"เบทาโกร+เหมา ตู้\"","InputParametersUsed":null,"Prominence":"Do_Not_Display","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":true,"BulkApplicable":true}
```

</details>

## Thai paper (SCG Express)

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | SET_COLUMN_VALUE |
| การแสดงผล | Do_Not_Display |
| ลำดับ | 1 |
| Bulk action | Yes |
| แก้ไขข้อมูล | Yes |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | ชื่องาน |
| ตั้งค่าคอลัมน์ | ชื่องาน |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
true
```

**ตั้งค่าเป็น:**

```
="Thai paper (SCG Express)"
```

<details><summary>With these properties (JSON)</summary>

```json
{"Assignments":[{"ColumnToEdit":"ชื่อ งาน","NewColumnValue":"=\"Thai paper (SCG Express)\""}, {"ColumnToEdit":"ปริ๊นใบวางบิลแยกตามชื่อ งาน","NewColumnValue":"=TRUE"}],"ColumnToEdit":"ชื่อ งาน","NewColumnValue":"=\"Thai paper (SCG Express)\"","InputParametersUsed":null,"Prominence":"Do_Not_Display","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":true,"BulkApplicable":true}
```

</details>

## LINEMAN (6W) (SCG Express)

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | SET_COLUMN_VALUE |
| การแสดงผล | Do_Not_Display |
| ลำดับ | 1 |
| Bulk action | Yes |
| แก้ไขข้อมูล | Yes |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | ชื่องาน |
| ตั้งค่าคอลัมน์ | ชื่องาน |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
true
```

**ตั้งค่าเป็น:**

```
="LINEMAN (6W) (SCG Express)"
```

<details><summary>With these properties (JSON)</summary>

```json
{"Assignments":[{"ColumnToEdit":"ชื่อ งาน","NewColumnValue":"=\"LINEMAN (6W) (SCG Express)\""}, {"ColumnToEdit":"ปริ๊นใบวางบิลแยกตามชื่อ งาน","NewColumnValue":"=TRUE"}],"ColumnToEdit":"ชื่อ งาน","NewColumnValue":"=\"LINEMAN (6W) (SCG Express)\"","InputParametersUsed":null,"Prominence":"Do_Not_Display","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":true,"BulkApplicable":true}
```

</details>

## โอนคลัง บุญถาวร เกษตร_นวมินทร์

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | SET_COLUMN_VALUE |
| การแสดงผล | Do_Not_Display |
| ลำดับ | 1 |
| Bulk action | Yes |
| แก้ไขข้อมูล | Yes |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | ชื่องาน |
| ตั้งค่าคอลัมน์ | ชื่องาน |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
true
```

**ตั้งค่าเป็น:**

```
="โอนคลัง บุญถาวร เกษตร_นวมินทร์"
```

<details><summary>With these properties (JSON)</summary>

```json
{"Assignments":[{"ColumnToEdit":"ชื่อ งาน","NewColumnValue":"=\"โอนคลัง บุญถาวร เกษตร_นวมิ นทร์\""},{"ColumnToEdit":"ปริ๊นใบวางบิลแยกตามชื่อ งาน","NewColumnValue":"=TRUE"}],"ColumnToEdit":"ชื่อ งาน","NewColumnValue":"=\"โอนคลัง บุญถาวร เกษตร_นวมิ นทร์\"","InputParametersUsed":null,"Prominence":"Do_Not_Display","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":true,"BulkApplicable":true}
```

</details>

