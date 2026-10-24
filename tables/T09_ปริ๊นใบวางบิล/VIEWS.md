# Views ที่เกี่ยวกับตาราง ปริ๊นใบวางบิล

รวม **2 views**

## สร้างรายงาน

| คุณสมบัติ | ค่า |
|---|---|
| ชนิด View | detail |
| ตำแหน่ง | menu |
| ActionType | Automatic |
| สร้างโดย | App owner |
| การมองเห็น | ALWAYS |
| ลำดับเมนู | 1 |
| แสดงเมื่อ | =USERROLE() = "ADMIN" |

<details><summary>View configuration (JSON)</summary>

```json
{"MainSlideshowImageColumn": "**auto**", "DetailContentColumn": "**none**", "HeaderColumns": [], "QuickEditColumns": ["ชื่อ งาน", "StartDate", "EndDate", "Export to xlsx", "Export to xlsx To Athens", "ปริ๊นใบวางบิลแยกตามชื่องาน", "วันที่ออก เอกสาร"], "ColumnOrder": ["ชื่องาน", "StartDate", "EndDate", "ปริ๊นใบวางบิลแยกตามชื่องาน", "วันที่ออกเอกสาร", "Export to xlsx", "Export to xlsx To Athens", "ผลลัพท์", "ราคารวม"], "ImageStyle": "Fill", "Layout": null, "UseCardLayout": false, "DisplayMode": "Automatic", "MaxNestedRows": 5, "SlideshowMode": true, "DesktopSplitMode": "Split view", "UseDesktopMultiColumn": true, "SortBy": [], "PrimarySortColumn": null, "IsPrimarySortDescending": false, "Events": [], "Icon": "fa-list-ul", "IconRunnerUps": null, "MenuOrder": 1}
```

</details>

## PDFชื่องาน_Detail

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
{"MainSlideshowImageColumn": "**auto**", "DetailContentColumn": "**none**", "HeaderColumns": [], "QuickEditColumns": ["ชื่อ งาน", "StartDate", "EndDate", "Export to xlsx", "Export to xlsx To Athens", "ปริ๊นใบวางบิลแยกตามชื่องาน", "วันที่ออก เอกสาร"], "ColumnOrder": ["ชื่องาน", "StartDate", "EndDate", "วันที่ออกเอกสาร", "ปริ๊นใบวางบิลแยกตามชื่องาน", "ผลลัพท์", "Export to xlsx", "Export to xlsx To Athens", "ราคารวม"], "ImageStyle": "Fill", "Layout": null, "UseCardLayout": false, "DisplayMode": "Automatic", "MaxNestedRows": 5, "SlideshowMode": true, "DesktopSplitMode": "Split view", "UseDesktopMultiColumn": true, "SortBy": [], "PrimarySortColumn": null, "IsPrimarySortDescending": false, "Events": [], "Icon": "fa-indent", "IconRunnerUps": null, "MenuOrder": 1}
```

</details>

