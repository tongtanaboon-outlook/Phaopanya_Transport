# Views ที่เกี่ยวกับตาราง ตารางงานประจำวัน

รวม **10 views**

## ตารางงานประจำวัน

| คุณสมบัติ | ค่า |
|---|---|
| ชนิด View | table |
| ตำแหน่ง | menu |
| สร้างโดย | App owner |
| การมองเห็น | ALWAYS |
| ลำดับเมนู | 1 |

<details><summary>View configuration (JSON)</summary>

```json
{"ColumnWidth": "Default", "EnableQuickEdit": true, "ColumnOrder": ["LatLong_Actual", "Invoice No", "ID_งานประจำวัน", "ที่อยู่ปลายทาง_LatLong", "Email พนักงาน", "Plan Delivery", "Shipment No", "ชื่อ - นามสกุล", "ทะเบียนรถ", "รหัสผู้รับเหมา", "ชื่อผู้รับเหมา", "รหัสลูกค้า", "ชื่อเจ้าของสินค้า", "ชื่อปลายทาง", "ที่อยู่ปลายทาง", "ชื่อวัสดุ", "จำนวนสินค้า", "หน่วย", "ItemWeight", "DeliveryNo", "จำนวนปลายทาง_System", "รายชื่อปลายทาง_System", "ScanStatus", "DeliveryStatus", "จำนวนสินค้ารวมของร้านนี้", "น้ำหนักสินค้ารวมของร้านนี้", "จำนวน_Invoice_ที่ต้องสแกน", "ชื่อเจ้าของสินค้า_Invoice_ที่ต้องสแกน", "ShopKey", "จำนวนปลายทาง", "ลำดับแรก", "จำนวนจุดที่ส่งจริง", "เดือน", "Related SCGนครหลวงJWDภูมิภาคs", "Related แจ้งปัญหาระหว่างวันs", "Related ScanDocs"], "GroupBy": [{"Column": "Plan Delivery", "Order": "Descending"}, {"Column": "Shipment No", "Order": "Descending"}, {"Column": "_RowNumber", "Order": "Descending"}], "GroupAggregate": "MAX :: จำนวนปลายทาง_System", "SortBy": [{"Column": "_RowNumber", "Order": "Descending"}], "PrimarySortColumn": null, "IsPrimarySortDescending": false, "Events": [{"EventType": "RowSelected", "EventAction": "**auto**"}], "Icon": "fa-list-ul", "IconRunnerUps": null, "MenuOrder": 1}
```

</details>

## สรุปจำนวนจุดส่งสินค้า

| คุณสมบัติ | ค่า |
|---|---|
| ชนิด View | table |
| ตำแหน่ง | menu |
| สร้างโดย | App owner |
| การมองเห็น | ALWAYS |
| ลำดับเมนู | 1 |

<details><summary>View configuration (JSON)</summary>

```json
{"ColumnWidth": "Default", "EnableQuickEdit": false, "ColumnOrder": ["จำนวนปลายทาง", "Shipment No", "ชื่อ - นามสกุล", "ทะเบียนรถ", "Plan Delivery", "ชื่อปลายทาง"], "GroupBy": [{"Column": "Plan Delivery", "Order": "Descending"}, {"Column": "_RowNumber", "Order": "Descending"}], "GroupAggregate": "MAX :: จำนวนปลายทาง", "SortBy": [{"Column": "_RowNumber", "Order": "Descending"}], "PrimarySortColumn": null, "IsPrimarySortDescending": false, "Events": [{"EventType": "RowSelected", "EventAction": "**auto**"}], "Icon": "fa-list-ul", "IconRunnerUps": null, "MenuOrder": 1}
```

</details>

## Slice_Monitor_Today_Detail

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
{"MainSlideshowImageColumn": "**auto**", "DetailContentColumn": "**none**", "HeaderColumns": [], "QuickEditColumns": [], "ColumnOrder": [], "ImageStyle": "Fit", "Layout": null, "UseCardLayout": false, "DisplayMode": "Automatic", "MaxNestedRows": 5, "SlideshowMode": true, "DesktopSplitMode": "Split view", "UseDesktopMultiColumn": true, "SortBy": [], "PrimarySortColumn": null, "IsPrimarySortDescending": false, "Events": [], "Icon": "fa-indent", "IconRunnerUps": null, "MenuOrder": 1}
```

</details>

## Slice_Monitor_Today_Form

| คุณสมบัติ | ค่า |
|---|---|
| ชนิด View | form |
| ตำแหน่ง | ref |
| สร้างโดย | System |
| การมองเห็น | ALWAYS |
| ลำดับเมนู | 1 |

<details><summary>View configuration (JSON)</summary>

```json
{"ColumnOrder": null, "AutoSave": false, "AutoReopen": false, "FinishView": "**Automatic**", "RowKey": "", "FormStyle": "Automatic", "PageStyle": "Automatic", "FormFooterStyle": "Bottom", "MaxNestedRows": 5, "AudioInput": false, "Events": [{"EventType": "Form Saved", "EventAction": "**auto**"}], "Icon": "fa-edit", "IconRunnerUps": null, "MenuOrder": 1}
```

</details>

## ค้างสแกนวันนี้และเมื่อวาน_Detail

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
{"MainSlideshowImageColumn": "**auto**", "DetailContentColumn": "**none**", "HeaderColumns": [], "QuickEditColumns": [], "ColumnOrder": [], "ImageStyle": "Fit", "Layout": null, "UseCardLayout": false, "DisplayMode": "Automatic", "MaxNestedRows": 5, "SlideshowMode": true, "DesktopSplitMode": "Split view", "UseDesktopMultiColumn": true, "SortBy": [], "PrimarySortColumn": null, "IsPrimarySortDescending": false, "Events": [], "Icon": "fa-indent", "IconRunnerUps": null, "MenuOrder": 1}
```

