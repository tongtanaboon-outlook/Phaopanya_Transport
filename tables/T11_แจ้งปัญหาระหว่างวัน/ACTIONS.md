# Actions ของตาราง แจ้งปัญหาระหว่างวัน

รวม **14 actions**

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

## ส่งรูปแจ้งปัญหา

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | NAVIGATE_DIFFERENT_APP |
| การแสดงผล | Display_Prominently |
| ลำดับ | 1 |
| Bulk action | No Confirmation Message กดส่งรูปแจ้งปัญหา เพื่อเข้าสู่ขั้นตอนการเพื่มรูปถ่าย |
| แก้ไขข้อมูล | No |
| ต้องยืนยัน | Yes |
| ผูกกับคอลัมน์ | ID_วางบิล |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
true
```

<details><summary>With these properties (JSON)</summary>

```json
{"NavigateTarget":"=LINKTOAPP(\"1c544f2c-efb8-41ee-8cc5-ac5573f10e5c\") \n& LINKTOROW([ID_แจ้งปัญหาระหว่างวัน], \"แจ้งปัญหาระหว่าง วัน_Detail\")","Prominence":"Display_Prominently","NeedsConfirmation":true,"ConfirmationMessage":"กดส่งรูปแจ้งปัญหา เพื่อเข้าสู่ขั้นตอนการเพื่มรูป ถ่าย","ModifiesData":false,"BulkApplicable":false}
```

</details>

## View Map (Lat/Long)

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | NAVIGATE_APP |
| การแสดงผล | Display_Inline |
| ลำดับ | 1 |
| Bulk action | No |
| แก้ไขข้อมูล | No |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | Lat/Long |
| ตั้งค่าคอลัมน์ | Lat/Long |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
NOT(ISBLANK([Lat/Long]))
```

<details><summary>With these properties (JSON)</summary>

```json
{"NavigateTarget":"CONCATENATE(\"#page=map&table=%E0%B9%81%E0%B8%88%E0%B9%89%E0%B8%87%E0%B8%9B%E0%B8%B1%E0%B8%8D%E0%B8%AB%E0%B8%B2%E0%B8%A3%E0%B8%B0%E0%B8%AB%E0%B8%A7%E0%B9%88%E0%B8%B2%E0%B8%87%E0%B8%A7%E0%B8%B1%E0%B8%99&mapcolumn=Lat%2FLong&row=\", ENCODEURL([_THISROW]))","Prominence":"Display_Inline","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":false,"BulkApplicable":false}
```

</details>

## เพิ่มข้อมูลแจ้งปัญหาในจุดส่งงาน

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | ADD_RECORD_TO |
| การแสดงผล | Do_Not_Display |
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
{"ReferencedTable":"SCGนครหลวงJWDภูมิภาค","Assignments": [{"ColumnToEdit":"head","NewColumnValue":"=[หมายเหตุ]"}, {"ColumnToEdit":"ID_SCGนครหลวงJWDภูมิภาค","NewColumnValue":"=UNIQUEID()"},{"ColumnToEdit":"วันที่ส่ง สินค้า","NewColumnValue":"=TODAY()"},{"ColumnToEdit":"เวลาที่ส่งสินค้า","NewColumnValue":"=TIME([วันที่+เวลา])"}, {"ColumnToEdit":"จุดส่งสินค้าปลายทาง","NewColumnValue":"= [Lat/Long]"},{"ColumnToEdit":"Shipment No","NewColumnValue":"=[Shipment No]"}, {"ColumnToEdit":"Invoice No","NewColumnValue":"=SPLIT(TEXT([Invoice No]), \" , \")"}, {"ColumnToEdit":"รูปถ่ายบิลส่งสินค้า","NewColumnValue":"= [รูป1]"},{"ColumnToEdit":"รูปสินค้าตอนส่ง","NewColumnValue":"=[รูป2]"},{"ColumnToEdit":"รูปหน้าร้าน / บ้าน","NewColumnValue":"=[เพิ่มรูปแคปหน้าจอ นำกลับคืนคลัง]"}, {"ColumnToEdit":"หมายเหตุ","NewColumnValue":"=[ใส่ข้อมูลการแจ้งปัญหา เพื่อนับจุดส่งงาน]"}, {"ColumnToEdit":"ID_พนักงาน","NewColumnValue":"= [ID_พนักงาน]"},{"ColumnToEdit":"Email พนักงาน","NewColumnValue":"=[Email พนักงาน]"}, {"ColumnToEdit":"SM_Link_SCG","NewColumnValue":"= [SM_Link]"},{"ColumnToEdit":"พิกัดตอนกดบันทึก งาน","NewColumnValue":"=[LatLong_ตรวจสอบ]"}, {"ColumnToEdit":"เวลาบันทึกงาน สำเร็จ","NewColumnValue":"=TIMENOW()"}],"InputParametersUsed":null,"Prominence":"Do_Not_Display","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":true,"BulkApplicable":true}
```

</details>

## แจ้งปัญหาระหว่างวันcsv

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

## View Ref (SM_Link)

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | NAVIGATE_APP |
| การแสดงผล | Display_Inline |
| ลำดับ | 1 |
| Bulk action | No |
| แก้ไขข้อมูล | No |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | SM_Link |
| ตั้งค่าคอลัมน์ | SM_Link |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
NOT(ISBLANK([SM_Link]))
```

