# Actions ของตาราง SCGนครหลวงJWDภูมิภาค

รวม **13 actions**

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

## View Map (จุดส่งสินค้าปลายทาง)

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | NAVIGATE_APP |
| การแสดงผล | Display_Inline |
| ลำดับ | 1 |
| Bulk action | No |
| แก้ไขข้อมูล | No |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | จุดส่งสินค้าปลายทาง |
| ตั้งค่าคอลัมน์ | จุดส่งสินค้าปลายทาง |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
NOT(ISBLANK([จุดส่งสินค้าปลายทาง]))
```

<details><summary>With these properties (JSON)</summary>

```json
{"NavigateTarget":"CONCATENATE(\"#page=map&table=SCG%E0%B8%99%E0%B8%84%E0%B8%A3%E0%B8%AB%E0%B8%A5%E0%B8%A7%E0%B8%87JWD%E0%B8%A0%E0%B8%B9%E0%B8%A1%E0%B8%B4%E0%B8%A0%E0%B8%B2%E0%B8%84&mapcolumn=%E0%B8%88%E0%B8%B8%E0%B8%94%E0%B8%AA%E0%B9%88%E0%B8%87%E0%B8%AA%E0%B8%B4%E0%B8%99%E0%B8%84%E0%B9%89%E0%B8%B2%E0%B8%9B%E0%B8%A5%E0%B8%B2%E0%B8%A2%E0%B8%97%E0%B8%B2%E0%B8%87&row=\", ENCODEURL([_THISROW]))","Prominence":"Display_Inline","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":false,"BulkApplicable":false}
```

</details>

## View Ref (ID_เอกสารนำกลับคืนคลัง)

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | NAVIGATE_APP |
| การแสดงผล | Display_Inline |
| ลำดับ | 1 |
| Bulk action | No |
| แก้ไขข้อมูล | No |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | ID_Doc_Return |
| ตั้งค่าคอลัมน์ | ID_Doc_Return |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
NOT(ISBLANK([ID_Doc_Return]))
```

<details><summary>With these properties (JSON)</summary>

```json
{"NavigateTarget":"CONCATENATE(\"#page=detail&table=Doc_Return&row=\", ENCODEURL([ID_Doc_Return]) )","Prominence":"Display_Inline","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":false,"BulkApplicable":false}
```

</details>

## View Map (คลังสินค้า เอสซีจี เจดับเบิ้ลยูดี วังน้อย)

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | NAVIGATE_APP |
| การแสดงผล | Display_Inline |
| ลำดับ | 1 |
| Bulk action | No |
| แก้ไขข้อมูล | No |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | คลังสินค้า เอสซีจี เจดับเบิ้ลยูดี วังน้อย |
| ตั้งค่าคอลัมน์ | คลังสินค้า เอสซีจี เจดับเบิ้ลยูดี วังน้อย |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
NOT(ISBLANK([คลังสินค้า เอสซีจี เจดับเบิ้ลยูดี วังน้อย]))
```

<details><summary>With these properties (JSON)</summary>

```json
{"NavigateTarget":"CONCATENATE(\"#page=map&table=SCG%E0%B8%99%E0%B8%84%E0%B8%A3%E0%B8%AB%E0%B8%A5%E0%B8%A7%E0%B8%87JWD%E0%B8%A0%E0%B8%B9%E0%B8%A1%E0%B8%B4%E0%B8%A0%E0%B8%B2%E0%B8%84&mapcolumn=%E0%B8%84%E0%B8%A5%E0%B8%B1%E0%B8%87%E0%B8%AA%E0%B8%B4%E0%B8%99%E0%B8%84%E0%B9%89%E0%B8%B2%20%E0%B9%80%E0%B8%AD%E0%B8%AA%E0%B8%8B%E0%B8%B5%E0%B8%88%E0%B8%B5%20%E0%B9%80%E0%B8%88%E0%B8%94%E0%B8%B1%E0%B8%9A%E0%B9%80%E0%B8%9A%E0%B8%B4%E0%B9%89%E0%B8%A5%E0%B8%A2%E0%B8%B9%E0%B8%94%E0%B8%B5%20%E0%B8%A7%E0%B8%B1%E0%B8%87%E0%B8%99%E0%B9%89%E0%B8%AD%E0%B8%A2&row=\", ENCODEURL([_THISROW]))","Prominence":"Display_Inline","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":false,"BulkApplicable":false}
```

</details>

## View Map (ที่อยู่ปลายทาง_LatLong_Api)

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | NAVIGATE_APP |
| การแสดงผล | Display_Inline |
| ลำดับ | 1 |
| Bulk action | No |
| แก้ไขข้อมูล | No |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | ที่อยู่ปลายทาง_LatLong_Api |
| ตั้งค่าคอลัมน์ | ที่อยู่ปลายทาง_LatLong_Api |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
NOT(ISBLANK([ที่อยู่ปลายทาง_LatLong_Api]))
```

