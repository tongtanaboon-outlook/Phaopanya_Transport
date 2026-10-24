# สารบัญ Actions ทั้งหมด (214 รายการ)

Actions คือปุ่มกด/การกระทำที่ผู้ใช้เรียกใช้ได้ในแอป (หรือที่ Bot เรียกใช้) รายละเอียดเต็มของแต่ละ action (สูตรเงื่อนไข ค่าที่ตั้ง JSON) อยู่ในไฟล์ `ACTIONS.md` ของแต่ละตาราง

## สรุปตามประเภทการทำงาน (Do this)

| Do this | จำนวน |
|---|---:|
| `SET_COLUMN_VALUE` | 49 |
| `ADD_RECORD` | 29 |
| `EDIT_RECORD` | 29 |
| `DELETE_RECORD` | 29 |
| `NAVIGATE_APP` | 29 |
| `EXPORT_VIEW` | 21 |
| `EMAIL` | 12 |
| `REF_ACTION` | 4 |
| `COMPOSITE` | 3 |
| `NAVIGATE_DIFFERENT_APP` | 3 |
| `NAVIGATE_URL` | 3 |
| `CALL` | 1 |
| `SMS` | 1 |
| `ADD_RECORD_TO` | 1 |

## [SCGนครหลวงJWDภูมิภาค](../tables/T01_SCGนครหลวงJWDภูมิภาค/) — 13 actions

| Action | Do this | Prominence | เงื่อนไข? |
|---|---|---|---|
| **Compose Email (Email พนักงาน)** | `EMAIL` | `Display_Inline` | ✓ |
| **Add** | `ADD_RECORD` | `Display_Overlay` |  |
| **Edit** | `EDIT_RECORD` | `Display_Overlay` |  |
| **Delete** | `DELETE_RECORD` | `Display_Prominently` |  |
| **View Map (จุดส่งสินค้าปลายทาง)** | `NAVIGATE_APP` | `Display_Inline` | ✓ |
| **View Ref (ID_เอกสารนำกลับคืนคลัง)** | `NAVIGATE_APP` | `Display_Inline` | ✓ |
| **View Map (คลังสินค้า เอสซีจี เจดับเบิ้ลยูดี วังน้อย)** | `NAVIGATE_APP` | `Display_Inline` | ✓ |
| **View Map (ที่อยู่ปลายทาง_LatLong_Api)** | `NAVIGATE_APP` | `Display_Inline` | ✓ |
| **SCGนครหลวงJWDภูมิภาค_csv** | `EXPORT_VIEW` | `Display_Prominently` | ✓ |
| **Process_Delivery_Status_Bot Action - 1** | `REF_ACTION` | `Do_Not_Display` | ✓ |
| **View Ref (SM_Link_SCG)** | `NAVIGATE_APP` | `Display_Inline` | ✓ |
| **View Ref (ID_พนักงาน)** | `NAVIGATE_APP` | `Display_Inline` | ✓ |
| **View Map (พิกัดตอนกดบันทึกงาน)** | `NAVIGATE_APP` | `Display_Inline` | ✓ |

## [ข้อมูลการเข้าบำรุงรักษา](../tables/T03_ข้อมูลการเข้าบำรุงรักษา/) — 6 actions

| Action | Do this | Prominence | เงื่อนไข? |
|---|---|---|---|
| **Compose Email (Email พนักงาน)** | `EMAIL` | `Display_Inline` | ✓ |
| **Add** | `ADD_RECORD` | `Display_Overlay` |  |
| **Delete** | `DELETE_RECORD` | `Display_Prominently` |  |
| **Edit** | `EDIT_RECORD` | `Display_Overlay` |  |
| **ข้อมูลการเข้าบำรุงรักษาcsv** | `EXPORT_VIEW` | `Display_Prominently` | ✓ |
| **View Ref (ID_พนักงาน)** | `NAVIGATE_APP` | `Display_Inline` | ✓ |

## [ข้อมูลการวางบิล](../tables/T04_ข้อมูลการวางบิล/) — 10 actions

