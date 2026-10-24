# Views ทั้งหมด (หน้าจอของแอป)

รวม **115 views** — จัดกลุ่มตามตารางที่ view ผูกอยู่ เนื่องจาก AppSheet ผูก view เข้ากับตาราง/slice ด้วยชื่อ การ map บางส่วนจึงเป็นการ "อนุมาน" (ระบุไว้ให้ทุกกรณี) และมีหมวดสุดท้ายสำหรับ view ระดับแอปที่ไม่ผูกกับตารางใดตารางเดียว

## สรุปจำนวนตามชนิด View

| ชนิด View | จำนวน |
|---|---:|
| `detail` | 38 |
| `form` | 36 |
| `table` | 32 |
| `deck` | 8 |
| `gallery` | 1 |

## [SCGนครหลวงJWDภูมิภาค](../tables/T01_SCGนครหลวงJWDภูมิภาค/) — 4 views

| View | ชนิด | ตำแหน่ง | วิธี map |
|---|---|---|---|
| **SCGนครหลวงJWDภูมิภาค** | `table` | menu |  |
| **SCGนครหลวงJWDภูมิภาค_Detail** | `detail` | ref |  |
| **SCGนครหลวงJWDภูมิภาค_Form** | `form` | ref |  |
| **SCGนครหลวงJWDภูมิภาค_Inline** | `table` | ref |  |

- *SCGนครหลวงJWDภูมิภาค*: Events: `Row Selected`
- *SCGนครหลวงJWDภูมิภาค_Form*: Events: `Form Saved`
- *SCGนครหลวงJWDภูมิภาค_Inline*: Events: `Row Selected`

## [ข้อมูลการเข้าบำรุงรักษา](../tables/T03_ข้อมูลการเข้าบำรุงรักษา/) — 4 views

| View | ชนิด | ตำแหน่ง | วิธี map |
|---|---|---|---|
| **ข้อมูลการเข้าบำรุงรักษา** | `table` | menu |  |
| **ข้อมูลการเข้าบำรุงรักษา_Detail** | `detail` | ref |  |
| **ข้อมูลการเข้าบำรุงรักษา_Form** | `form` | ref |  |
| **ข้อมูลการเข้าบำรุงรักษา_Inline** | `deck` | ref |  |

- *ข้อมูลการเข้าบำรุงรักษา*: Events: `RowSelected`
- *ข้อมูลการเข้าบำรุงรักษา_Form*: Events: `Form Saved`
- *ข้อมูลการเข้าบำรุงรักษา_Inline*: Events: `Row Selected`, `Row Swiped Left`, `Row Swiped Right`

## [ข้อมูลการวางบิล](../tables/T04_ข้อมูลการวางบิล/) — 12 views

| View | ชนิด | ตำแหน่ง | วิธี map |
|---|---|---|---|
| **รอการอนุมัติ** | `table` | right most | ผ่าน slice ชื่อเดียวกัน |
| **View ราคาไม่ตรง list** | `table` | menu |  |
| **ข้อมูลการวางบิล** | `table` | menu |  |
| **ค่าใช้จ่าย** | `table` | menu |  |
| **View ราคาไม่ตรง_Detail** | `detail` | ref |  |
| **ข้อมูลการวางของแต่ละคน_Detail** | `detail` | ref |  |
| **ข้อมูลการวางของแต่ละคน_Form** | `form` | ref |  |
| **ข้อมูลการวางบิล_Detail** | `detail` | ref |  |
| **ข้อมูลการวางบิล_Form** | `form` | ref |  |
| **ข้อมูลการวางบิล_Inline** | `deck` | ref |  |
| **รอการอนุมัติ_Detail** | `detail` | ref |  |
| **รอการอนุมัติ_Form** | `form` | ref |  |

- *รอการอนุมัติ*: Show if: `=USERROLE() = "ADMIN"` · Events: `RowSelected`
- *View ราคาไม่ตรง list*: Events: `Row Selected`
- *ข้อมูลการวางบิล*: Show if: `=USERROLE() = ADMIN` · Events: `RowSelected`
- *ค่าใช้จ่าย*: Events: `Row Selected`
- *ข้อมูลการวางของแต่ละคน_Form*: Events: `Form Saved`
- *ข้อมูลการวางบิล_Form*: Events: `Form Saved`
- *ข้อมูลการวางบิล_Inline*: Events: `Row Selected`, `Row Swiped Left`, `Row Swiped Right`
- *รอการอนุมัติ_Form*: Events: `Form Saved`

