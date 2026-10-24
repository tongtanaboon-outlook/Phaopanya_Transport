# Views ที่เกี่ยวกับตาราง รับงานคืนได้เงิน200

รวม **4 views**

## รับงานคืนได้เงิน200

| คุณสมบัติ | ค่า |
|---|---|
| ชนิด View | table |
| ตำแหน่ง | menu |
| สร้างโดย | App owner |
| การมองเห็น | ALWAYS |
| ลำดับเมนู | 1 |

<details><summary>View configuration (JSON)</summary>

```json
{"ColumnWidth": "Default", "EnableQuickEdit": true, "ColumnOrder": [], "GroupBy": [{"Column": "เดือน", "Order": "Descending"}, {"Column": "สถานะการเข้ารับสินค้า", "Order": "Descending"}, {"Column": "วันที่เข้ารับ", "Order": "Descending"}, {"Column": "_RowNumber", "Order": "Descending"}], "GroupAggregate": "COUNT", "SortBy": [{"Column": "_RowNumber", "Order": "Descending"}], "PrimarySortColumn": null, "IsPrimarySortDescending": false, "Events": [{"EventType": "RowSelected", "EventAction": "**auto**"}], "Icon": "fa-list-ul", "IconRunnerUps": null, "MenuOrder": 1}
```

</details>

## รับงานคืนได้เงิน200_Detail

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
{"MainSlideshowImageColumn": "**auto**", "DetailContentColumn": "**none**", "HeaderColumns": [], "QuickEditColumns": ["สร้างPDFรับ คืน", "สถานะการเข้ารับสินค้า", "หมายเหตุ", "ราคา", "จำนวนสินค้า", "วันที่เข้า รับ", "Shipment (หลัก)", "เลขที่เอกสารรับคืน", "Shipment No", "Invoice No", "รูปสินค้า", "รูปบิลรับคืน", "รูปจุดที่ส่งงาน"], "ColumnOrder": ["สร้างPDFรับคืน", "ID_รับงานคืนได้เงิน200", "สถานะการเข้ารับสินค้า", "วันที่เข้ารับ", "ชื่อ - นามสกุล", "ทะเบียนรถ", "Shipment (หลัก)", "Shipment (รับคืน)", "เลขที่เอกสารรับคืน", "Shipment No", "Invoice No", "จำนวนสินค้า", "ชื่อเจ้าของสินค้า", "รหัสลูกค้า", "ชื่อลูกค้าที่เข้ารับ", "รูปสินค้า", "รูปบิลรับคืน", "รูปจุดที่ส่งงาน", "ราคา", "หมายเหตุ", "Lat / Long", "Email พนักงาน", "ตรวจสอบก่อนบันทึกข้อมูล", "รายชื่อจุดส่งในตารางงานประจำวัน"], "ImageStyle": "Fit", "Layout": null, "UseCardLayout": false, "DisplayMode": "Automatic", "MaxNestedRows": 5, "SlideshowMode": true, "DesktopSplitMode": "Split view", "UseDesktopMultiColumn": true, "SortBy": [{"Column": "วันที่เข้ารับ", "Order": "Descending"}, {"Column": "_RowNumber", "Order": "Descending"}], "PrimarySortColumn": null, "IsPrimarySortDescending": false, "Events": [], "Icon": "fa-indent", "IconRunnerUps": null, "MenuOrder": 1}
```

</details>

## รับงานคืนได้เงิน200_Form

| คุณสมบัติ | ค่า |
|---|---|
| ชนิด View | form |
| ตำแหน่ง | ref |
| สร้างโดย | System |
| การมองเห็น | ALWAYS |
| ลำดับเมนู | 1 |

<details><summary>View configuration (JSON)</summary>

```json
{"ColumnOrder": ["ตรวจสอบก่อนบันทึกข้อมูล", "สถานะการเข้ารับสินค้า", "วันที่เข้ารับ", "ID_พนักงาน", "ชื่อ - นามสกุล", "ทะเบียนรถ", "Shipment (หลัก)", "Shipment (รับคืน)", "เลขที่เอกสารรับคืน", "Shipment No", "Invoice No", "จำนวนสินค้า", "ชื่อเจ้าของสินค้า", "รหัสลูกค้า", "ชื่อลูกค้าที่เข้ารับ", "รูปสินค้า", "รูปบิลรับคืน", "หมายเหตุ", "Lat / Long", "Email พนักงาน"], "AutoSave": false, "AutoReopen": false, "FinishView": "รับงานคืนได้ เงิน200_Detail", "RowKey": "", "FormStyle": "Automatic", "PageStyle": "Automatic", "FormFooterStyle": "Bottom", "MaxNestedRows": 5, "AudioInput": false, "Events": [{"EventType": "Form Saved", "EventAction": "**auto**"}], "Icon": "fa-edit", "IconRunnerUps": null, "MenuOrder": 1}
```

</details>

## รับงานคืนได้เงิน200_Inline

| คุณสมบัติ | ค่า |
|---|---|
| ชนิด View | deck |
| ตำแหน่ง | ref |
| ActionType | Square Image |
| สร้างโดย | System |
| การมองเห็น | ALWAYS |
| ลำดับเมนู | 1 |

<details><summary>View configuration (JSON)</summary>

```json
{"MainDeckImageColumn": null, "ImageShape": "Square Image", "PrimaryDeckHeaderColumn": null, "SecondaryDeckHeaderColumn": null, "DeckSummaryColumn": null, "DeckNestedTableColumn": null, "ShowActionBar": true, "ActionColumns": null, "ActionBarEntries": [], "GroupBy": [], "GroupAggregate": "NONE", "SortBy": [], "PrimarySortColumn": null, "IsPrimarySortDescending": false, "Events": [{"EventType": "Row Selected", "EventAction": "**auto**"}, {"EventType": "Row Swiped Left", "EventAction": "**auto**"}, {"EventType": "Row Swiped Right", "EventAction": "**auto**"}], "Icon": "fa-list-ul", "IconRunnerUps": null, "MenuOrder": 1}
```

</details>

