# Actions ของตาราง PDFพนักงาน

รวม **26 actions**

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

## CLEAR 2

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | SET_COLUMN_VALUE |
| การแสดงผล | Display_Prominently |
| ลำดับ | 1 |
| Bulk action | Yes |
| แก้ไขข้อมูล | Yes |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | ชื่องาน |
| ตั้งค่าคอลัมน์ | ชื่อ - นามสกุล |
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
{"Assignments":[{"ColumnToEdit":"ชื่อ -นามสกุล","NewColumnValue":"=\"\""}, {"ColumnToEdit":"StartDate","NewColumnValue":"=\"\""}, {"ColumnToEdit":"EndDate","NewColumnValue":"=\"\""}, {"ColumnToEdit":"Export to XLSX","NewColumnValue":"=\"\""}, {"ColumnToEdit":"ชื่อ ไฟล์","NewColumnValue":"=\"\""}],"ColumnToEdit":"ชื่อ -นามสกุล","NewColumnValue":"=\"\"","InputParametersUsed":null,"Prominence":"Display_Prominently","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":true,"BulkApplicable":true}
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

## สร้างใบป่ะหน้า_สำเริง แก้วกามเกตุ

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | SET_COLUMN_VALUE |
| การแสดงผล | Do_Not_Display |
| ลำดับ | 1 |
| Bulk action | Yes |
| แก้ไขข้อมูล | Yes |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | ชื่อ - นามสกุล |
| ตั้งค่าคอลัมน์ | ชื่อ - นามสกุล |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
true
```

**ตั้งค่าเป็น:**

```
="สำเริง แก้วกามเกตุ"
```

<details><summary>With these properties (JSON)</summary>

```json
{"Assignments":[{"ColumnToEdit":"ชื่อ -นามสกุล","NewColumnValue":"=\"สำเริง แก้วกามเกตุ\""}, {"ColumnToEdit":"Export to XLSX","NewColumnValue":"=TRUE"}],"ColumnToEdit":"ชื่อ -นามสกุล","NewColumnValue":"=\"สำเริง แก้วกาม เกตุ\"","InputParametersUsed":null,"Prominence":"Do_Not_Display","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":true,"BulkApplicable":true}
```

</details>

## สร้างใบป่ะหน้าทุกคน

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
{"Actions":[{"ActionName":"สร้างใบป่ะหน้า_สำเริง แก้วกามเกตุ"}, {"ActionName":"Clearหน้าจอ"},{"ActionName":"สร้างใบป่ะหน้า_สุ ทิศ นันพนัก"},{"ActionName":"Clearหน้าจอ"},{"ActionName":"สร้างใบป่ะหน้า_เอกรัฐ อนุรักษ์"},{"ActionName":"Clearหน้าจอ"}, {"ActionName":"สร้างใบป่ะหน้า_สุด พันพม่า"}, {"ActionName":"Clearหน้าจอ"},{"ActionName":"สร้างใบป่ะ หน้า_ธวัชชัย หนูมา"},{"ActionName":"Clearหน้าจอ"}, {"ActionName":"สร้างใบป่ะหน้า_ปราโมทย์ เรียนพิษ"}, {"ActionName":"Clearหน้าจอ"},{"ActionName":"สร้างใบป่ะ หน้า_กฤษฎา พิญญะดำ"},{"ActionName":"Clearหน้าจอ"}, {"ActionName":"สร้างใบป่ะหน้า_กิตติพงษ์ แหลมผักแว่น"}, {"ActionName":"Clearหน้าจอ"},{"ActionName":"สร้างใบป่ะ หน้า_จักรภัทร วงทอง"},{"ActionName":"Clearหน้าจอ"}, {"ActionName":"สร้างใบป่ะหน้า_พีระพล รูปแก้ว"}, {"ActionName":"Clearหน้าจอ"},{"ActionName":"สร้างใบป่ะ หน้า_อชิตพล ยังยิ้ม"},{"ActionName":"Clearหน้าจอ"}, {"ActionName":"สร้างใบป่ะหน้า_ธีรยุทธ นราทอง"}, {"ActionName":"Clearหน้าจอ"},{"ActionName":"สร้างใบป่ะหน้า_จิรายุ โคตรวงษ์"},{"ActionName":"Clearหน้าจอ"},{"ActionName":"สร้างใบป่ะหน้า_ทัดเทพ พรมมา"},{"ActionName":"Clearหน้าจอ"}, {"ActionName":"สร้างใบป่ะหน้า_พงศธร หมวดไธสง"}, {"ActionName":"Clearหน้าจอ"},{"ActionName":"สร้างใบป่ะ หน้า_เกียรติศักดิ์ พินิจเมือง"},{"ActionName":"Clearหน้าจอ"}, {"ActionName":"สร้างใบป่ะหน้า_เกียรติศักดิ์ ยอมใหญ่"}, {"ActionName":"Clearหน้าจอ"},{"ActionName":"สร้างใบป่ะ หน้า_สิทธิชัย ทิศวงค์"},{"ActionName":"Clearหน้าจอ"}, {"ActionName":"สร้างใบป่ะหน้า_ไนยชน วงศ์บุญมา"}, {"ActionName":"CLEAR 2"}],"Prominence":"Display_Prominently","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":true,"BulkApplicable":true}
```