| Action | Do this | Prominence | เงื่อนไข? |
|---|---|---|---|
| **Compose Email (Email พนักงาน)** | `EMAIL` | `Display_Inline` | ✓ |
| **Compose Email (Email ผู้อนุมัติ)** | `EMAIL` | `Display_Inline` | ✓ |
| **Add** | `ADD_RECORD` | `Display_Overlay` |  |
| **อนุมัติ** | `SET_COLUMN_VALUE` | `Display_Prominently` | ✓ |
| **รอการอนุมัติ** | `SET_COLUMN_VALUE` | `Display_Inline` | ✓ |
| **Edit** | `EDIT_RECORD` | `Display_Overlay` |  |
| **Delete** | `DELETE_RECORD` | `Display_Prominently` |  |
| **ส่งรูปวางบิลหรือสลิปโอนเงิน** | `NAVIGATE_DIFFERENT_APP` | `Display_Prominently` | ✓ |
| **ข้อมูลการวางบิลcsv** | `EXPORT_VIEW` | `Display_Prominently` | ✓ |
| **View Ref (ID_พนักงาน)** | `NAVIGATE_APP` | `Display_Inline` | ✓ |

## [ตารางงานประจำวัน](../tables/T05_ตารางงานประจำวัน/) — 10 actions

| Action | Do this | Prominence | เงื่อนไข? |
|---|---|---|---|
| **Delete** | `DELETE_RECORD` | `Display_Prominently` |  |
| **Edit** | `EDIT_RECORD` | `Display_Overlay` |  |
| **Add** | `ADD_RECORD` | `Display_Overlay` |  |
| **View Map (ที่อยู่ปลายทาง_LatLong)** | `NAVIGATE_APP` | `Display_Inline` | ✓ |
| **ตารางงานประจำวันcsv** | `EXPORT_VIEW` | `Display_Prominently` | ✓ |
| **Mark_As_Delivered** | `SET_COLUMN_VALUE` | `Do_Not_Display` | ✓ |
| **Mark_As_Delivered_not** | `SET_COLUMN_VALUE` | `Do_Not_Display` | ✓ |
| **Compose Email (Email พนักงาน)** | `EMAIL` | `Display_Inline` | ✓ |
| **View Map (LatLong_Actual)** | `NAVIGATE_APP` | `Display_Inline` | ✓ |
| **Update ScanStatus** | `SET_COLUMN_VALUE` | `Do_Not_Display` | ✓ |

## [ราคาน้ำมันดีเซล](../tables/T06_ราคาน้ำมันดีเซล/) — 4 actions

| Action | Do this | Prominence | เงื่อนไข? |
|---|---|---|---|
| **Add** | `ADD_RECORD` | `Display_Overlay` |  |
| **Delete** | `DELETE_RECORD` | `Display_Prominently` |  |
| **Edit** | `EDIT_RECORD` | `Display_Overlay` |  |
| **ราคาน้ำมันดีเซลcsv** | `EXPORT_VIEW` | `Display_Prominently` | ✓ |

## [ราคาในระบบก่อนส่งสินค้า](../tables/T07_ราคาในระบบก่อนส่งสินค้า/) — 4 actions

| Action | Do this | Prominence | เงื่อนไข? |
|---|---|---|---|
| **Delete** | `DELETE_RECORD` | `Display_Prominently` |  |
| **Edit** | `EDIT_RECORD` | `Display_Overlay` |  |
| **Add** | `ADD_RECORD` | `Display_Overlay` |  |
| **ราคาในระบบก่อนส่งสินค้าcsv** | `EXPORT_VIEW` | `Display_Prominently` | ✓ |

## [หน้าหลัก](../tables/T08_หน้าหลัก/) — 5 actions

| Action | Do this | Prominence | เงื่อนไข? |
|---|---|---|---|
| **Delete** | `DELETE_RECORD` | `Display_Prominently` |  |
| **Edit** | `EDIT_RECORD` | `Display_Overlay` |  |
| **Add** | `ADD_RECORD` | `Display_Overlay` |  |
| **GoToView** | `NAVIGATE_APP` | `Do_Not_Display` | ✓ |
| **หน้าหลักcsv** | `EXPORT_VIEW` | `Display_Prominently` | ✓ |

## [ปริ๊นใบวางบิล](../tables/T09_ปริ๊นใบวางบิล/) — 21 actions

