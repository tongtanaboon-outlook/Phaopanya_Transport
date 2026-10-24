# Views ที่เกี่ยวกับตาราง ข้อมูลงานRT

รวม **3 views**

## ข้อมูลงานRT

| คุณสมบัติ | ค่า |
|---|---|
| ชนิด View | table |
| ตำแหน่ง | menu |
| สร้างโดย | App owner |
| การมองเห็น | ALWAYS |
| ลำดับเมนู | 1 |

<details><summary>View configuration (JSON)</summary>

```json
{"ColumnWidth": "Default", "EnableQuickEdit": false, "ColumnOrder": [], "GroupBy": [{"Column": "วันที่เข้ารับ", "Order": "Descending"}, {"Column": "Shipment (รับคืน)", "Order": "Descending"}, {"Column": "Shipment (หลัก)", "Order": "Descending"}, {"Column": "_RowNumber", "Order": "Descending"}], "GroupAggregate": "NONE", "SortBy": [{"Column": "_RowNumber", "Order": "Descending"}], "PrimarySortColumn": null, "IsPrimarySortDescending": false, "Events": [{"EventType": "RowSelected", "EventAction": "**auto**"}], "Icon": "fa-list-ul", "IconRunnerUps": null, "MenuOrder": 1}
```

</details>

## ข้อมูลงานRT_Detail

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

## ข้อมูลงานRT_Form

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