<details><summary>With these properties (JSON)</summary>

```json
{"NavigateTarget":"CONCATENATE(\"#page=detail&table=%E0%B8%95%E0%B8%B2%E0%B8%A3%E0%B8%B2%E0%B8%87%E0%B8%87%E0%B8%B2%E0%B8%99%E0%B8%9B%E0%B8%A3%E0%B8%B0%E0%B8%88%E0%B8%B3%E0%B8%A7%E0%B8%B1%E0%B8%99&row=\", ENCODEURL([SM_Link]) )","Prominence":"Display_Inline","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":false,"BulkApplicable":false}
```

</details>

## View Ref (RT_Link)

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | NAVIGATE_APP |
| การแสดงผล | Display_Inline |
| ลำดับ | 1 |
| Bulk action | No |
| แก้ไขข้อมูล | No |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | RT_Link |
| ตั้งค่าคอลัมน์ | RT_Link |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
NOT(ISBLANK([RT_Link]))
```

<details><summary>With these properties (JSON)</summary>

```json
{"NavigateTarget":"CONCATENATE(\"#page=detail&table=%E0%B8%82%E0%B9%89%E0%B8%AD%E0%B8%A1%E0%B8%B9%E0%B8%A5%E0%B8%87%E0%B8%B2%E0%B8%99RT&row=\", ENCODEURL([RT_Link]) )","Prominence":"Display_Inline","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":false,"BulkApplicable":false}
```

</details>

## ACT_Create_SCG_Flow

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | COMPOSITE |
| การแสดงผล | Do_Not_Display |
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
{"Actions":[{"ActionName":"เพิ่มข้อมูลแจ้งปัญหาในจุดส่งงาน"}, {"ActionName":"New Action"}],"Prominence":"Do_Not_Display","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":true,"BulkApplicable":true}
```

</details>

## New Action

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | REF_ACTION |
| การแสดงผล | Do_Not_Display |
| ลำดับ | 1 |
| Bulk action | Yes |
| แก้ไขข้อมูล | No |
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
{"ReferencedTable":"ตารางงานประจำ วัน","ReferencedRows":"=SELECT(ตารางงานประจำวัน[ID_งานประจำวัน], \n IN([Invoice No], [_THISROW].[Invoice No])\n)","ReferencedAction":"Mark_As_Delivered_not","InputAssignments": [],"InputParametersUsed":null,"Prominence":"Do_Not_Display","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":false,"BulkApplicable":true}
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

## View Map (LatLong_ตรวจสอบ)

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | NAVIGATE_APP |
| การแสดงผล | Display_Inline |
| ลำดับ | 1 |
| Bulk action | No |
| แก้ไขข้อมูล | No |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | LatLong_ตรวจสอบ |
| ตั้งค่าคอลัมน์ | LatLong_ตรวจสอบ |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
NOT(ISBLANK([LatLong_ตรวจสอบ]))
```

<details><summary>With these properties (JSON)</summary>

```json
{"NavigateTarget":"CONCATENATE(\"#page=map&table=%E0%B9%81%E0%B8%88%E0%B9%89%E0%B8%87%E0%B8%9B%E0%B8%B1%E0%B8%8D%E0%B8%AB%E0%B8%B2%E0%B8%A3%E0%B8%B0%E0%B8%AB%E0%B8%A7%E0%B9%88%E0%B8%B2%E0%B8%87%E0%B8%A7%E0%B8%B1%E0%B8%99&mapcolumn=LatLong_%E0%B8%95%E0%B8%A3%E0%B8%A7%E0%B8%88%E0%B8%AA%E0%B8%AD%E0%B8%9A&row=\", ENCODEURL([_THISROW]))","Prominence":"Display_Inline","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":false,"BulkApplicable":false}
```

</details>

