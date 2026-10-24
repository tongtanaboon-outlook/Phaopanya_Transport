# Slices ของตาราง ตารางงานประจำวัน

รวม **5 slices**

## สรุปงานประจำวัน

| คุณสมบัติ | ค่า |
|---|---|
| Update mode | ALL_CHANGES |
| การมองเห็น | ALWAYS |

**เงื่อนไขการกรอง (Row filter condition):**

```
=[ลำดับแรก] = TRUE
```

**คอลัมน์ที่แสดง (29):** `_RowNumber`, `ID_งานประจำวัน`, `Plan Delivery`, `ชื่อ - นามสกุล`, `ทะเบียนรถ`, `Shipment No`, `ชื่อปลายทาง`, `จำนวนปลายทาง`, `ลำดับแรก`, `ที่อยู่ปลายทาง`, `ที่อยู่ปลายทาง_LatLong`, `หน่วย`, `ItemWeight`, `DeliveryNo`, `ScanStatus`, `Related แจ้งปัญหาระหว่างวันs`, `DeliveryStatus`, `Related SCGนครหลวงJWDภูมิภาคs`, `Email พนักงาน`, `จำนวนสินค้ารวมของร้านนี้`, `น้ำหนักสินค้ารวมของร้านนี้`, `จำนวน_Invoice_ที่ต้องสแกน`, `LatLong_Actual`, `ชื่อเจ้าของสินค้า_Invoice_ที่ต้องสแกน`, `ShopKey`, `Related ScanDocs`, `MATCH_KEY`, `MD_ID`, `LatLong_Actual_Status`

## Slice_Monitor_Today

| คุณสมบัติ | ค่า |
|---|---|
| Update mode | ALL_CHANGES |
| การมองเห็น | ALWAYS |

**เงื่อนไขการกรอง (Row filter condition):**

```
=[ID_งานประจำวัน] = LOOKUP( MIN( SELECT( ตารางงานประจำ วัน[_ROWNUMBER], AND( [Shipment No] = [_THISROW].[Shipment No], [Invoice No] = [_THISROW].[Invoice No] ) ) ), ตารางงานประจำวัน,"_ROWNUMBER", "ID_งานประจำวัน" )
```

**คอลัมน์ที่แสดง (37):** `_RowNumber`, `ScanStatus`, `Invoice No`, `DeliveryNo`, `ชื่อเจ้าของสินค้า`, `Plan Delivery`, `ชื่อปลายทาง`, `Shipment No`, `ชื่อ - นามสกุล`, `ทะเบียนรถ`, `รหัสลูกค้า`, `ที่อยู่ปลายทาง`, `จำนวนสินค้า`, `จำนวนปลายทาง`, `จำนวนจุดที่ส่งจริง`, `ที่อยู่ปลายทาง_LatLong`, `ชื่อวัสดุ`, `หน่วย`, `ItemWeight`, `ลำดับแรก`, `ID_งานประจำวัน`, `รหัสผู้รับเหมา`, `ชื่อผู้รับเหมา`, `Related แจ้งปัญหาระหว่างวันs`, `DeliveryStatus`, `Related SCGนครหลวงJWDภูมิภาคs`, `Email พนักงาน`, `จำนวนสินค้ารวมของร้านนี้`, `น้ำหนักสินค้ารวมของร้านนี้`, `จำนวน_Invoice_ที่ต้องสแกน`, `LatLong_Actual`, `ชื่อเจ้าของสินค้า_Invoice_ที่ต้องสแกน`, `ShopKey`, `Related ScanDocs`, `MATCH_KEY`, `MD_ID`, `LatLong_Actual_Status`

## SM_Today_User

| คุณสมบัติ | ค่า |
|---|---|
| Update mode | ADDS_AND_UPDATES |
| การมองเห็น | ALWAYS |

**เงื่อนไขการกรอง (Row filter condition):**

```
=IF(USERROLE() = "ADMIN", true, AND( [Plan Delivery] = TODAY(), [DeliveryStatus] <> "จัดส่งเรียบร้อย" ) )
```