| Action | Do this | Prominence | เงื่อนไข? |
|---|---|---|---|
| **Edit** | `EDIT_RECORD` | `Display_Overlay` |  |
| **Add** | `ADD_RECORD` | `Display_Overlay` |  |
| **Clear** | `SET_COLUMN_VALUE` | `Do_Not_Display` | ✓ |
| **Delete** | `DELETE_RECORD` | `Display_Prominently` |  |
| **ไอโรบอท** | `SET_COLUMN_VALUE` | `Do_Not_Display` | ✓ |
| **รับเอกสาร (งานพี่เหน่ง)** | `SET_COLUMN_VALUE` | `Do_Not_Display` | ✓ |
| **โอนคลัง เอเธน** | `SET_COLUMN_VALUE` | `Do_Not_Display` | ✓ |
| **โอนคลัง กระสอบ2(บางบัวทอง)** | `SET_COLUMN_VALUE` | `Do_Not_Display` | ✓ |
| **คลังSCGJWDวังน้อย** | `SET_COLUMN_VALUE` | `Do_Not_Display` | ✓ |
| **MeSpace** | `SET_COLUMN_VALUE` | `Do_Not_Display` | ✓ |
| **โอนคลัง มโนยนต์ (นวนคร)** | `SET_COLUMN_VALUE` | `Do_Not_Display` | ✓ |
| **โอนคลัง (GQ) จีคิว** | `SET_COLUMN_VALUE` | `Do_Not_Display` | ✓ |
| **ปริ๊นวางบิลทุกงาน** | `COMPOSITE` | `Display_Prominently` | ✓ |
| **เคลียหน้าจอ** | `SET_COLUMN_VALUE` | `Display_Prominently` | ✓ |
| **รับเอกสาร (งานพี่เหน่ง) สตีเบล** | `SET_COLUMN_VALUE` | `Do_Not_Display` | ✓ |
| **CLEAR_ปริ๊นใบวางบิล_Action** | `SET_COLUMN_VALUE` | `Do_Not_Display` | ✓ |
| **ปริ๊นใบวางบิลcsv** | `EXPORT_VIEW` | `Display_Prominently` | ✓ |
| **เบทาโกร+เหมาตู้** | `SET_COLUMN_VALUE` | `Do_Not_Display` | ✓ |
| **Thai paper (SCG Express)** | `SET_COLUMN_VALUE` | `Do_Not_Display` | ✓ |
| **LINEMAN (6W) (SCG Express)** | `SET_COLUMN_VALUE` | `Do_Not_Display` | ✓ |
| **โอนคลัง บุญถาวร เกษตร_นวมินทร์** | `SET_COLUMN_VALUE` | `Do_Not_Display` | ✓ |

## [PDFพนักงาน](../tables/T10_PDFพนักงาน/) — 26 actions