## [ตารางงานประจำวัน](../tables/T05_ตารางงานประจำวัน/) — 10 views

| View | ชนิด | ตำแหน่ง | วิธี map |
|---|---|---|---|
| **ตารางงานประจำวัน** | `table` | menu |  |
| **สรุปจำนวนจุดส่งสินค้า** | `table` | menu |  |
| **Slice_Monitor_Today_Detail** | `detail` | ref |  |
| **Slice_Monitor_Today_Form** | `form` | ref |  |
| **ค้างสแกนวันนี้และเมื่อวาน_Detail** | `detail` | ref |  |
| **ค้างสแกนวันนี้และเมื่อวาน_Form** | `form` | ref |  |
| **ตารางงานประจำวัน_Detail** | `detail` | ref |  |
| **ตารางงานประจำวัน_Form** | `form` | ref |  |
| **สรุปงานประจำวัน_Detail** | `detail` | ref |  |
| **สรุปงานประจำวัน_Form** | `form` | ref |  |

- *ตารางงานประจำวัน*: Events: `RowSelected`
- *สรุปจำนวนจุดส่งสินค้า*: Events: `RowSelected`
- *Slice_Monitor_Today_Form*: Events: `Form Saved`
- *ค้างสแกนวันนี้และเมื่อวาน_Form*: Events: `Form Saved`
- *ตารางงานประจำวัน_Form*: Events: `Form Saved`
- *สรุปงานประจำวัน_Form*: Events: `Form Saved`

## [ราคาน้ำมันดีเซล](../tables/T06_ราคาน้ำมันดีเซล/) — 3 views

| View | ชนิด | ตำแหน่ง | วิธี map |
|---|---|---|---|
| **ราคาน้ำมันดีเซล** | `table` | menu |  |
| **ราคาน้ำมันดีเซล_Detail** | `detail` | ref |  |
| **ราคาน้ำมันดีเซล_Form** | `form` | ref |  |

- *ราคาน้ำมันดีเซล*: Events: `Row Selected`
- *ราคาน้ำมันดีเซล_Form*: Events: `Form Saved`

## [ราคาในระบบก่อนส่งสินค้า](../tables/T07_ราคาในระบบก่อนส่งสินค้า/) — 3 views

| View | ชนิด | ตำแหน่ง | วิธี map |
|---|---|---|---|
| **ราคาในระบบก่อนส่งสินค้า** | `table` | menu |  |
| **ราคาในระบบก่อนส่งสินค้า_Detail** | `detail` | ref |  |
| **ราคาในระบบก่อนส่งสินค้า_Form** | `form` | ref |  |

- *ราคาในระบบก่อนส่งสินค้า*: Events: `RowSelected`
- *ราคาในระบบก่อนส่งสินค้า_Form*: Events: `Form Saved`

## [หน้าหลัก](../tables/T08_หน้าหลัก/) — 3 views

| View | ชนิด | ตำแหน่ง | วิธี map |
|---|---|---|---|
| **หน้าหลัก** | `gallery` | right |  |
| **หน้าหลัก_Detail** | `detail` | ref |  |
| **หน้าหลัก_Form** | `form` | ref |  |

- *หน้าหลัก*: Events: `Row Selected`
- *หน้าหลัก_Form*: Events: `Form Saved`

## [ปริ๊นใบวางบิล](../tables/T09_ปริ๊นใบวางบิล/) — 2 views

| View | ชนิด | ตำแหน่ง | วิธี map |
|---|---|---|---|
| **สร้างรายงาน** | `detail` | menu |  |
| **PDFชื่องาน_Detail** | `detail` | ref |  |

- *สร้างรายงาน*: Show if: `=USERROLE() = "ADMIN"`

## [PDFพนักงาน](../tables/T10_PDFพนักงาน/) — 2 views

| View | ชนิด | ตำแหน่ง | วิธี map |
|---|---|---|---|
| **PDFพนักงาน_Detail** | `detail` | ref |  |
| **PDFพนักงาน_Form** | `form` | ref |  |

- *PDFพนักงาน_Form*: Events: `Form Saved`

## [แจ้งปัญหาระหว่างวัน](../tables/T11_แจ้งปัญหาระหว่างวัน/) — 4 views

