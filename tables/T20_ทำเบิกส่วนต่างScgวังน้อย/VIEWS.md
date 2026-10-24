# Views ที่เกี่ยวกับตาราง ทำเบิกส่วนต่างScgวังน้อย

รวม **4 views**

## ทำเบิกส่วนต่างScgวังน้อย

| คุณสมบัติ | ค่า |
|---|---|
| ชนิด View | table |
| ตำแหน่ง | menu |
| สร้างโดย | App owner |
| การมองเห็น | ALWAYS |
| ลำดับเมนู | 1 |

<details><summary>View configuration (JSON)</summary>

```json
{"ColumnWidth": "Default", "EnableQuickEdit": true, "ColumnOrder": ["สถานะ", "ขออนุมัติเบิกค่าขนส่งส่วนเพิ่ม", "ราคาหลังส่งสินค้า", "ราคาที่สมควรได้", "ราคาตามระยะทาง", "ราคาจุดเพิ่ม", "จำนวนจุดส่งงานจริง", "จำนวนจุดส่งก่อนเริ่มงาน", "ระยะทาง_GoogleMapAPI_Km", "ระยะทางในระบบก่อนส่งสินค้า", "ราคาในระบบก่อนส่งสินค้า", "ชื่องาน", "Shipment No", "วันที่ส่งสินค้า", "ชื่อ - นามสกุล", "ทะเบียนรถ", "เรท น้ำมันดีเซล", "เดือน"], "GroupBy": [{"Column": "เดือน", "Order": "Descending"}, {"Column": "สถานะ", "Order": "Descending"}, {"Column": "ชื่อ -นามสกุล", "Order": "Descending"}, {"Column": "วันที่ส่ง สินค้า", "Order": "Descending"}, {"Column": "_RowNumber", "Order": "Descending"}], "GroupAggregate": "SUM :: ขออนุมัติเบิกค่าขนส่งส่วนเพิ่ม", "SortBy": [{"Column": "Shipment No", "Order": "Descending"}, {"Column": "_RowNumber", "Order": "Descending"}], "PrimarySortColumn": null, "IsPrimarySortDescending": false, "Events": [{"EventType": "RowSelected", "EventAction": "**auto**"}], "Icon": "fa-list-ul", "IconRunnerUps": null, "MenuOrder": 1}
```

</details>

