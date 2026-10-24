# Views ที่เกี่ยวกับตาราง ข้อมูลการเข้าบำรุงรักษา

รวม **4 views**

## ข้อมูลการเข้าบำรุงรักษา

| คุณสมบัติ | ค่า |
|---|---|
| ชนิด View | table |
| ตำแหน่ง | menu |
| สร้างโดย | App owner |
| การมองเห็น | ALWAYS |
| ลำดับเมนู | 1 |

<details><summary>View configuration (JSON)</summary>

```json
{"ColumnWidth": "Default", "EnableQuickEdit": true, "ColumnOrder": ["ID_การเข้าบำรุงรักษา", "Email พนักงาน", "วันที่เข้าบำรุงรักษา", "ชื่อ - นามสกุล", "ทะเบียนรถ", "รูปถ่ายเลขไมล์รถยนต์ก่อนเข้าบำรุงรักษา", "รูปถ่ายบิลหรือใบเสร็จ รายการเข้าบำรุงรักษา", "ราคา", "เดือน"], "GroupBy": [{"Column": "เดือน", "Order": "Descending"}, {"Column": "วันที่เข้าบำรุง รักษา", "Order": "Descending"}, {"Column": "_RowNumber", "Order": "Descending"}], "GroupAggregate": "SUM :: ราคา", "SortBy": [{"Column": "_RowNumber", "Order": "Descending"}], "PrimarySortColumn": null, "IsPrimarySortDescending": false, "Events": [{"EventType": "RowSelected", "EventAction": "**auto**"}], "Icon": "fa-list-ul", "IconRunnerUps": null, "MenuOrder": 1}
```

</details>

## ข้อมูลการเข้าบำรุงรักษา_Detail

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
{"MainSlideshowImageColumn": "**auto**", "DetailContentColumn": "**none**", "HeaderColumns": [], "QuickEditColumns": ["ID_พนักงาน", "ราคา"], "ColumnOrder": [], "ImageStyle": "Fill", "Layout": null, "UseCardLayout": false, "DisplayMode": "Automatic", "MaxNestedRows": 5, "SlideshowMode": true, "DesktopSplitMode": "Split view", "UseDesktopMultiColumn": true, "SortBy": [{"Column": "_RowNumber", "Order": "Descending"}], "PrimarySortColumn": null, "IsPrimarySortDescending": false, "Events": [], "Icon": "fa-indent", "IconRunnerUps": null, "MenuOrder": 1}
```

</details>

## ข้อมูลการเข้าบำรุงรักษา_Form

| คุณสมบัติ | ค่า |
|---|---|
| ชนิด View | form |
| ตำแหน่ง | ref |
| สร้างโดย | System |
| การมองเห็น | ALWAYS |
| ลำดับเมนู | 1 |

<details><summary>View configuration (JSON)</summary>

```json
{"ColumnOrder": ["วันที่เข้าบำรุงรักษา", "ID_พนักงาน", "ชื่อ - นามสกุล", "ทะเบียนรถ", "รูปถ่ายเลขไมล์รถยนต์ก่อนเข้าบำรุงรักษา", "กรุณาพิม เลขไมล์รถยนต์ก่อนเข้าบำรุงรักษา", "รูปถ่ายบิลหรือใบเสร็จ รายการเข้าบำรุงรักษา", "กรุณาพิม รายการเข้าบำรุงรักษา", "ราคา", "กรุณาพิม เลข ไมล์รถยนต์ รอบบำรุงรักษาครั้งถัดไป", "Email พนักงาน"], "AutoSave": false, "AutoReopen": false, "FinishView": "หน้า หลัก", "RowKey": "", "FormStyle": "Automatic", "PageStyle": "Automatic", "FormFooterStyle": "Bottom", "MaxNestedRows": 5, "AudioInput": false, "Events": [{"EventType": "Form Saved", "EventAction": "**auto**"}], "Icon": "fa-edit", "IconRunnerUps": null, "MenuOrder": 1}
```

</details>

## ข้อมูลการเข้าบำรุงรักษา_Inline

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

