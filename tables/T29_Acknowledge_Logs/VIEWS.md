# Views ที่เกี่ยวกับตาราง Acknowledge_Logs

รวม **5 views**

## ฟอร์มรับทราบประกาศ

| คุณสมบัติ | ค่า |
|---|---|
| ชนิด View | form |
| ตำแหน่ง | right |
| สร้างโดย | App owner |
| การมองเห็น | ALWAYS |
| ลำดับเมนู | 1 |
| แสดงเมื่อ | =COUNT( SELECT( Announcements[ID_ประกาศ], NOT(IN([ID_ประกาศ], SELECT(Acknowledge_Logs[ID_ประกาศ], [Email พนักงาน] = USEREMAIL()))) ) ) > 0 |

<details><summary>View configuration (JSON)</summary>

```json
{"ColumnOrder": ["ข้อความประกาศ", "หมายเหตุ", "เลือกเพื่อยืนยัน", "ลงชื่อพนักงาน", "วันที่และเวลารับทราบ", "ชื่อ - นามสกุล", "ทะเบียนรถ", "Email พนักงาน"], "AutoSave": false, "AutoReopen": false, "FinishView": "**Automatic**", "RowKey": "", "FormStyle": "Automatic", "PageStyle": "Automatic", "FormFooterStyle": "Bottom", "MaxNestedRows": 5, "AudioInput": false, "Events": [{"EventType": "Form Saved", "EventAction": "**auto**"}], "Icon": "fas fa-home-heart", "IconRunnerUps": null, "MenuOrder": 1}
```

</details>

## Acknowledge_Logs_Table

| คุณสมบัติ | ค่า |
|---|---|
| ชนิด View | table |
| ตำแหน่ง | menu |
| สร้างโดย | App owner |
| การมองเห็น | ALWAYS |
| ลำดับเมนู | 1 |

<details><summary>View configuration (JSON)</summary>

```json
{"ColumnWidth": "Default", "EnableQuickEdit": true, "ColumnOrder": [], "GroupBy": [{"Column": "ชื่อ - นามสกุล", "Order": "Ascending"}, {"Column": "_RowNumber", "Order": "Ascending"}], "GroupAggregate": "COUNT", "SortBy": [{"Column": "_RowNumber", "Order": "Ascending"}], "PrimarySortColumn": null, "IsPrimarySortDescending": false, "Events": [{"EventType": "Row Selected", "EventAction": "**auto**"}], "Icon": "fa-list-ul", "IconRunnerUps": null, "MenuOrder": 1}
```

</details>

## Acknowledge_Logs_Detail

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
{"MainSlideshowImageColumn": "**auto**", "DetailContentColumn": "**none**", "HeaderColumns": ["ข้อความประกาศ"], "QuickEditColumns": [], "ColumnOrder": ["วันที่และเวลารับทราบ", "หมายเหตุ", "เลือกเพื่อยืนยัน", "ลงชื่อพนักงาน", "ชื่อ - นามสกุล", "ทะเบียนรถ", "Email พนักงาน"], "ImageStyle": "Fit", "Layout": null, "UseCardLayout": false, "DisplayMode": "Automatic", "MaxNestedRows": 5, "SlideshowMode": true, "DesktopSplitMode": "Split view", "UseDesktopMultiColumn": true, "SortBy": [], "PrimarySortColumn": null, "IsPrimarySortDescending": false, "Events": [], "Icon": "fa-indent", "IconRunnerUps": null, "MenuOrder": 1}
```

</details>

## Acknowledge_Logs_Form

| คุณสมบัติ | ค่า |
|---|---|
| ชนิด View | form |
| ตำแหน่ง | ref |
| สร้างโดย | System |
| การมองเห็น | ALWAYS |
| ลำดับเมนู | 1 |

<details><summary>View configuration (JSON)</summary>

```json
{"ColumnOrder": ["ข้อความประกาศ", "หมายเหตุ", "วันที่และเวลารับทราบ", "เลือกเพื่อยืนยัน", "ลงชื่อพนักงาน", "ชื่อ - นามสกุล", "ทะเบียนรถ"], "AutoSave": false, "AutoReopen": false, "FinishView": "**Automatic**", "RowKey": "", "FormStyle": "Automatic", "PageStyle": "Automatic", "FormFooterStyle": "Bottom", "MaxNestedRows": 5, "AudioInput": false, "Events": [{"EventType": "Form Saved", "EventAction": "**auto**"}], "Icon": "fa-edit", "IconRunnerUps": null, "MenuOrder": 1}
```

</details>

## Acknowledge_Logs_Inline

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

