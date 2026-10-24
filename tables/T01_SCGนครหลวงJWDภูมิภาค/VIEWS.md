# Views ที่เกี่ยวกับตาราง SCGนครหลวงJWDภูมิภาค

รวม **4 views**

## SCGนครหลวงJWDภูมิภาค

| คุณสมบัติ | ค่า |
|---|---|
| ชนิด View | table |
| ตำแหน่ง | menu |
| สร้างโดย | App owner |
| การมองเห็น | ALWAYS |
| ลำดับเมนู | 1 |

<details><summary>View configuration (JSON)</summary>

```json
{"ColumnWidth": "Default", "EnableQuickEdit": true, "ColumnOrder": ["head", "ผลการตรวจสอบงานส่ง", "ที่อยู่ปลายทาง", "LAT", "LONG", "จุดส่งสินค้าปลายทาง", "Email พนักงาน", "วันที่ส่งสินค้า", "เวลาที่ส่งสินค้า", "ชื่อ - นามสกุล", "ทะเบียนรถ", "Shipment No", "Invoice No", "รหัสลูกค้า", "ชื่อเจ้าของสินค้า", "ชื่อปลายทาง", "หมายเหตุ", "ที่อยู่ปลายทาง_LatLong_Api", "ระยะทางจากคลัง_Km", "พิกัดตอนกดบันทึกงาน", "เวลาเริ่มกรอกงาน", "เวลาบันทึกงานสำเร็จ", "ระยะขยับจากจุดเริ่มต้น_เมตร", "ระยะเวลาใช้งาน_นาที", "ความเร็วการเคลื่อนที่_เมตร_นาที"], "GroupBy": [{"Column": "เดือน", "Order": "Descending"}, {"Column": "วันที่ส่ง สินค้า", "Order": "Descending"}, {"Column": "ชื่อ -นามสกุล", "Order": "Descending"}, {"Column": "Shipment No", "Order": "Descending"}, {"Column": "_RowNumber", "Order": "Descending"}], "GroupAggregate": "NONE", "SortBy": [], "PrimarySortColumn": null, "IsPrimarySortDescending": false, "Events": [{"EventType": "Row Selected", "EventAction": "**auto**"}], "Icon": "fa-list-ul", "IconRunnerUps": null, "MenuOrder": 1}
```

</details>

## SCGนครหลวงJWDภูมิภาค_Detail

| คุณสมบัติ | ค่า |
|---|---|
| ชนิด View | detail |
| ตำแหน่ง | ref |
| ActionType | Automatic |
| สร้างโดย | System |
| การมองเห็น | ALWAYS |
| ลำดับเมนู | 1 |

<details><summary>View configuration (JSON)</summary>

```json
{"MainSlideshowImageColumn": "**none**", "DetailContentColumn": "**none**", "HeaderColumns": [], "QuickEditColumns": ["วันที่ส่งสินค้า", "เวลาที่ส่งสินค้า", "จุดส่งสินค้าปลายทาง", "Shipment No", "Invoice No", "รูปถ่าย บิลส่งสินค้า", "รูปสินค้าตอนส่ง", "รูปหน้าร้าน / บ้าน", "หมายเหตุ", "ID_พนักงาน", "รหัสลูกค้า", "ชื่อเจ้าของสินค้า", "ชื่อปลาย ทาง", "ที่อยู่ปลายทาง", "ID_Doc_Return", "SM_Link_SCG"], "ColumnOrder": [], "ImageStyle": "Fill", "Layout": null, "UseCardLayout": false, "DisplayMode": "Automatic", "MaxNestedRows": 5, "SlideshowMode": true, "DesktopSplitMode": "Split view", "UseDesktopMultiColumn": true, "SortBy": [{"Column": "_RowNumber", "Order": "Descending"}], "PrimarySortColumn": null, "IsPrimarySortDescending": false, "Events": [], "Icon": "fa-indent", "IconRunnerUps": null, "MenuOrder": 1}
```

</details>

## SCGนครหลวงJWDภูมิภาค_Form

| คุณสมบัติ | ค่า |
|---|---|
| ชนิด View | form |
| ตำแหน่ง | ref |
| สร้างโดย | System |
| การมองเห็น | ALWAYS |
| ลำดับเมนู | 1 |

<details><summary>View configuration (JSON)</summary>

```json
{"ColumnOrder": ["วันที่ส่งสินค้า", "เวลาที่ส่งสินค้า", "จุดส่งสินค้าปลายทาง", "รูปหน้าร้าน / บ้าน", "เวลาถ่ายรูปหน้าร้าน_หน้าบ้าน", "ID_พนักงาน", "ชื่อ - นามสกุล", "ทะเบียนรถ", "Shipment No", "Document_Return", "Invoice No", "Image_Document_Return", "รูปถ่ายบิลส่งสินค้า", "รูปสินค้าตอนส่ง", "ชื่อปลายทาง", "รหัสลูกค้า", "ชื่อเจ้าของสินค้า", "Email พนักงาน", "หมายเหตุ", "ที่อยู่ปลายทาง"], "AutoSave": false, "AutoReopen": false, "FinishView": "**Automatic**", "RowKey": "", "FormStyle": "Automatic", "PageStyle": "Automatic", "FormFooterStyle": "Bottom", "MaxNestedRows": 5, "AudioInput": false, "Events": [{"EventType": "Form Saved", "EventAction": "**auto**"}], "Icon": "fa-edit", "IconRunnerUps": null, "MenuOrder": 1}
```

</details>

## SCGนครหลวงJWDภูมิภาค_Inline

| คุณสมบัติ | ค่า |
|---|---|
| ชนิด View | table |
| ตำแหน่ง | ref |
| สร้างโดย | System |
| การมองเห็น | ALWAYS |
| ลำดับเมนู | 1 |

<details><summary>View configuration (JSON)</summary>

```json
{"ColumnWidth": "Default", "EnableQuickEdit": true, "ColumnOrder": [], "GroupBy": [{"Column": "Shipment No", "Order": "Descending"}, {"Column": "_RowNumber", "Order": "Descending"}], "GroupAggregate": "NONE", "SortBy": [{"Column": "_RowNumber", "Order": "Ascending"}], "PrimarySortColumn": null, "IsPrimarySortDescending": false, "Events": [{"EventType": "Row Selected", "EventAction": "**auto**"}], "Icon": "fa-list-ul", "IconRunnerUps": null, "MenuOrder": 1}
```

</details>

