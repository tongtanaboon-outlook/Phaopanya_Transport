# Actions ของตาราง สรุปเบิกส่วนต่าง

รวม **6 actions**

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
| ผูกกับคอลัมน์ | _ComputedKey_ID_SCGนครหลวงJWDภูมิภาค |
| ตั้งค่าคอลัมน์ | _ComputedKey_ID_SCGนครหลวงJWDภูมิภาค |
| ปิด sync อัตโนมัติ | No |
| การมองเห็น | ALWAYS |
| ไอคอน |  |

**แสดงเมื่อเงื่อนไขนี้เป็นจริง:**

```
NOT(ISBLANK([_ComputedKey_ID_SCGนครหลวงJWDภูมิภาค]))
```

<details><summary>With these properties (JSON)</summary>

```json
{"NavigateTarget":"CONCATENATE(\"#page=detail&table=SCG%E0%B8%99%E0%B8%84%E0%B8%A3%E0%B8%AB%E0%B8%A5%E0%B8%A7%E0%B8%87JWD%E0%B8%A0%E0%B8%B9%E0%B8%A1%E0%B8%B4%E0%B8%A0%E0%B8%B2%E0%B8%84&row=\", ENCODEURL([_ComputedKey_ID_SCGนครหลวงJWDภูมิภาค]))","Prominence":"Display_Inline","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":false,"BulkApplicable":false}
```

</details>

## Clearหน้าจอสรุปส่วนต่าง

| คุณสมบัติ | ค่า |
|---|---|
| ประเภทการทำงาน (Do this) | SET_COLUMN_VALUE |
| การแสดงผล | Display_Prominently |
| ลำดับ | 1 |
| Bulk action | Yes |
| แก้ไขข้อมูล | Yes |
| ต้องยืนยัน | No |
| ผูกกับคอลัมน์ | ชื่อ - นามสกุล |
| ตั้งค่าคอลัมน์ | วันที่เริ่มต้น |
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
{"Assignments":[{"ColumnToEdit":"วันที่เริ่ม ต้น","NewColumnValue":"=\"\""},{"ColumnToEdit":"วันที่สิ้น สุด","NewColumnValue":"=\"\""},{"ColumnToEdit":"Export to Excel","NewColumnValue":"=\"\""}],"ColumnToEdit":"วันที่เริ่ม ต้น","NewColumnValue":"=\"\"","InputParametersUsed":null,"Pro minence":"Display_Prominently","NeedsConfirmation":false,"ConfirmationMessage":"","ModifiesData":true,"BulkApplicable":true}
```

</details>

## สรุปเบิกส่วนต่างcsv

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