| Action | Do this | Prominence | เงื่อนไข? |
|---|---|---|---|
| **Edit** | `EDIT_RECORD` | `Display_Overlay` |  |
| **Add** | `ADD_RECORD` | `Display_Overlay` |  |
| **CLEAR 2** | `SET_COLUMN_VALUE` | `Display_Prominently` | ✓ |
| **Delete** | `DELETE_RECORD` | `Display_Prominently` |  |
| **สร้างใบป่ะหน้า_สำเริง แก้วกามเกตุ** | `SET_COLUMN_VALUE` | `Do_Not_Display` | ✓ |
| **สร้างใบป่ะหน้าทุกคน** | `COMPOSITE` | `Display_Prominently` | ✓ |
| **Clearหน้าจอ** | `SET_COLUMN_VALUE` | `Do_Not_Display` | ✓ |
| **สร้างใบป่ะหน้า_สุทิศ นันพนัก** | `SET_COLUMN_VALUE` | `Do_Not_Display` | ✓ |
| **สร้างใบป่ะหน้า_เอกรัฐ อนุรักษ์** | `SET_COLUMN_VALUE` | `Do_Not_Display` | ✓ |
| **สร้างใบป่ะหน้า_สุด พันพม่า** | `SET_COLUMN_VALUE` | `Do_Not_Display` | ✓ |
| **สร้างใบป่ะหน้า_ธวัชชัย หนูมา** | `SET_COLUMN_VALUE` | `Do_Not_Display` | ✓ |
| **สร้างใบป่ะหน้า_ปราโมทย์ เรียนพิษ** | `SET_COLUMN_VALUE` | `Do_Not_Display` | ✓ |
| **สร้างใบป่ะหน้า_กฤษฎา พิญญะดำ** | `SET_COLUMN_VALUE` | `Do_Not_Display` | ✓ |
| **สร้างใบป่ะหน้า_กิตติพงษ์ แหลมผักแว่น** | `SET_COLUMN_VALUE` | `Do_Not_Display` | ✓ |
| **สร้างใบป่ะหน้า_จักรภัทร วงทอง** | `SET_COLUMN_VALUE` | `Do_Not_Display` | ✓ |
| **สร้างใบป่ะหน้า_พีระพล รูปแก้ว** | `SET_COLUMN_VALUE` | `Do_Not_Display` | ✓ |
| **สร้างใบป่ะหน้า_อชิตพล ยังยิ้ม** | `SET_COLUMN_VALUE` | `Do_Not_Display` | ✓ |
| **สร้างใบป่ะหน้า_ธีรยุทธ นราทอง** | `SET_COLUMN_VALUE` | `Do_Not_Display` | ✓ |
| **สร้างใบป่ะหน้า_จิรายุ โคตรวงษ์** | `SET_COLUMN_VALUE` | `Do_Not_Display` | ✓ |
| **สร้างใบป่ะหน้า_ทัดเทพ พรมมา** | `SET_COLUMN_VALUE` | `Do_Not_Display` | ✓ |
| **สร้างใบป่ะหน้า_พงศธร หมวดไธสง** | `SET_COLUMN_VALUE` | `Do_Not_Display` | ✓ |
| **สร้างใบป่ะหน้า_เกียรติศักดิ์ พินิจเมือง** | `SET_COLUMN_VALUE` | `Do_Not_Display` | ✓ |
| **สร้างใบป่ะหน้า_เกียรติศักดิ์ ยอมใหญ่** | `SET_COLUMN_VALUE` | `Do_Not_Display` | ✓ |
| **PDFพนักงานcsv** | `EXPORT_VIEW` | `Display_Prominently` | ✓ |
| **สร้างใบป่ะหน้า_สิทธิชัย ทิศวงค์** | `SET_COLUMN_VALUE` | `Do_Not_Display` | ✓ |
| **สร้างใบป่ะหน้า_ไนยชน วงศ์บุญมา** | `SET_COLUMN_VALUE` | `Do_Not_Display` | ✓ |

## [แจ้งปัญหาระหว่างวัน](../tables/T11_แจ้งปัญหาระหว่างวัน/) — 14 actions

| Action | Do this | Prominence | เงื่อนไข? |
|---|---|---|---|
| **Edit** | `EDIT_RECORD` | `Display_Overlay` |  |
| **Compose Email (Email พนักงาน)** | `EMAIL` | `Display_Inline` | ✓ |
| **Add** | `ADD_RECORD` | `Display_Overlay` |  |
| **Delete** | `DELETE_RECORD` | `Display_Prominently` |  |
| **ส่งรูปแจ้งปัญหา** | `NAVIGATE_DIFFERENT_APP` | `Display_Prominently` | ✓ |
| **View Map (Lat/Long)** | `NAVIGATE_APP` | `Display_Inline` | ✓ |
| **เพิ่มข้อมูลแจ้งปัญหาในจุดส่งงาน** | `ADD_RECORD_TO` | `Do_Not_Display` | ✓ |
| **แจ้งปัญหาระหว่างวันcsv** | `EXPORT_VIEW` | `Display_Prominently` | ✓ |
| **View Ref (SM_Link)** | `NAVIGATE_APP` | `Display_Inline` | ✓ |
| **View Ref (RT_Link)** | `NAVIGATE_APP` | `Display_Inline` | ✓ |
| **ACT_Create_SCG_Flow** | `COMPOSITE` | `Do_Not_Display` | ✓ |
| **New Action** | `REF_ACTION` | `Do_Not_Display` | ✓ |
| **View Ref (ID_พนักงาน)** | `NAVIGATE_APP` | `Display_Inline` | ✓ |
| **View Map (LatLong_ตรวจสอบ)** | `NAVIGATE_APP` | `Display_Inline` | ✓ |

## [รับงานคืนได้เงิน200](../tables/T12_รับงานคืนได้เงิน200/) — 9 actions

