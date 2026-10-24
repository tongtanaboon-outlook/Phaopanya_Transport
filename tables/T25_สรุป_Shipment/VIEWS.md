# Views ที่เกี่ยวกับตาราง สรุป_Shipment

รวม **3 views**

## 📦 สรุป_Shipment

| คุณสมบัติ | ค่า |
|---|---|
| ชนิด View | deck |
| ตำแหน่ง | menu |
| ActionType | Square Image |
| สร้างโดย | App owner |
| การมองเห็น | ALWAYS |
| ลำดับเมนู | 1 |

<details><summary>View configuration (JSON)</summary>

```json
{"MainDeckImageColumn": "**auto**", "ImageShape": "Square Image", "PrimaryDeckHeaderColumn": "ShipmentKey", "SecondaryDeckHeaderColumn": "สรุป ยอด", "DeckSummaryColumn": "PlanDelivery", "DeckNestedTableColumn": "**none**", "ShowActionBar": true, "ActionColumns": [], "ActionBarEntries": [], "GroupBy": [{"Column": "PlanDelivery", "Order": "Descending"}, {"Column": "_RowNumber", "Order": "Descending"}], "GroupAggregate": "NONE", "SortBy": [], "PrimarySortColumn": null, "IsPrimarySortDescending": false, "Events": [{"EventType": "Row Selected", "EventAction": "**auto**"}, {"EventType": "Row Swiped Left", "EventAction": "**auto**"}, {"EventType": "Row Swiped Right", "EventAction": "**auto**"}], "Icon": "fa-list-ul", "IconRunnerUps": null, "MenuOrder": 1}
```

</details>

## สรุป_Shipment_Detail

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
{"MainSlideshowImageColumn": "**auto**", "DetailContentColumn": "**none**", "HeaderColumns": [], "QuickEditColumns": [], "ColumnOrder": ["PlanDelivery", "ShipmentNo", "TruckLicense", "สรุปยอด", "รายการ_ทั้งหมด"], "ImageStyle": "Fit", "Layout": null, "UseCardLayout": false, "DisplayMode": "Automatic", "MaxNestedRows": 5, "SlideshowMode": true, "DesktopSplitMode": "Split view", "UseDesktopMultiColumn": true, "SortBy": [], "PrimarySortColumn": null, "IsPrimarySortDescending": false, "Events": [], "Icon": "fa-indent", "IconRunnerUps": null, "MenuOrder": 1}
```

</details>

## สรุป_Shipment_Form

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

