# Actions ของตาราง ScanDocs

รวม **7 actions**

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

## Compose Email (Scan_By)

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | EMAIL |
| การแสดงผล | Display_Inline |
| ลำดับ | 1 |
| Bulk action | No |
| แก้ไขข้อมูล | No |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | Scan_By |
| ตั้งค่าคอลัมน์ | Scan_By |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
NOT(ISBLANK([Scan_By]))
```

<details><summary>With these properties (JSON)</summary>

```json
{"EmailTo":" [Scan_By]","Subject":null,"Body":null,"Prominence":"Display_Inline","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":false,"BulkApplicable":false}
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

## ScanStatus

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
{"ReferencedTable":"ตารางงานประจำ วัน","ReferencedRows":"=SELECT(\n ตารางงานประจำวัน[ID_งานประจำวัน],\n IN([Invoice No], LIST([_THISROW].[Scan_Invoice], [_THISROW].[Select_Invoice]))\n)","ReferencedAction":"Update ScanStatus","InputAssignments": [],"InputParametersUsed":null,"Prominence":"Do_Not_Display","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":false,"BulkApplicable":true}
```

</details>

## View Ref (Invoice_No)

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | NAVIGATE_APP |
| การแสดงผล | Display_Inline |
| ลำดับ | 1 |
| Bulk action | No |
| แก้ไขข้อมูล | No |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | Invoice_No |
| ตั้งค่าคอลัมน์ | Invoice_No |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
NOT(ISBLANK([Invoice_No]))
```

<details><summary>With these properties (JSON)</summary>

```json
{"NavigateTarget":"CONCATENATE(\"#page=detail&table=%E0%B8%95%E0%B8%B2%E0%B8%A3%E0%B8%B2%E0%B8%87%E0%B8%87%E0%B8%B2%E0%B8%99%E0%B8%9B%E0%B8%A3%E0%B8%B0%E0%B8%88%E0%B8%B3%E0%B8%A7%E0%B8%B1%E0%B8%99&row=\", ENCODEURL([Invoice_No]) )","Prominence":"Display_Inline","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":false,"BulkApplicable":false}
```

</details>

## Update Action - 1

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | REF_ACTION |
| การแสดงผล | Display_Prominently |
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
{"ReferencedTable":"ตารางงานประจำ วัน","ReferencedRows":"=SELECT(\n ตารางงานประจำวัน[ID_งานประจำวัน],\n IN([Invoice No], LIST([_THISROW].[Scan_Invoice], [_THISROW].[Select_Invoice]))\n)","ReferencedAction":"Update ScanStatus","InputAssignments": [],"InputParametersUsed":null,"Prominence":"Display_Prominently","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":false,"BulkApplicable":true}
```

</details>