| Action | Do this | Prominence | เงื่อนไข? |
|---|---|---|---|
| **Compose Email (Email พนักงาน)** | `EMAIL` | `Display_Inline` | ✓ |
| **Add** | `ADD_RECORD` | `Display_Overlay` |  |
| **Delete** | `DELETE_RECORD` | `Display_Prominently` |  |
| **Edit** | `EDIT_RECORD` | `Display_Overlay` |  |
| **View Map (Lat / Long)** | `NAVIGATE_APP` | `Display_Inline` | ✓ |
| **Chart Data for รับงานคืนได้เงิน200** | `NAVIGATE_APP` | `Display_Prominently` | ✓ |
| **ส่งรูปจุดที่ส่งงาน** | `NAVIGATE_DIFFERENT_APP` | `Display_Prominently` | ✓ |
| **รับงานคืนได้เงิน200csv** | `EXPORT_VIEW` | `Display_Prominently` | ✓ |
| **View Ref (ID_พนักงาน)** | `NAVIGATE_APP` | `Display_Inline` | ✓ |

## [ข้อมูลงานRT](../tables/T13_ข้อมูลงานRT/) — 4 actions

| Action | Do this | Prominence | เงื่อนไข? |
|---|---|---|---|
| **Delete** | `DELETE_RECORD` | `Display_Prominently` |  |
| **Edit** | `EDIT_RECORD` | `Display_Overlay` |  |
| **Add** | `ADD_RECORD` | `Display_Overlay` |  |
| **ข้อมูลงานRTcsv** | `EXPORT_VIEW` | `Display_Prominently` | ✓ |

## [FILTER](../tables/T14_FILTER/) — 6 actions

| Action | Do this | Prominence | เงื่อนไข? |
|---|---|---|---|
| **Delete** | `DELETE_RECORD` | `Display_Prominently` |  |
| **Edit** | `EDIT_RECORD` | `Display_Overlay` |  |
| **Add** | `ADD_RECORD` | `Display_Overlay` |  |
| **cLeAR_รับคืน** | `SET_COLUMN_VALUE` | `Display_Prominently` | ✓ |
| **เคลียสรุปจุดส่ง Action - 1** | `SET_COLUMN_VALUE` | `Display_Prominently` | ✓ |
| **FILTERcsv** | `EXPORT_VIEW` | `Display_Prominently` | ✓ |

## [ข้อมูลพนักงาน](../tables/T15_ข้อมูลพนักงาน/) — 7 actions

| Action | Do this | Prominence | เงื่อนไข? |
|---|---|---|---|
| **Compose Email (Email พนักงาน)** | `EMAIL` | `Display_Inline` | ✓ |
| **Call Phone (เบอร์โทรศัพท์)** | `CALL` | `Display_Inline` | ✓ |
| **Delete** | `DELETE_RECORD` | `Display_Prominently` |  |
| **Edit** | `EDIT_RECORD` | `Display_Overlay` |  |
| **Add** | `ADD_RECORD` | `Display_Overlay` |  |
| **Send SMS (เบอร์โทรศัพท์)** | `SMS` | `Display_Inline` | ✓ |
| **ข้อมูลพนักงานcsv** | `EXPORT_VIEW` | `Display_Prominently` | ✓ |

## [ข้อมูลชื่องานต้นทางปลายทาง](../tables/T16_ข้อมูลชื่องานต้นทางปลายทาง/) — 4 actions

| Action | Do this | Prominence | เงื่อนไข? |
|---|---|---|---|
| **Add** | `ADD_RECORD` | `Display_Overlay` |  |
| **Delete** | `DELETE_RECORD` | `Display_Prominently` |  |
| **Edit** | `EDIT_RECORD` | `Display_Overlay` |  |
| **ข้อมูลชื่องานต้นทางปลายทางcsv** | `EXPORT_VIEW` | `Display_Prominently` | ✓ |

## [สรุปเบิกส่วนต่าง](../tables/T17_สรุปเบิกส่วนต่าง/) — 6 actions

| Action | Do this | Prominence | เงื่อนไข? |
|---|---|---|---|
| **Delete** | `DELETE_RECORD` | `Display_Prominently` |  |
| **Edit** | `EDIT_RECORD` | `Display_Overlay` |  |
| **Add** | `ADD_RECORD` | `Display_Overlay` |  |
| **View Ref (_ComputedKey_ID_SCGนครหลวงJWDภูมิภาค)** | `NAVIGATE_APP` | `Display_Inline` | ✓ |
| **Clearหน้าจอสรุปส่วนต่าง** | `SET_COLUMN_VALUE` | `Display_Prominently` | ✓ |
| **สรุปเบิกส่วนต่างcsv** | `EXPORT_VIEW` | `Display_Prominently` | ✓ |