</details>

## Clearหน้าจอ

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | SET_COLUMN_VALUE |
| การแสดงผล | Do_Not_Display |
| ลำดับ | 1 |
| Bulk action | Yes |
| แก้ไขข้อมูล | Yes |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | ชื่อ - นามสกุล |
| ตั้งค่าคอลัมน์ | ชื่อ - นามสกุล |
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
{"Assignments":[{"ColumnToEdit":"ชื่อ -นามสกุล","NewColumnValue":"=\"\""},{"ColumnToEdit":"Export toXLSX","NewColumnValue":"=\"\""},{"ColumnToEdit":"ชื่อ ไฟล์","NewColumnValue":"=\"\""}],"ColumnToEdit":"ชื่อ -นามสกุล","NewColumnValue":"=\"\"","InputParametersUsed":null,"Prominence":"Do_Not_Display","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":true,"BulkApplicable":true}
```

</details>

## สร้างใบป่ะหน้า_สุทิศ นันพนัก

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | SET_COLUMN_VALUE |
| การแสดงผล | Do_Not_Display |
| ลำดับ | 1 |
| Bulk action | Yes |
| แก้ไขข้อมูล | Yes |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | ชื่อ - นามสกุล |
| ตั้งค่าคอลัมน์ | ชื่อ - นามสกุล |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
true
```

**ตั้งค่าเป็น:**

```
="สุทิศ นันพนัก"
```

<details><summary>With these properties (JSON)</summary>

```json
{"Assignments":[{"ColumnToEdit":"ชื่อ -นามสกุล","NewColumnValue":"=\"สุทิศ นันพนัก\""}, {"ColumnToEdit":"Export to XLSX","NewColumnValue":"=TRUE"}],"ColumnToEdit":"ชื่อ -นามสกุล","NewColumnValue":"=\"สุทิศ นัน พนัก\"","InputParametersUsed":null,"Prominence":"Do_Not_Display","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":true,"BulkApplicable":true}
```

</details>

## สร้างใบป่ะหน้า_เอกรัฐ อนุรักษ์

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | SET_COLUMN_VALUE |
| การแสดงผล | Do_Not_Display |
| ลำดับ | 1 |
| Bulk action | Yes |
| แก้ไขข้อมูล | Yes |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | ชื่อ - นามสกุล |
| ตั้งค่าคอลัมน์ | ชื่อ - นามสกุล |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
true
```

**ตั้งค่าเป็น:**

```
="เอกรัฐ อนุรักษ์"
```

<details><summary>With these properties (JSON)</summary>

```json
{"Assignments":[{"ColumnToEdit":"ชื่อ -นามสกุล","NewColumnValue":"=\"เอกรัฐ อนุรักษ์\""}, {"ColumnToEdit":"Export to XLSX","NewColumnValue":"=TRUE"}],"ColumnToEdit":"ชื่อ -นามสกุล","NewColumnValue":"=\"เอกรัฐ อนุรักษ์\"","InputParametersUsed":null,"Prominence":"Do_Not_Display","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":true,"BulkApplicable":true}
```

</details>

## สร้างใบป่ะหน้า_สุด พันพม่า

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | SET_COLUMN_VALUE |
| การแสดงผล | Do_Not_Display |
| ลำดับ | 1 |
| Bulk action | Yes |
| แก้ไขข้อมูล | Yes |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | ชื่อ - นามสกุล |
| ตั้งค่าคอลัมน์ | ชื่อ - นามสกุล |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
true
```