<details><summary>With these properties (JSON)</summary>

```json
{"NavigateTarget":"CONCATENATE(\"#page=map&table=SCG%E0%B8%99%E0%B8%84%E0%B8%A3%E0%B8%AB%E0%B8%A5%E0%B8%A7%E0%B8%87JWD%E0%B8%A0%E0%B8%B9%E0%B8%A1%E0%B8%B4%E0%B8%A0%E0%B8%B2%E0%B8%84&mapcolumn=%E0%B8%97%E0%B8%B5%E0%B9%88%E0%B8%AD%E0%B8%A2%E0%B8%B9%E0%B9%88%E0%B8%9B%E0%B8%A5%E0%B8%B2%E0%B8%A2%E0%B8%97%E0%B8%B2%E0%B8%87_LatLong_Api&row=\", ENCODEURL([_THISROW]))","Prominence":"Display_Inline","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":false,"BulkApplicable":false}
```

</details>

## SCGนครหลวงJWDภูมิภาค_csv

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

## Process_Delivery_Status_Bot Action - 1

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
{"ReferencedTable":"ตารางงานประจำ วัน","ReferencedRows":"=SELECT(ตารางงานประจำวัน[ID_งานประจำวัน], \n IN([Invoice No], [_THISROW].[Invoice No])\n)","ReferencedAction":"Mark_As_Delivered","InputAssignments": [],"InputParametersUsed":null,"Prominence":"Do_Not_Display","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":false,"BulkApplicable":true}
```

</details>

## View Ref (SM_Link_SCG)

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | NAVIGATE_APP |
| การแสดงผล | Display_Inline |
| ลำดับ | 1 |
| Bulk action | No |
| แก้ไขข้อมูล | No |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | SM_Link_SCG |
| ตั้งค่าคอลัมน์ | SM_Link_SCG |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
NOT(ISBLANK([SM_Link_SCG]))
```

<details><summary>With these properties (JSON)</summary>

```json
{"NavigateTarget":"CONCATENATE(\"#page=detail&table=%E0%B8%95%E0%B8%B2%E0%B8%A3%E0%B8%B2%E0%B8%87%E0%B8%87%E0%B8%B2%E0%B8%99%E0%B8%9B%E0%B8%A3%E0%B8%B0%E0%B8%88%E0%B8%B3%E0%B8%A7%E0%B8%B1%E0%B8%99&row=\", ENCODEURL([SM_Link_SCG]) )","Prominence":"Display_Inline","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":false,"BulkApplicable":false}
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

## View Map (พิกัดตอนกดบันทึกงาน)

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | NAVIGATE_APP |
| การแสดงผล | Display_Inline |
| ลำดับ | 1 |
| Bulk action | No |
| แก้ไขข้อมูล | No |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | พิกัดตอนกดบันทึกงาน |
| ตั้งค่าคอลัมน์ | พิกัดตอนกดบันทึกงาน |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
NOT(ISBLANK([พิกัดตอนกดบันทึกงาน]))
```

<details><summary>With these properties (JSON)</summary>

```json
{"NavigateTarget":"CONCATENATE(\"#page=map&table=SCG%E0%B8%99%E0%B8%84%E0%B8%A3%E0%B8%AB%E0%B8%A5%E0%B8%A7%E0%B8%87JWD%E0%B8%A0%E0%B8%B9%E0%B8%A1%E0%B8%B4%E0%B8%A0%E0%B8%B2%E0%B8%84&mapcolumn=%E0%B8%9E%E0%B8%B4%E0%B8%81%E0%B8%B1%E0%B8%94%E0%B8%95%E0%B8%AD%E0%B8%99%E0%B8%81%E0%B8%94%E0%B8%9A%E0%B8%B1%E0%B8%99%E0%B8%97%E0%B8%B6%E0%B8%81%E0%B8%87%E0%B8%B2%E0%B8%99&row=\", ENCODEURL([_THISROW]))","Prominence":"Display_Inline","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":false,"BulkApplicable":false}
```

</details>

