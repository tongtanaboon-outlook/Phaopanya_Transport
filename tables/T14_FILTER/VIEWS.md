# Views ที่เกี่ยวกับตาราง FILTER

รวม **3 views**

## FILTER

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
{"MainSlideshowImageColumn": "**auto**", "DetailContentColumn": "**none**", "HeaderColumns": [], "QuickEditColumns": ["STARTDATE", "ENDDATE", "EXPORT TO PDF", "วันที่ออก เอกสาร", "EXPORT TO Excel(สรุปจำนวนจุดส่งงาน)"], "ColumnOrder": ["STARTDATE", "ENDDATE", "ได้เพิ่ม200_ไม่มีสินค้าคืน_ร้านปิด_ไม่มีในจุดส่ง", "ราคา_ได้เพิ่ม200_ไม่มีสินค้าคืน_ร้านปิด_ไม่มีในจุดส่ง", "ทำเบิกค่ายกขึ้นชั้น", "ราคา_ทำเบิกค่ายกขึ้นชั้น", "ได้เพิ่ม50%ของค่าเที่ยว", "ราคา_ได้เพิ่ม50%ของค่าเที่ยว", "วันที่ออกเอกสาร", "EXPORT TO PDF", "สรุปจำนวนจุดส่งงาน", "EXPORT TO Excel(สรุปจำนวนจุดส่งงาน)"], "ImageStyle": "Fill", "Layout": null, "UseCardLayout": false, "DisplayMode": "Automatic", "MaxNestedRows": 5, "SlideshowMode": true, "DesktopSplitMode": "Split view", "UseDesktopMultiColumn": true, "SortBy": [], "PrimarySortColumn": null, "IsPrimarySortDescending": false, "Events": [], "Icon": "fa-list-ul", "IconRunnerUps": null, "MenuOrder": 1}
```

</details>

## FILTER_Detail

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
{"MainSlideshowImageColumn": "**auto**", "DetailContentColumn": "**none**", "HeaderColumns": [], "QuickEditColumns": ["STARTDATE", "ENDDATE", "วันที่ออกเอกสาร", "EXPORT TO PDF", "EXPORT TO Excel(สรุปจำนวนจุดส่งงาน)"], "ColumnOrder": ["STARTDATE", "ENDDATE", "ได้เพิ่ม200_ไม่มีสินค้าคืน_ร้านปิด_ไม่มีในจุดส่ง", "ราคา_ได้เพิ่ม200_ไม่มีสินค้าคืน_ร้านปิด_ไม่มีในจุดส่ง", "ทำเบิกค่ายกขึ้นชั้น", "ราคา_ทำเบิกค่ายกขึ้นชั้น", "ได้เพิ่ม50%ของค่าเที่ยว", "ราคา_ได้เพิ่ม50%ของค่าเที่ยว", "วันที่ออกเอกสาร", "EXPORT TO PDF", "สรุปจำนวนจุดส่งงาน", "EXPORT TO Excel(สรุปจำนวนจุดส่งงาน)"], "ImageStyle": "Fit", "Layout": null, "UseCardLayout": false, "DisplayMode": "Automatic", "MaxNestedRows": 5, "SlideshowMode": true, "DesktopSplitMode": "Split view", "UseDesktopMultiColumn": true, "SortBy": [], "PrimarySortColumn": null, "IsPrimarySortDescending": false, "Events": [], "Icon": "fa-indent", "IconRunnerUps": null, "MenuOrder": 1}
```

</details>

## FILTER_Form

| คุณสมบัติ | ค่า |
|---|---|
| ชนิด View | form |
| ตำแหน่ง | ref |
| สร้างโดย | System |
| การมองเห็น | ALWAYS |
| ลำดับเมนู | 1 |

<details><summary>View configuration (JSON)</summary>

```json
{"ColumnOrder": ["STARTDATE", "ENDDATE", "EXPORT TO .", "New Virtual Column"], "AutoSave": false, "AutoReopen": false, "FinishView": "**Automatic**", "RowKey": "", "FormStyle": "Automatic", "PageStyle": "Automatic", "FormFooterStyle": "Bottom", "MaxNestedRows": 5, "AudioInput": false, "Events": [{"EventType": "Form Saved", "EventAction": "**auto**"}], "Icon": "fa-edit", "IconRunnerUps": null, "MenuOrder": 1}
```

</details>