**ตั้งค่าเป็น:**

```
="สุด พันพม่า"
```

<details><summary>With these properties (JSON)</summary>

```json
{"Assignments":[{"ColumnToEdit":"ชื่อ -นามสกุล","NewColumnValue":"=\"สุด พันพม่า\""}, {"ColumnToEdit":"Export to XLSX","NewColumnValue":"=TRUE"}],"ColumnToEdit":"ชื่อ -นามสกุล","NewColumnValue":"=\"สุด พัน พม่า\"","InputParametersUsed":null,"Prominence":"Do_Not_Display","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":true,"BulkApplicable":true}
```

</details>

## สร้างใบป่ะหน้า_ธวัชชัย หนูมา

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | SET_COLUMN_VALUE |
| การแสดงผล | Do_Not_Display |
| ลำดับ | 1 |
| Bulk action | Yes |
| แก้ไขข้อมูล | Yes |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | ชื่อ - นามสกุล |
| ตั้งค่าคอลัมน์ | ชื่อ - นามสกุล |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
true
```

**ตั้งค่าเป็น:**

```
="ธวัชชัย หนูมา"
```

<details><summary>With these properties (JSON)</summary>

```json
{"Assignments":[{"ColumnToEdit":"ชื่อ -นามสกุล","NewColumnValue":"=\"ธวัชชัย หนูมา\""}, {"ColumnToEdit":"Export to XLSX","NewColumnValue":"=TRUE"}],"ColumnToEdit":"ชื่อ -นามสกุล","NewColumnValue":"=\"ธวัชชัย หนู มา\"","InputParametersUsed":null,"Prominence":"Do_Not_Display","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":true,"BulkApplicable":true}
```

</details>

## สร้างใบป่ะหน้า_ปราโมทย์ เรียนพิษ

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | SET_COLUMN_VALUE |
| การแสดงผล | Do_Not_Display |
| ลำดับ | 1 |
| Bulk action | Yes |
| แก้ไขข้อมูล | Yes |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | ชื่อ - นามสกุล |
| ตั้งค่าคอลัมน์ | ชื่อ - นามสกุล |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
true
```

**ตั้งค่าเป็น:**

```
="ปราโมทย์ เรียนพิษ"
```

<details><summary>With these properties (JSON)</summary>

```json
{"Assignments":[{"ColumnToEdit":"ชื่อ -นามสกุล","NewColumnValue":"=\"ปราโมทย์ เรียนพิษ\""}, {"ColumnToEdit":"Export to XLSX","NewColumnValue":"=TRUE"}],"ColumnToEdit":"ชื่อ -นามสกุล","NewColumnValue":"=\"ปราโมทย์ เรียน พิษ\"","InputParametersUsed":null,"Prominence":"Do_Not_Display","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":true,"BulkApplicable":true}
```

</details>

## สร้างใบป่ะหน้า_กฤษฎา พิญญะดำ

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | SET_COLUMN_VALUE |
| การแสดงผล | Do_Not_Display |
| ลำดับ | 1 |
| Bulk action | Yes |
| แก้ไขข้อมูล | Yes |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | ชื่อ - นามสกุล |
| ตั้งค่าคอลัมน์ | ชื่อ - นามสกุล |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
true
```

**ตั้งค่าเป็น:**

```
="กฤษฎา พิญญะดำ"
```

<details><summary>With these properties (JSON)</summary>

```json
{"Assignments":[{"ColumnToEdit":"ชื่อ -นามสกุล","NewColumnValue":"=\"กฤษฎา พิญญะดำ\""}, {"ColumnToEdit":"Export to XLSX","NewColumnValue":"=TRUE"}],"ColumnToEdit":"ชื่อ -นามสกุล","NewColumnValue":"=\"กฤษฎา พิญญะ ดำ\"","InputParametersUsed":null,"Prominence":"Do_Not_Display","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":true,"BulkApplicable":true}
```

</details>

## สร้างใบป่ะหน้า_กิตติพงษ์ แหลมผักแว่น

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | SET_COLUMN_VALUE |
| การแสดงผล | Do_Not_Display |
| ลำดับ | 1 |
| Bulk action | Yes |
| แก้ไขข้อมูล | Yes |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | ชื่อ - นามสกุล |
| ตั้งค่าคอลัมน์ | ชื่อ - นามสกุล |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
true
```