## [Doc_Return](../tables/T18_Doc_Return/) — 4 actions

| Action | Do this | Prominence | เงื่อนไข? |
|---|---|---|---|
| **Delete** | `DELETE_RECORD` | `Display_Prominently` |  |
| **Edit** | `EDIT_RECORD` | `Display_Overlay` |  |
| **Add** | `ADD_RECORD` | `Display_Overlay` |  |
| **Doc_Return_csv** | `EXPORT_VIEW` | `Display_Prominently` | ✓ |

## [Image_Doc_Return](../tables/T19_Image_Doc_Return/) — 5 actions

| Action | Do this | Prominence | เงื่อนไข? |
|---|---|---|---|
| **Delete** | `DELETE_RECORD` | `Display_Prominently` |  |
| **Edit** | `EDIT_RECORD` | `Display_Overlay` |  |
| **Add** | `ADD_RECORD` | `Display_Overlay` |  |
| **View Ref (ID_Doc_Return)** | `NAVIGATE_APP` | `Display_Inline` | ✓ |
| **Image_Doc_Return_csv** | `EXPORT_VIEW` | `Display_Prominently` | ✓ |

## [ทำเบิกส่วนต่างScgวังน้อย](../tables/T20_ทำเบิกส่วนต่างScgวังน้อย/) — 15 actions

| Action | Do this | Prominence | เงื่อนไข? |
|---|---|---|---|
| **Delete** | `DELETE_RECORD` | `Display_Prominently` |  |
| **Edit** | `EDIT_RECORD` | `Display_Overlay` |  |
| **Add** | `ADD_RECORD` | `Display_Overlay` |  |
| **View Ref (_ComputedKey_ID_SCGนครหลวงJWDภูมิภาค)** | `NAVIGATE_APP` | `Display_Inline` | ✓ |
| **View Map (ต้นทาง)** | `NAVIGATE_APP` | `Display_Inline` | ✓ |
| **Compose Email (Email พนักงาน)** | `EMAIL` | `Display_Inline` | ✓ |
| **อัพเดตค่าสถานะผ่านการตรวจสอบ** | `SET_COLUMN_VALUE` | `Display_Prominently` | ✓ |
| **Open Url (แสดงแผนที่_GoogleMapsRoutesAPI)** | `NAVIGATE_URL` | `Display_Inline` | ✓ |
| **อัพเดตสถานะไม่ผ่านการตรวจสอบ** | `SET_COLUMN_VALUE` | `Display_Prominently` | ✓ |
| **ปุ่มเปิดYes 2** | `SET_COLUMN_VALUE` | `Display_Prominently` | ✓ |
| **ทำเบิกส่วนต่างScgวังน้อยcsv** | `EXPORT_VIEW` | `Display_Prominently` | ✓ |
| **View Ref (ID_พนักงาน)** | `NAVIGATE_APP` | `Display_Inline` | ✓ |
| **ปุ่มเปิดYes_ราคาตามระยะทาง** | `SET_COLUMN_VALUE` | `Display_Prominently` | ✓ |
| **Open Url (Candidate_2_แสดงแผนที่)** | `NAVIGATE_URL` | `Display_Inline` | ✓ |
| **Open Url (Candidate_3_แสดงแผนที่)** | `NAVIGATE_URL` | `Display_Inline` | ✓ |

## [ข้อมูลงานRW](../tables/T21_ข้อมูลงานRW/) — 4 actions

| Action | Do this | Prominence | เงื่อนไข? |
|---|---|---|---|
| **Edit** | `EDIT_RECORD` | `Display_Overlay` |  |
| **Add** | `ADD_RECORD` | `Display_Overlay` |  |
| **ข้อมูลงานRWcsv** | `EXPORT_VIEW` | `Display_Prominently` | ✓ |
| **Delete** | `DELETE_RECORD` | `Display_Prominently` |  |

## [สร้างเอกสาร](../tables/T22_สร้างเอกสาร/) — 3 actions

| Action | Do this | Prominence | เงื่อนไข? |
|---|---|---|---|
| **Delete** | `DELETE_RECORD` | `Display_Prominently` |  |
| **Edit** | `EDIT_RECORD` | `Display_Overlay` |  |
| **Add** | `ADD_RECORD` | `Display_Overlay` |  |

## [ScanDocs](../tables/T23_ScanDocs/) — 7 actions