| View | ชนิด | ตำแหน่ง | วิธี map |
|---|---|---|---|
| **แจ้งปัญหา** | `table` | menu |  |
| **แจ้งปัญหาระหว่างวัน_Detail** | `detail` | ref |  |
| **แจ้งปัญหาระหว่างวัน_Form** | `form` | ref |  |
| **แจ้งปัญหาระหว่างวัน_Inline** | `deck` | ref |  |

- *แจ้งปัญหา*: Events: `RowSelected`
- *แจ้งปัญหาระหว่างวัน_Form*: Events: `Form Saved`
- *แจ้งปัญหาระหว่างวัน_Inline*: Events: `Row Selected`, `Row Swiped Left`, `Row Swiped Right`

## [รับงานคืนได้เงิน200](../tables/T12_รับงานคืนได้เงิน200/) — 4 views

| View | ชนิด | ตำแหน่ง | วิธี map |
|---|---|---|---|
| **รับงานคืนได้เงิน200** | `table` | menu |  |
| **รับงานคืนได้เงิน200_Detail** | `detail` | ref |  |
| **รับงานคืนได้เงิน200_Form** | `form` | ref |  |
| **รับงานคืนได้เงิน200_Inline** | `deck` | ref |  |

- *รับงานคืนได้เงิน200*: Events: `RowSelected`
- *รับงานคืนได้เงิน200_Form*: Events: `Form Saved`
- *รับงานคืนได้เงิน200_Inline*: Events: `Row Selected`, `Row Swiped Left`, `Row Swiped Right`

## [ข้อมูลงานRT](../tables/T13_ข้อมูลงานRT/) — 3 views

| View | ชนิด | ตำแหน่ง | วิธี map |
|---|---|---|---|
| **ข้อมูลงานRT** | `table` | menu |  |
| **ข้อมูลงานRT_Detail** | `detail` | ref |  |
| **ข้อมูลงานRT_Form** | `form` | ref |  |

- *ข้อมูลงานRT*: Events: `RowSelected`
- *ข้อมูลงานRT_Form*: Events: `Form Saved`

## [FILTER](../tables/T14_FILTER/) — 3 views

| View | ชนิด | ตำแหน่ง | วิธี map |
|---|---|---|---|
| **FILTER** | `detail` | menu |  |
| **FILTER_Detail** | `detail` | ref |  |
| **FILTER_Form** | `form` | ref |  |

- *FILTER*: Show if: `=USERROLE() = "ADMIN"`
- *FILTER_Form*: Events: `Form Saved`

## [ข้อมูลพนักงาน](../tables/T15_ข้อมูลพนักงาน/) — 3 views

| View | ชนิด | ตำแหน่ง | วิธี map |
|---|---|---|---|
| **ข้อมูลพนักงาน** | `table` | menu |  |
| **ข้อมูลพนักงาน_Detail** | `detail` | ref |  |
| **ข้อมูลพนักงาน_Form** | `form` | ref |  |

- *ข้อมูลพนักงาน*: Events: `Row Selected`
- *ข้อมูลพนักงาน_Form*: Events: `Form Saved`

## [ข้อมูลชื่องานต้นทางปลายทาง](../tables/T16_ข้อมูลชื่องานต้นทางปลายทาง/) — 3 views

| View | ชนิด | ตำแหน่ง | วิธี map |
|---|---|---|---|
| **ข้อมูลชื่องานต้นทางปลายทาง** | `table` | menu |  |
| **ข้อมูลชื่องานต้นทางปลายทาง_Detail** | `detail` | ref |  |
| **ข้อมูลชื่องานต้นทางปลายทาง_Form** | `form` | ref |  |

- *ข้อมูลชื่องานต้นทางปลายทาง*: Events: `Row Selected`
- *ข้อมูลชื่องานต้นทางปลายทาง_Form*: Events: `Form Saved`

## [สรุปเบิกส่วนต่าง](../tables/T17_สรุปเบิกส่วนต่าง/) — 4 views

| View | ชนิด | ตำแหน่ง | วิธี map |
|---|---|---|---|
| **สรุปเบิกส่วนต่าง** | `table` | menu |  |
| **สรุปเบิกส่วนต่าง_Detail** | `detail` | ref |  |
| **สรุปเบิกส่วนต่าง_Form** | `form` | ref |  |
| **สรุปเบิกส่วนต่าง_Inline** | `table` | ref |  |

