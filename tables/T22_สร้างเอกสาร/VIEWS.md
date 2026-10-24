# Views ที่เกี่ยวกับตาราง สร้างเอกสาร

รวม **3 views**

## สร้างเอกสาร

| คุณสมบัติ | ค่า |
|---|---|
| ชนิด View | table |
| ตำแหน่ง | menu |
| สร้างโดย | App owner |
| การมองเห็น | ALWAYS |
| ลำดับเมนู | 1 |

<details><summary>View configuration (JSON)</summary>

```json
{"ColumnWidth": "Default", "EnableQuickEdit": false, "ColumnOrder": [], "GroupBy": [], "GroupAggregate": "NONE", "SortBy": [], "PrimarySortColumn": null, "IsPrimarySortDescending": false, "Events": [{"EventType": "Row Selected", "EventAction": "**auto**"}], "Icon": "fa-list-ul", "IconRunnerUps": null, "MenuOrder": 1}
```

</details>

## สร้างเอกสาร_Detail

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
{"MainSlideshowImageColumn": "**auto**", "DetailContentColumn": "**none**", "HeaderColumns": [], "QuickEditColumns": ["ชื่องาน", "ชื่อ -นามสกุล", "StartDate", "EndDate", "Export to xlsx", "Export to xlsx To Athens", "ปริ๊นใบวางบิลแยกตามชื่องาน", "วันที่ออกเอกสาร", "Export to XLSX_12", "EXPORT TO PDFรับคืน"], "ColumnOrder": ["StartDate", "EndDate", "ชื่องาน", "ชื่อ - นามสกุล", "Export to xlsx", "Export to xlsx To Athens", "ปริ๊นใบวางบิลแยกตามชื่องาน", "วันที่ออกเอกสาร", "Export to XLSX_12", "ปริ๊นใบวางบิล", "ราคารวม", "ปริ๊นใบป่ะหน้า", "ราคารวมคนขับ", "ปริ๊นทำเบิกส่วนต่างScgวังน้อย", "ราคารวม_ทำเบิกส่วนต่างScgวังน้อย", "สรุปจำนวนจุดส่งงาน", "EXPORT TO PDFรับคืน", "ได้เพิ่ม200_ไม่มีสินค้าคืน_ร้านปิด_ไม่มีในจุดส่ง", "ราคา_ได้เพิ่ม200_ไม่มีสินค้าคืน_ร้านปิด_ไม่มีในจุดส่ง", "ทำเบิกค่ายกขึ้นชั้น", "ราคา_ทำเบิกค่ายกขึ้นชั้น", "ได้เพิ่ม50%ของค่าเที่ยว", "ราคา_ได้เพิ่ม50%ของค่าเที่ยว"], "ImageStyle": "Fit", "Layout": null, "UseCardLayout": false, "DisplayMode": "Automatic", "MaxNestedRows": 5, "SlideshowMode": true, "DesktopSplitMode": "Split view", "UseDesktopMultiColumn": true, "SortBy": [], "PrimarySortColumn": null, "IsPrimarySortDescending": false, "Events": [], "Icon": "fa-indent", "IconRunnerUps": null, "MenuOrder": 1}
```

</details>

## สร้างเอกสาร_Form

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