**ตั้งค่าเป็น:**

```
="กิตติพงษ์ แหลมผักแว่น"
```

<details><summary>With these properties (JSON)</summary>

```json
{"Assignments":[{"ColumnToEdit":"ชื่อ -นามสกุล","NewColumnValue":"=\"กิตติพงษ์ แหลมผักแว่น\""}, {"ColumnToEdit":"Export to XLSX","NewColumnValue":"=TRUE"}],"ColumnToEdit":"ชื่อ -นามสกุล","NewColumnValue":"=\"กิตติพงษ์ แหลมผัก แว่น\"","InputParametersUsed":null,"Prominence":"Do_Not_Display","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":true,"BulkApplicable":true}
```

</details>

## สร้างใบป่ะหน้า_จักรภัทร วงทอง

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | SET_COLUMN_VALUE |
| การแสดงผล | Do_Not_Display |
| ลำดับ | 1 |
| Bulk action | Yes |
| แก้ไขข้อมูล | Yes |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | ชื่อ - นามสกุล |
| ตั้งค่าคอลัมน์ | ชื่อ - นามสกุล |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
true
```

**ตั้งค่าเป็น:**

```
="จักรภัทร วงทอง"
```

<details><summary>With these properties (JSON)</summary>

```json
{"Assignments":[{"ColumnToEdit":"ชื่อ -นามสกุล","NewColumnValue":"=\"จักรภัทร วงทอง\""}, {"ColumnToEdit":"Export to XLSX","NewColumnValue":"=TRUE"}],"ColumnToEdit":"ชื่อ -นามสกุล","NewColumnValue":"=\"จักรภัทร วง ทอง\"","InputParametersUsed":null,"Prominence":"Do_Not_Display","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":true,"BulkApplicable":true}
```

</details>

## สร้างใบป่ะหน้า_พีระพล รูปแก้ว

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | SET_COLUMN_VALUE |
| การแสดงผล | Do_Not_Display |
| ลำดับ | 1 |
| Bulk action | Yes |
| แก้ไขข้อมูล | Yes |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | ชื่อ - นามสกุล |
| ตั้งค่าคอลัมน์ | ชื่อ - นามสกุล |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
true
```

**ตั้งค่าเป็น:**

```
="พีระพล รูปแก้ว"
```

<details><summary>With these properties (JSON)</summary>

```json
{"Assignments":[{"ColumnToEdit":"ชื่อ -นามสกุล","NewColumnValue":"=\"พีระพล รูปแก้ว\""}, {"ColumnToEdit":"Export to XLSX","NewColumnValue":"=TRUE"}],"ColumnToEdit":"ชื่อ -นามสกุล","NewColumnValue":"=\"พีระพล รูป แก้ว\"","InputParametersUsed":null,"Prominence":"Do_Not_Display","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":true,"BulkApplicable":true}
```

</details>

## สร้างใบป่ะหน้า_อชิตพล ยังยิ้ม

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | SET_COLUMN_VALUE |
| การแสดงผล | Do_Not_Display |
| ลำดับ | 1 |
| Bulk action | Yes |
| แก้ไขข้อมูล | Yes |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | ชื่อ - นามสกุล |
| ตั้งค่าคอลัมน์ | ชื่อ - นามสกุล |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
true
```

**ตั้งค่าเป็น:**

```
="อชิตพล ยังยิ้ม"
```

<details><summary>With these properties (JSON)</summary>

```json
{"Assignments":[{"ColumnToEdit":"ชื่อ -นามสกุล","NewColumnValue":"=\"อชิตพล ยังยิ้ม\""}, {"ColumnToEdit":"Export to XLSX","NewColumnValue":"=TRUE"}],"ColumnToEdit":"ชื่อ -นามสกุล","NewColumnValue":"=\"อชิตพล ยัง ยิ้ม\"","InputParametersUsed":null,"Prominence":"Do_Not_Display","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":true,"BulkApplicable":true}
```

</details>

## สร้างใบป่ะหน้า_ธีรยุทธ นราทอง

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | SET_COLUMN_VALUE |
| การแสดงผล | Do_Not_Display |
| ลำดับ | 1 |
| Bulk action | Yes |
| แก้ไขข้อมูล | Yes |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | ชื่อ - นามสกุล |
| ตั้งค่าคอลัมน์ | ชื่อ - นามสกุล |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
true
```