- *สรุปเบิกส่วนต่าง*: Events: `RowSelected`
- *สรุปเบิกส่วนต่าง_Form*: Events: `Form Saved`
- *สรุปเบิกส่วนต่าง_Inline*: Events: `Row Selected`

## [Doc_Return](../tables/T18_Doc_Return/) — 2 views

| View | ชนิด | ตำแหน่ง | วิธี map |
|---|---|---|---|
| **Doc_Return_Detail** | `detail` | ref |  |
| **Doc_Return_Form** | `form` | ref |  |

- *Doc_Return_Form*: Events: `Form Saved`

## [Image_Doc_Return](../tables/T19_Image_Doc_Return/) — 3 views

| View | ชนิด | ตำแหน่ง | วิธี map |
|---|---|---|---|
| **Image_Doc_Return_Detail** | `detail` | ref |  |
| **Image_Doc_Return_Form** | `form` | ref |  |
| **Image_Doc_Return_Inline** | `deck` | ref |  |

- *Image_Doc_Return_Form*: Events: `Form Saved`
- *Image_Doc_Return_Inline*: Events: `Row Selected`, `Row Swiped Left`, `Row Swiped Right`

## [ทำเบิกส่วนต่างScgวังน้อย](../tables/T20_ทำเบิกส่วนต่างScgวังน้อย/) — 4 views

| View | ชนิด | ตำแหน่ง | วิธี map |
|---|---|---|---|
| **ทำเบิกส่วนต่างScgวังน้อย** | `table` | menu |  |
| **ทำเบิกส่วนต่างScgวังน้อย_Detail** | `detail` | ref |  |
| **ทำเบิกส่วนต่างScgวังน้อย_Form** | `form` | ref |  |
| **ทำเบิกส่วนต่างScgวังน้อย_Inline** | `table` | ref |  |

- *ทำเบิกส่วนต่างScgวังน้อย*: Events: `RowSelected`
- *ทำเบิกส่วนต่างScgวังน้อย_Form*: Events: `Form Saved`
- *ทำเบิกส่วนต่างScgวังน้อย_Inline*: Events: `RowSelected`

## [ข้อมูลงานRW](../tables/T21_ข้อมูลงานRW/) — 3 views

| View | ชนิด | ตำแหน่ง | วิธี map |
|---|---|---|---|
| **ข้อมูลงานRW** | `table` | menu |  |
| **ข้อมูลงานRW_Detail** | `detail` | ref |  |
| **ข้อมูลงานRW_Form** | `form` | ref |  |

- *ข้อมูลงานRW*: Events: `Row Selected`
- *ข้อมูลงานRW_Form*: Events: `Form Saved`

## [สร้างเอกสาร](../tables/T22_สร้างเอกสาร/) — 3 views

| View | ชนิด | ตำแหน่ง | วิธี map |
|---|---|---|---|
| **สร้างเอกสาร** | `table` | menu |  |
| **สร้างเอกสาร_Detail** | `detail` | ref |  |
| **สร้างเอกสาร_Form** | `form` | ref |  |

- *สร้างเอกสาร*: Events: `Row Selected`
- *สร้างเอกสาร_Form*: Events: `Form Saved`

## [ScanDocs](../tables/T23_ScanDocs/) — 5 views

| View | ชนิด | ตำแหน่ง | วิธี map |
|---|---|---|---|
| **Scan 📋** | `form` | left |  |
| **🧾ที่สแกนรับ ✅** | `table` | menu |  |
| **ScanDocs_Detail** | `detail` | ref |  |
| **ScanDocs_Form** | `form` | ref |  |
| **ScanDocs_Inline** | `table` | ref |  |

- *Scan 📋*: Events: `Form Saved`
- *🧾ที่สแกนรับ ✅*: Events: `RowSelected`
- *ScanDocs_Form*: Events: `Form Saved`
- *ScanDocs_Inline*: Events: `Row Selected`

## [สรุป_เจ้าของสินค้า](../tables/T24_สรุป_เจ้าของสินค้า/) — 2 views

| View | ชนิด | ตำแหน่ง | วิธี map |
|---|---|---|---|
| **สรุป_เจ้าของสินค้า_Detail** | `detail` | ref |  |
| **สรุป_เจ้าของสินค้า_Form** | `form` | ref |  |

- *สรุป_เจ้าของสินค้า_Form*: Events: `Form Saved`

## [สรุป_Shipment](../tables/T25_สรุป_Shipment/) — 3 views

