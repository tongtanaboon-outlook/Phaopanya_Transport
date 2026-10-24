# Views ที่เกี่ยวกับตาราง Image_Doc_Return

รวม **3 views**

## Image_Doc_Return_Detail

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
{"MainSlideshowImageColumn": "**auto**", "DetailContentColumn": "**none**", "HeaderColumns": [], "QuickEditColumns": [], "ColumnOrder": ["Image_Document_Return", "ID_Image_Doc_Return", "ID_Doc_Return"], "ImageStyle": "Fit", "Layout": null, "UseCardLayout": false, "DisplayMode": "Automatic", "MaxNestedRows": 5, "SlideshowMode": true, "DesktopSplitMode": "Split view", "UseDesktopMultiColumn": true, "SortBy": [], "PrimarySortColumn": null, "IsPrimarySortDescending": false, "Events": [], "Icon": "fa-indent", "IconRunnerUps": null, "MenuOrder": 1}
```

</details>

## Image_Doc_Return_Form

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

## Image_Doc_Return_Inline

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
{"MainDeckImageColumn": "**auto**", "ImageShape": "Square Image", "PrimaryDeckHeaderColumn": "ID_Doc_Return", "SecondaryDeckHeaderColumn": "**auto**", "DeckSummaryColumn": "**auto**", "DeckNestedTableColumn": null, "ShowActionBar": true, "ActionColumns": [], "ActionBarEntries": [], "GroupBy": [], "GroupAggregate": "NONE", "SortBy": [{"Column": "_RowNumber", "Order": "Ascending"}], "PrimarySortColumn": null, "IsPrimarySortDescending": false, "Events": [{"EventType": "Row Selected", "EventAction": "**auto**"}, {"EventType": "Row Swiped Left", "EventAction": "**auto**"}, {"EventType": "Row Swiped Right", "EventAction": "**auto**"}], "Icon": "fa-list-ul", "IconRunnerUps": null, "MenuOrder": 1}
```

</details>