**คอลัมน์ที่แสดง (40):** `_RowNumber`, `ID_งานประจำวัน`, `Plan Delivery`, `Invoice No`, `Shipment No`, `ชื่อ - นามสกุล`, `ทะเบียนรถ`, `รหัสผู้รับเหมา`, `ชื่อผู้รับเหมา`, `รหัสลูกค้า`, `ชื่อเจ้าของสินค้า`, `ชื่อปลายทาง`, `ที่อยู่ปลายทาง`, `ที่อยู่ปลายทาง_LatLong`, `ชื่อวัสดุ`, `จำนวนสินค้า`, `หน่วย`, `ItemWeight`, `DeliveryNo`, `จำนวนปลายทาง_System`, `ลำดับแรก`, `จำนวนจุดที่ส่งจริง`, `Related แจ้งปัญหาระหว่างวันs`, `รายชื่อปลายทาง_System`, `ScanStatus`, `จำนวนปลายทาง`, `DeliveryStatus`, `เดือน`, `Related SCGนครหลวงJWDภูมิภาคs`, `Email พนักงาน`, `จำนวนสินค้ารวมของร้านนี้`, `น้ำหนักสินค้ารวมของร้านนี้`, `จำนวน_Invoice_ที่ต้องสแกน`, `LatLong_Actual`, `ชื่อเจ้าของสินค้า_Invoice_ที่ต้องสแกน`, `ShopKey`, `Related ScanDocs`, `MATCH_KEY`, `MD_ID`, `LatLong_Actual_Status`

## ค้างสแกนวันนี้และเมื่อวาน

| คุณสมบัติ | ค่า |
|---|---|
| Update mode | ALL_CHANGES |
| การมองเห็น | ALWAYS |

**เงื่อนไขการกรอง (Row filter condition):**

```
=AND( IN([Plan Delivery], LIST(TODAY(), TODAY() - 1)), [ScanStatus]<> "สแกนรับแล้ว" )
```

**คอลัมน์ที่แสดง (40):** `_RowNumber`, `ID_งานประจำวัน`, `Plan Delivery`, `Invoice No`, `Shipment No`, `ชื่อ - นามสกุล`, `ทะเบียนรถ`, `รหัสผู้รับเหมา`, `ชื่อผู้รับเหมา`, `รหัสลูกค้า`, `ชื่อเจ้าของสินค้า`, `ชื่อปลายทาง`, `ที่อยู่ปลายทาง`, `ที่อยู่ปลายทาง_LatLong`, `ชื่อวัสดุ`, `จำนวนสินค้า`, `หน่วย`, `ItemWeight`, `DeliveryNo`, `จำนวนปลายทาง_System`, `รายชื่อปลายทาง_System`, `ScanStatus`, `DeliveryStatus`, `Email พนักงาน`, `จำนวนสินค้ารวมของร้านนี้`, `น้ำหนักสินค้ารวมของร้านนี้`, `จำนวน_Invoice_ที่ต้องสแกน`, `LatLong_Actual`, `ชื่อเจ้าของสินค้า_Invoice_ที่ต้องสแกน`, `ShopKey`, `จำนวนปลายทาง`, `ลำดับแรก`, `จำนวนจุดที่ส่งจริง`, `เดือน`, `Related SCGนครหลวงJWDภูมิภาคs`, `Related แจ้งปัญหาระหว่างวันs`, `Related ScanDocs`, `MATCH_KEY`, `MD_ID`, `LatLong_Actual_Status`

## SM_Today_User 2

| คุณสมบัติ | ค่า |
|---|---|
| Update mode | ADDS_AND_UPDATES |
| การมองเห็น | ALWAYS |

**เงื่อนไขการกรอง (Row filter condition):**

```
=IF(USERROLE() = "ADMIN",true, AND( [Plan Delivery] = TODAY(), [Email พนักงาน] = USEREMAIL() ) )
```

**คอลัมน์ที่แสดง (40):** `_RowNumber`, `ID_งานประจำวัน`, `Plan Delivery`, `Invoice No`, `Shipment No`, `ชื่อ - นามสกุล`, `ทะเบียนรถ`, `รหัสผู้รับเหมา`, `ชื่อผู้รับเหมา`, `รหัสลูกค้า`, `ชื่อเจ้าของสินค้า`, `ชื่อปลายทาง`, `ที่อยู่ปลายทาง`, `ที่อยู่ปลายทาง_LatLong`, `ชื่อวัสดุ`, `จำนวนสินค้า`, `หน่วย`, `ItemWeight`, `DeliveryNo`, `จำนวนปลายทาง_System`, `ลำดับแรก`, `จำนวนจุดที่ส่งจริง`, `Related แจ้งปัญหาระหว่างวันs`, `รายชื่อปลายทาง_System`, `ScanStatus`, `จำนวนปลายทาง`, `DeliveryStatus`, `เดือน`, `Related SCGนครหลวงJWDภูมิภาคs`, `Email พนักงาน`, `จำนวนสินค้ารวมของร้านนี้`, `น้ำหนักสินค้ารวมของร้านนี้`, `จำนวน_Invoice_ที่ต้องสแกน`, `LatLong_Actual`, `ชื่อเจ้าของสินค้า_Invoice_ที่ต้องสแกน`, `ShopKey`, `Related ScanDocs`, `MATCH_KEY`, `MD_ID`, `LatLong_Actual_Status`