| View | ชนิด | ตำแหน่ง | วิธี map |
|---|---|---|---|
| **📦 สรุป_Shipment** | `deck` | menu |  |
| **สรุป_Shipment_Detail** | `detail` | ref |  |
| **สรุป_Shipment_Form** | `form` | ref |  |

- *📦 สรุป_Shipment*: Events: `Row Selected`, `Row Swiped Left`, `Row Swiped Right`
- *สรุป_Shipment_Form*: Events: `Form Saved`

## [PriceOverride](../tables/T26_PriceOverride/) — 3 views

| View | ชนิด | ตำแหน่ง | วิธี map |
|---|---|---|---|
| **PriceOverride** | `table` | menu |  |
| **PriceOverride_Detail** | `detail` | ref |  |
| **PriceOverride_Form** | `form` | ref |  |

- *PriceOverride*: Events: `Row Selected`
- *PriceOverride_Form*: Events: `Form Saved`

## [Price_Table](../tables/T27_Price_Table/) — 2 views

| View | ชนิด | ตำแหน่ง | วิธี map |
|---|---|---|---|
| **Price_Table_Detail** | `detail` | ref |  |
| **Price_Table_Form** | `form` | ref |  |

- *Price_Table_Form*: Events: `Form Saved`

## [ส่งงานที่ยังไม่มีข้อมูลในระบบ](../tables/T28_ส่งงานที่ยังไม่มีข้อมูลในระบบ/) — 3 views

| View | ชนิด | ตำแหน่ง | วิธี map |
|---|---|---|---|
| **ส่งงานที่ยังไม่มีข้อมูลในระบบ_Detail** | `detail` | ref |  |
| **ส่งงานที่ยังไม่มีข้อมูลในระบบ_Form** | `form` | ref |  |
| **ส่งงานที่ยังไม่มีข้อมูลในระบบ_Inline** | `deck` | ref |  |

- *ส่งงานที่ยังไม่มีข้อมูลในระบบ_Form*: Events: `Form Saved`
- *ส่งงานที่ยังไม่มีข้อมูลในระบบ_Inline*: Events: `Row Selected`, `Row Swiped Left`, `Row Swiped Right`

## [Acknowledge_Logs](../tables/T29_Acknowledge_Logs/) — 5 views

| View | ชนิด | ตำแหน่ง | วิธี map |
|---|---|---|---|
| **ฟอร์มรับทราบประกาศ** | `form` | right |  |
| **Acknowledge_Logs_Table** | `table` | menu |  |
| **Acknowledge_Logs_Detail** | `detail` | ref |  |
| **Acknowledge_Logs_Form** | `form` | ref |  |
| **Acknowledge_Logs_Inline** | `table` | ref |  |

- *ฟอร์มรับทราบประกาศ*: Show if: `=COUNT( SELECT( Announcements[ID_ประกาศ], NOT(IN([ID_ประกาศ], SELECT(Acknowledge_Logs[ID_ประกาศ], [Email พนักงาน] = USEREMAIL()))) ) ) > 0` · Events: `Form Saved`
- *Acknowledge_Logs_Table*: Events: `Row Selected`
- *Acknowledge_Logs_Form*: Events: `Form Saved`
- *Acknowledge_Logs_Inline*: Events: `Row Selected`

## [Announcements](../tables/T30_Announcements/) — 2 views

| View | ชนิด | ตำแหน่ง | วิธี map |
|---|---|---|---|
| **Announcements_Detail** | `detail` | ref |  |
| **Announcements_Form** | `form` | ref |  |

- *Announcements_Form*: Events: `Form Saved`

## View ระดับแอป / ไม่ผูกกับตารางใดโดยตรง

รวม 8 views (เช่น dashboard รวม หรือ view ที่อ้าง slice ที่ไม่ได้อยู่ในเอกสาร)

| View | ชนิด | ตำแหน่ง |
|---|---|---|
| **📦 สรุปรับเอกสาร** | `deck` | menu |
| **Document_Return** | `table` | menu |
| **Image_Document_Return** | `table` | menu |
| **Monitor_Dashboard** | `table` | menu |
| **ข้อมูลการวางบิลแต่ละคน** | `table` | menu |
| **ตารางราคา** | `table` | menu |
| **สรุปใบป่ะหน้าคนขับ** | `detail` | menu |
| **PDFชื่องาน_Form** | `form` | ref |

