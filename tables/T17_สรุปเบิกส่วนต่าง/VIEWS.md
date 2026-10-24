# Views ที่เกี่ยวกับตาราง สรุปเบิกส่วนต่าง

รวม **4 views**

## สรุปเบิกส่วนต่าง

| คุณสมบัติ | ค่า |
|---|---|
| ชนิด View | table |
| ตำแหน่ง | menu |
| สร้างโดย | App owner |
| การมองเห็น | ALWAYS |
| ลำดับเมนู | 1 |

<details><summary>View configuration (JSON)</summary>

```json
{"ColumnWidth": "Default", "EnableQuickEdit": false, "ColumnOrder": ["วันที่เริ่มต้น", "วันที่สิ้นสุด", "Export to Excel", "ID_สรุปเบิกส่วนต่าง", "ID_Optimization", "ID_เบิกส่วนต่างSCGวังน้อย", "_ComputedKey_ID_SCGนครหลวงJWDภูมิภาค"], "GroupBy": [], "GroupAggregate": "NONE", "SortBy": [{"Column": "_RowNumber", "Order": "Descending"}], "PrimarySortColumn": null, "IsPrimarySortDescending": false, "Events": [{"EventType": "RowSelected", "EventAction": "**auto**"}], "Icon": "fa-list-ul", "IconRunnerUps": null, "MenuOrder": 1}
```

</details>

## สรุปเบิกส่วนต่าง_Detail

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
{"MainSlideshowImageColumn": "**auto**", "DetailContentColumn": "**none**", "HeaderColumns": [], "QuickEditColumns": ["วันที่เริ่มต้น", "วันที่สิ้นสุด", "วันที่ออกเอกสาร", "Export to Excel"], "ColumnOrder": ["วันที่เริ่มต้น", "วันที่สิ้นสุด", "วันที่ออกเอกสาร", "Export to Excel", "สรุป_ทำเบิกส่วนต่างScgวังน้อย", "ราคารวม_ทำเบิกส่วนต่างScgวังน้อย"], "ImageStyle": "Fit", "Layout": null, "UseCardLayout": false, "DisplayMode": "Automatic", "MaxNestedRows": 5, "SlideshowMode": true, "DesktopSplitMode": "Split view", "UseDesktopMultiColumn": true, "SortBy": [], "PrimarySortColumn": null, "IsPrimarySortDescending": false, "Events": [], "Icon": "fa-indent", "IconRunnerUps": null, "MenuOrder": 1}
```

</details>

## สรุปเบิกส่วนต่าง_Form

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

## สรุปเบิกส่วนต่าง_Inline

| คุณสมบัติ | ค่า |
|---|---|
| ชนิด View | table |
| ตำแหน่ง | ref |
| สร้างโดย | System |
| การมองเห็น | ALWAYS |
| ลำดับเมนู | 1 |

<details><summary>View configuration (JSON)</summary>

```json
{"ColumnWidth": "Default", "EnableQuickEdit": false, "ColumnOrder": [], "GroupBy": [], "GroupAggregate": "NONE", "SortBy": [], "PrimarySortColumn": null, "IsPrimarySortDescending": false, "Events": [{"EventType": "Row Selected", "EventAction": "**auto**"}], "Icon": "fa-table", "IconRunnerUps": null, "MenuOrder": 1}
```

</details>