**ตั้งค่าเป็น:**

```
="ธีรยุทธ นราทอง"
```

<details><summary>With these properties (JSON)</summary>

```json
{"Assignments":[{"ColumnToEdit":"ชื่อ -นามสกุล","NewColumnValue":"=\"ธีรยุทธ นราทอง\""}, {"ColumnToEdit":"Export to XLSX","NewColumnValue":"=TRUE"}],"ColumnToEdit":"ชื่อ -นามสกุล","NewColumnValue":"=\"ธีรยุทธ นรา ทอง\"","InputParametersUsed":null,"Prominence":"Do_Not_Display","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":true,"BulkApplicable":true}
```

</details>

## สร้างใบป่ะหน้า_จิรายุ โคตรวงษ์

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | SET_COLUMN_VALUE |
| การแสดงผล | Do_Not_Display |
| ลำดับ | 1 |
| Bulk action | Yes |
| แก้ไขข้อมูล | Yes |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | ชื่อ - นามสกุล |
| ตั้งค่าคอลัมน์ | ชื่อ - นามสกุล |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
true
```

**ตั้งค่าเป็น:**

```
="จิรายุ โคตรวงษ์"
```

<details><summary>With these properties (JSON)</summary>

```json
{"Assignments":[{"ColumnToEdit":"ชื่อ -นามสกุล","NewColumnValue":"=\"จิรายุ โคตรวงษ์\""}, {"ColumnToEdit":"Export to XLSX","NewColumnValue":"=TRUE"}],"ColumnToEdit":"ชื่อ -นามสกุล","NewColumnValue":"=\"จิรายุ โคตร วงษ์\"","InputParametersUsed":null,"Prominence":"Do_Not_Display","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":true,"BulkApplicable":true}
```

</details>

## สร้างใบป่ะหน้า_ทัดเทพ พรมมา

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | SET_COLUMN_VALUE |
| การแสดงผล | Do_Not_Display |
| ลำดับ | 1 |
| Bulk action | Yes |
| แก้ไขข้อมูล | Yes |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | ชื่อ - นามสกุล |
| ตั้งค่าคอลัมน์ | ชื่อ - นามสกุล |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
true
```

**ตั้งค่าเป็น:**

```
="ทัดเทพ พรมมา"
```

<details><summary>With these properties (JSON)</summary>

```json
{"Assignments":[{"ColumnToEdit":"ชื่อ -นามสกุล","NewColumnValue":"=\"ทัดเทพ พรมมา\""}, {"ColumnToEdit":"Export to XLSX","NewColumnValue":"=TRUE"}],"ColumnToEdit":"ชื่อ -นามสกุล","NewColumnValue":"=\"ทัดเทพ พรม มา\"","InputParametersUsed":null,"Prominence":"Do_Not_Display","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":true,"BulkApplicable":true}
```

</details>

## สร้างใบป่ะหน้า_พงศธร หมวดไธสง

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | SET_COLUMN_VALUE |
| การแสดงผล | Do_Not_Display |
| ลำดับ | 1 |
| Bulk action | Yes |
| แก้ไขข้อมูล | Yes |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | ชื่อ - นามสกุล |
| ตั้งค่าคอลัมน์ | ชื่อ - นามสกุล |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
true
```

**ตั้งค่าเป็น:**

```
="พงศธร หมวดไธสง"
```

<details><summary>With these properties (JSON)</summary>

```json
{"Assignments":[{"ColumnToEdit":"ชื่อ -นามสกุล","NewColumnValue":"=\"พงศธร หมวดไธสง\""}, {"ColumnToEdit":"Export to XLSX","NewColumnValue":"=TRUE"}],"ColumnToEdit":"ชื่อ -นามสกุล","NewColumnValue":"=\"พงศธร หมวดไธ สง\"","InputParametersUsed":null,"Prominence":"Do_Not_Display","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":true,"BulkApplicable":true}
```

</details>

## สร้างใบป่ะหน้า_เกียรติศักดิ์ พินิจเมือง

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | SET_COLUMN_VALUE |
| การแสดงผล | Do_Not_Display |
| ลำดับ | 1 |
| Bulk action | Yes |
| แก้ไขข้อมูล | Yes |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | ชื่อ - นามสกุล |
| ตั้งค่าคอลัมน์ | ชื่อ - นามสกุล |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
true
```