## ทำเบิกส่วนต่างScgวังน้อย_Detail

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
{"MainSlideshowImageColumn": "**auto**", "DetailContentColumn": "**none**", "HeaderColumns": [], "QuickEditColumns": ["สร้างPDFเบิกส่วน ต่าง", "Email พนักงาน", "สร้างPDFเบิกตามระยะทาง"], "ColumnOrder": ["QR code เส้นทางรวม", "สร้างPDFเบิกตามระยะทาง", "สร้างPDFเบิกส่วนต่าง", "GoogleMapsRoutesAPI", "แสดงแผนที่_GoogleMapsRoutesAPI", "วันที่ส่งสินค้า", "ชื่อ - นามสกุล", "ทะเบียนรถ", "Shipment No", "ราคาในระบบก่อนส่งสินค้า", "ระยะทางในระบบก่อนส่งสินค้า", "สถานะ", "ชื่องาน", "ระยะทาง_GoogleMapAPI_Km", "ราคาตามระยะทาง", "จำนวนจุดส่งงานจริง", "ราคาจุดเพิ่ม", "ราคาที่สมควรได้", "ราคาหลังส่งสินค้า", "ขออนุมัติเบิกค่าขนส่งส่วนเพิ่ม", "จำนวนจุดส่งก่อนเริ่มงาน", "ต้นทาง", "Lat/Long_ปลายทาง_01", "01เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No", "รูปบิลส่งสินค้า_01", "รูปหน้าร้าน_บ้าน01", "รูปส่งสินค้า01", "Lat/Long_ปลายทาง_02", "02เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No", "รูปบิลส่งสินค้า_02", "รูปหน้าร้าน_บ้าน02", "รูปส่งสินค้า02", "Lat/Long_ปลายทาง_03", "03เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No", "รูปบิลส่งสินค้า_03", "รูปหน้าร้าน_บ้าน03", "รูปส่งสินค้า03", "Lat/Long_ปลายทาง_04", "04เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No", "รูปบิลส่งสินค้า_04", "รูปหน้าร้าน_บ้าน04", "รูปส่งสินค้า04", "Lat/Long_ปลายทาง_05", "05เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No", "รูปบิลส่งสินค้า_05", "รูปหน้าร้าน_บ้าน05", "รูปส่งสินค้า05", "Lat/Long_ปลายทาง_06", "06เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No", "รูปบิลส่งสินค้า_06", "รูปหน้าร้าน_บ้าน06", "รูปส่งสินค้า06", "Lat/Long_ปลายทาง_07", "07เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No", "รูปบิลส่งสินค้า_07", "รูปหน้าร้าน_บ้าน07", "รูปส่งสินค้า07", "Lat/Long_ปลายทาง_08", "08เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No", "รูปบิลส่งสินค้า_08", "รูปหน้าร้าน_บ้าน08", "รูปส่งสินค้า08", "Lat/Long_ปลายทาง_09", "09เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No", "รูปบิลส่งสินค้า_09", "รูปหน้าร้าน_บ้าน09", "รูปส่งสินค้า09", "Lat/Long_ปลายทาง_10", "10เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No", "รูปบิลส่งสินค้า_10", "รูปหน้าร้าน_บ้าน10", "รูปส่งสินค้า10", "Lat/Long_ปลายทาง_11", "11เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No", "รูปบิลส่งสินค้า_11", "รูปหน้าร้าน_บ้าน11", "รูปส่งสินค้า11", "Lat/Long_ปลายทาง_12", "12เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No", "รูปบิลส่งสินค้า_12", "รูปหน้าร้าน_บ้าน12", "รูปส่งสินค้า12", "Lat/Long_ปลายทาง_13", "13เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No", "รูปบิลส่งสินค้า_13", "รูปหน้าร้าน_บ้าน13", "รูปส่งสินค้า13", "Lat/Long_ปลายทาง_14", "14เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No", "รูปบิลส่งสินค้า_14", "รูปหน้าร้าน_บ้าน14", "รูปส่งสินค้า14", "Lat/Long_ปลายทาง_15", "15เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No", "รูปบิลส่งสินค้า_15", "รูปหน้าร้าน_บ้าน15", "รูปส่งสินค้า15", "Lat/Long_ปลายทาง_16", "16เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No", "รูปบิลส่งสินค้า_16", "รูปหน้าร้าน_บ้าน16", "รูปส่งสินค้า16", "Lat/Long_ปลายทาง_17", "17เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No", "รูปบิลส่งสินค้า_17", "รูปหน้าร้าน_บ้าน17", "รูปส่งสินค้า17", "Lat/Long_ปลายทาง_18", "18เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No", "รูปบิลส่งสินค้า_18", "รูปหน้าร้าน_บ้าน18", "รูปส่งสินค้า18", "Lat/Long_ปลายทาง_19", "19เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No", "รูปบิลส่งสินค้า_19", "รูปหน้าร้าน_บ้าน19", "รูปส่งสินค้า19", "Lat/Long_ปลายทาง_20", "20เจ้าของสินค้า // ชื่อปลายทาง // Lat_Long // Inv No", "รูปบิลส่งสินค้า_20", "รูปหน้าร้าน_บ้าน20", "รูปส่งสินค้า20", "จุดส่งงานลำดับสุดท้าย", "ชื่อปลายทาง_INV_จุดสุดท้าย", "เรท น้ำมันดีเซล", "เดือน", "Email พนักงาน", "ตรวจสอบข้อมูล", "Candidate_2_ระยะทาง_Km", "Candidate_2_แสดงแผนที่", "Candidate_3_ระยะทาง_Km", "Candidate_3_แสดงแผนที่"], "ImageStyle": "Fit", "Layout": null, "UseCardLayout": false, "DisplayMode": "Automatic", "MaxNestedRows": 5, "SlideshowMode": true, "DesktopSplitMode": "Split view", "UseDesktopMultiColumn": true, "SortBy": [{"Column": "_RowNumber", "Order": "Descending"}], "PrimarySortColumn": null, "IsPrimarySortDescending": false, "Events": [], "Icon": "fa-indent", "IconRunnerUps": null, "MenuOrder": 1}
```

</details>

## ทำเบิกส่วนต่างScgวังน้อย_Form

| คุณสมบัติ | ค่า |
|---|---|
| ชนิด View | form |
| ตำแหน่ง | ref |
| สร้างโดย | System |
| การมองเห็น | ALWAYS |
| ลำดับเมนู | 1 |

<details><summary>View configuration (JSON)</summary>

```json
{"ColumnOrder": ["ต้นทาง", "สถานะ", "วันที่ส่งสินค้า", "ชื่อ - นามสกุล", "ทะเบียนรถ", "Shipment No", "ชื่องาน", "จำนวนจุดส่งงานจริง", "จำนวนจุดส่งก่อนเริ่มงาน", "ราคาในระบบก่อนส่งสินค้า", "ระยะทางในระบบก่อนส่งสินค้า", "ราคาสมควรได้", "เรท น้ำมันดีเซล", "Email พนักงาน", "ตรวจสอบข้อมูล"], "AutoSave": false, "AutoReopen": false, "FinishView": "ทำเบิกส่วนต่างScgวังน้อย_Detail", "RowKey": "", "FormStyle": "Automatic", "PageStyle": "Automatic", "FormFooterStyle": "Bottom", "MaxNestedRows": 5, "AudioInput": false, "Events": [{"EventType": "Form Saved", "EventAction": "**auto**"}], "Icon": "fa-edit", "IconRunnerUps": null, "MenuOrder": 1}
```

</details>

## ทำเบิกส่วนต่างScgวังน้อย_Inline

| คุณสมบัติ | ค่า |
|---|---|
| ชนิด View | table |
| ตำแหน่ง | ref |
| สร้างโดย | System |
| การมองเห็น | ALWAYS |
| ลำดับเมนู | 1 |

<details><summary>View configuration (JSON)</summary>

```json
{"ColumnWidth": "Default", "EnableQuickEdit": true, "ColumnOrder": [], "GroupBy": [{"Column": "เดือน", "Order": "Descending"}, {"Column": "วันที่ส่งสินค้า", "Order": "Descending"}, {"Column": "ชื่อ -นามสกุล", "Order": "Descending"}, {"Column": "สถานะ", "Order": "Descending"}, {"Column": "_RowNumber", "Order": "Descending"}], "GroupAggregate": "COUNT", "SortBy": [{"Column": "_RowNumber", "Order": "Descending"}], "PrimarySortColumn": null, "IsPrimarySortDescending": false, "Events": [{"EventType": "RowSelected", "EventAction": "**auto**"}], "Icon": "fa-table", "IconRunnerUps": null, "MenuOrder": 1}
```

</details>