</details>

## ค้างสแกนวันนี้และเมื่อวาน_Form

| คุณสมบัติ | ค่า |
|---|---|
| ชนิด View | form |
| ตำแหน่ง | ref |
| สร้างโดย | System |
| การมองเห็น | ALWAYS |
| ลำดับเมนู | 1 |

<details><summary>View configuration (JSON)</summary>

```json
{"ColumnOrder": null, "AutoSave": false, "AutoReopen": false, "FinishView": "**Automatic**", "RowKey": "", "FormStyle": "Automatic", "PageStyle": "Automatic", "FormFooterStyle": "Bottom", "MaxNestedRows": 5, "AudioInput": false, "Events": [{"EventType": "Form Saved", "EventAction": "**auto**"}], "Icon": "fa-edit", "IconRunnerUps": null, "MenuOrder": 1}
```

</details>

## ตารางงานประจำวัน_Detail

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
{"MainSlideshowImageColumn": "**auto**", "DetailContentColumn": "**none**", "HeaderColumns": [], "QuickEditColumns": [], "ColumnOrder": ["LatLong_Actual", "Invoice No", "ID_งานประจำวัน", "Plan Delivery", "Shipment No", "ชื่อ - นามสกุล", "ทะเบียนรถ", "รหัสผู้รับเหมา", "ชื่อผู้รับเหมา", "รหัสลูกค้า", "ชื่อเจ้าของสินค้า", "ชื่อปลายทาง", "ที่อยู่ปลายทาง", "ที่อยู่ปลายทาง_LatLong", "ชื่อวัสดุ", "จำนวนสินค้า", "หน่วย", "ItemWeight", "DeliveryNo", "จำนวนปลายทาง_System", "รายชื่อปลายทาง_System", "ScanStatus", "DeliveryStatus", "Email พนักงาน", "จำนวนสินค้ารวมของร้านนี้", "น้ำหนักสินค้ารวมของร้านนี้", "จำนวน_Invoice_ที่ต้องสแกน", "ชื่อเจ้าของสินค้า_Invoice_ที่ต้องสแกน", "ShopKey", "MATCH_KEY", "MD_ID", "LatLong_Actual_Status", "จำนวนปลายทาง", "ลำดับแรก", "จำนวนจุดที่ส่งจริง", "เดือน", "Related SCGนครหลวงJWDภูมิภาคs", "Related แจ้งปัญหาระหว่างวันs", "Related ScanDocs"], "ImageStyle": "Fill", "Layout": null, "UseCardLayout": false, "DisplayMode": "Automatic", "MaxNestedRows": 5, "SlideshowMode": true, "DesktopSplitMode": "Split view", "UseDesktopMultiColumn": true, "SortBy": [{"Column": "_RowNumber", "Order": "Descending"}], "PrimarySortColumn": null, "IsPrimarySortDescending": false, "Events": [], "Icon": "fa-indent", "IconRunnerUps": null, "MenuOrder": 1}
```

</details>

## ตารางงานประจำวัน_Form

| คุณสมบัติ | ค่า |
|---|---|
| ชนิด View | form |
| ตำแหน่ง | ref |
| สร้างโดย | System |
| การมองเห็น | ALWAYS |
| ลำดับเมนู | 1 |

<details><summary>View configuration (JSON)</summary>

```json
{"ColumnOrder": null, "AutoSave": false, "AutoReopen": false, "FinishView": "**Automatic**", "RowKey": "", "FormStyle": "Automatic", "PageStyle": "Automatic", "FormFooterStyle": "Bottom", "MaxNestedRows": 5, "AudioInput": false, "Events": [{"EventType": "Form Saved", "EventAction": "**auto**"}], "Icon": "fa-edit", "IconRunnerUps": null, "MenuOrder": 1}
```

</details>

## สรุปงานประจำวัน_Detail

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
{"MainSlideshowImageColumn": "**auto**", "DetailContentColumn": "**none**", "HeaderColumns": [], "QuickEditColumns": [], "ColumnOrder": [], "ImageStyle": "Fit", "Layout": null, "UseCardLayout": false, "DisplayMode": "Automatic", "MaxNestedRows": 5, "SlideshowMode": true, "DesktopSplitMode": "Split view", "UseDesktopMultiColumn": true, "SortBy": [], "PrimarySortColumn": null, "IsPrimarySortDescending": false, "Events": [], "Icon": "fa-indent", "IconRunnerUps": null, "MenuOrder": 1}
```

</details>

## สรุปงานประจำวัน_Form

| คุณสมบัติ | ค่า |
|---|---|
| ชนิด View | form |
| ตำแหน่ง | ref |
| สร้างโดย | System |
| การมองเห็น | ALWAYS |
| ลำดับเมนู | 1 |

<details><summary>View configuration (JSON)</summary>

```json
{"ColumnOrder": null, "AutoSave": false, "AutoReopen": false, "FinishView": "**Automatic**", "RowKey": "", "FormStyle": "Automatic", "PageStyle": "Automatic", "FormFooterStyle": "Bottom", "MaxNestedRows": 5, "AudioInput": false, "Events": [{"EventType": "Form Saved", "EventAction": "**auto**"}], "Icon": "fa-edit", "IconRunnerUps": null, "MenuOrder": 1}
```

</details>