**ตั้งค่าเป็น:**

```
="เกียรติศักดิ์ พินิจเมือง"
```

<details><summary>With these properties (JSON)</summary>

```json
{"Assignments":[{"ColumnToEdit":"ชื่อ -นามสกุล","NewColumnValue":"=\"เกียรติศักดิ์ พินิจเมือง\""}, {"ColumnToEdit":"Export to XLSX","NewColumnValue":"=TRUE"}],"ColumnToEdit":"ชื่อ -นามสกุล","NewColumnValue":"=\"เกียรติศักดิ์ พินิจ เมือง\"","InputParametersUsed":null,"Prominence":"Do_Not_Display","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":true,"BulkApplicable":true}
```

</details>

## สร้างใบป่ะหน้า_เกียรติศักดิ์ ยอมใหญ่

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | SET_COLUMN_VALUE |
| การแสดงผล | Do_Not_Display |
| ลำดับ | 1 |
| Bulk action | Yes |
| แก้ไขข้อมูล | Yes |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | ชื่อ - นามสกุล |
| ตั้งค่าคอลัมน์ | ชื่อ - นามสกุล |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
true
```

**ตั้งค่าเป็น:**

```
="เกียรติศักดิ์ ยอมใหญ่"
```

<details><summary>With these properties (JSON)</summary>

```json
{"Assignments":[{"ColumnToEdit":"ชื่อ -นามสกุล","NewColumnValue":"=\"เกียรติศักดิ์ ยอมใหญ่\""}, {"ColumnToEdit":"Export to XLSX","NewColumnValue":"=TRUE"}],"ColumnToEdit":"ชื่อ -นามสกุล","NewColumnValue":"=\"เกียรติศักดิ์ ยอม ใหญ่\"","InputParametersUsed":null,"Prominence":"Do_Not_Display","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":true,"BulkApplicable":true}
```

</details>

## PDFพนักงานcsv

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

## สร้างใบป่ะหน้า_สิทธิชัย ทิศวงค์

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | SET_COLUMN_VALUE |
| การแสดงผล | Do_Not_Display |
| ลำดับ | 1 |
| Bulk action | Yes |
| แก้ไขข้อมูล | Yes |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | ชื่อ - นามสกุล |
| ตั้งค่าคอลัมน์ | ชื่อ - นามสกุล |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
true
```

**ตั้งค่าเป็น:**

```
="สิทธิชัย ทิศวงค์"
```

<details><summary>With these properties (JSON)</summary>

```json
{"Assignments":[{"ColumnToEdit":"ชื่อ -นามสกุล","NewColumnValue":"=\"สิทธิชัย ทิศวงค์\""}, {"ColumnToEdit":"Export to XLSX","NewColumnValue":"=TRUE"}],"ColumnToEdit":"ชื่อ -นามสกุล","NewColumnValue":"=\"สิทธิชัย ทิศ วงค์\"","InputParametersUsed":null,"Prominence":"Do_Not_Display","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":true,"BulkApplicable":true}
```

</details>

## สร้างใบป่ะหน้า_ไนยชน วงศ์บุญมา

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | SET_COLUMN_VALUE |
| การแสดงผล | Do_Not_Display |
| ลำดับ | 1 |
| Bulk action | Yes |
| แก้ไขข้อมูล | Yes |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | ชื่อ - นามสกุล |
| ตั้งค่าคอลัมน์ | ชื่อ - นามสกุล |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
true
```

**ตั้งค่าเป็น:**

```
="ไนยชน วงศ์บุญมา"
```

<details><summary>With these properties (JSON)</summary>

```json
{"Assignments":[{"ColumnToEdit":"ชื่อ -นามสกุล","NewColumnValue":"=\"ไนยชน วงศ์บุญมา\""}, {"ColumnToEdit":"Export to XLSX","NewColumnValue":"=TRUE"}],"ColumnToEdit":"ชื่อ -นามสกุล","NewColumnValue":"=\"ไนยชน วงศ์บุญ มา\"","InputParametersUsed":null,"Prominence":"Do_Not_Display","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":true,"BulkApplicable":true}
```

</details>