| Action | Do this | Prominence | เงื่อนไข? |
|---|---|---|---|
| **Delete** | `DELETE_RECORD` | `Display_Prominently` |  |
| **Edit** | `EDIT_RECORD` | `Display_Overlay` |  |
| **Compose Email (Scan_By)** | `EMAIL` | `Display_Inline` | ✓ |
| **Add** | `ADD_RECORD` | `Display_Overlay` |  |
| **ScanStatus** | `REF_ACTION` | `Do_Not_Display` | ✓ |
| **View Ref (Invoice_No)** | `NAVIGATE_APP` | `Display_Inline` | ✓ |
| **Update Action - 1** | `REF_ACTION` | `Display_Prominently` | ✓ |

## [สรุป_เจ้าของสินค้า](../tables/T24_สรุป_เจ้าของสินค้า/) — 3 actions

| Action | Do this | Prominence | เงื่อนไข? |
|---|---|---|---|
| **Delete** | `DELETE_RECORD` | `Display_Prominently` |  |
| **Edit** | `EDIT_RECORD` | `Display_Overlay` |  |
| **Add** | `ADD_RECORD` | `Display_Overlay` |  |

## [สรุป_Shipment](../tables/T25_สรุป_Shipment/) — 3 actions

| Action | Do this | Prominence | เงื่อนไข? |
|---|---|---|---|
| **Delete** | `DELETE_RECORD` | `Display_Prominently` |  |
| **Edit** | `EDIT_RECORD` | `Display_Overlay` |  |
| **Add** | `ADD_RECORD` | `Display_Overlay` |  |

## [PriceOverride](../tables/T26_PriceOverride/) — 3 actions

| Action | Do this | Prominence | เงื่อนไข? |
|---|---|---|---|
| **Delete** | `DELETE_RECORD` | `Display_Prominently` |  |
| **Edit** | `EDIT_RECORD` | `Display_Overlay` |  |
| **Add** | `ADD_RECORD` | `Display_Overlay` |  |

## [Price_Table](../tables/T27_Price_Table/) — 4 actions

| Action | Do this | Prominence | เงื่อนไข? |
|---|---|---|---|
| **Delete** | `DELETE_RECORD` | `Display_Prominently` |  |
| **Edit** | `EDIT_RECORD` | `Display_Overlay` |  |
| **Add** | `ADD_RECORD` | `Display_Overlay` |  |
| **Price_Table_csv** | `EXPORT_VIEW` | `Display_Prominently` | ✓ |

## [ส่งงานที่ยังไม่มีข้อมูลในระบบ](../tables/T28_ส่งงานที่ยังไม่มีข้อมูลในระบบ/) — 6 actions

| Action | Do this | Prominence | เงื่อนไข? |
|---|---|---|---|
| **Delete** | `DELETE_RECORD` | `Display_Prominently` |  |
| **Edit** | `EDIT_RECORD` | `Display_Overlay` |  |
| **Compose Email (Email พนักงาน)** | `EMAIL` | `Display_Inline` | ✓ |
| **Add** | `ADD_RECORD` | `Display_Overlay` |  |
| **View Map (จุดส่งสินค้าปลายทาง)** | `NAVIGATE_APP` | `Display_Inline` | ✓ |
| **View Ref (ID_พนักงาน)** | `NAVIGATE_APP` | `Display_Inline` | ✓ |

## [Acknowledge_Logs](../tables/T29_Acknowledge_Logs/) — 5 actions

| Action | Do this | Prominence | เงื่อนไข? |
|---|---|---|---|
| **Delete** | `DELETE_RECORD` | `Display_Prominently` |  |
| **Edit** | `EDIT_RECORD` | `Display_Overlay` |  |
| **Compose Email (Email พนักงาน)** | `EMAIL` | `Display_Inline` | ✓ |
| **Add** | `ADD_RECORD` | `Display_Overlay` | ✓ |
| **View Ref (ID_ประกาศ)** | `NAVIGATE_APP` | `Display_Inline` | ✓ |

## [Announcements](../tables/T30_Announcements/) — 3 actions

| Action | Do this | Prominence | เงื่อนไข? |
|---|---|---|---|
| **Delete** | `DELETE_RECORD` | `Display_Prominently` |  |
| **Edit** | `EDIT_RECORD` | `Display_Overlay` |  |
| **Add** | `ADD_RECORD` | `Display_Overlay` |  |

