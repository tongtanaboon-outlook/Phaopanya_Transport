# Format Rules ทั้งหมด (กติกาจัดรูปแบบหน้าจอ)

รวม **11 format rules** — กติกาเหล่านี้เปลี่ยนสี/ตัวหนา/ไอคอนของค่าในหน้าจอตามเงื่อนไข เช่น เปลี่ยนสถานะการอนุมัติเป็นสีเขียวเมื่ออนุมัติแล้ว

## อนุมัติ

- **ใช้กับข้อมูล:** `ข้อมูลการวางบิล` ของ [ข้อมูลการวางบิล](../tables/T04_ข้อมูลการวางบิล/)
- **คอลัมน์/ปุ่มที่จัดรูปแบบ:** `ราคา`, `สถานะการอนุมัติ`
- **ลำดับกติกา:** 1

**เงื่อนไข (If this condition is true):**

```
=[สถานะการอนุมัติ] = "อนุมัติ"
```

**รูปแบบที่ใช้ (Like this):**

```json
{"textColor":"green","highlightColor":"green","textSize":1.1,"underline":false,"strikethrough":false,"bold":true,"italic":false,"uppercase":false,"icon":"fal fa-check","imageSize":null}
```

## รอการอนุมัติ

- **ใช้กับข้อมูล:** `ข้อมูลการวางบิล` ของ [ข้อมูลการวางบิล](../tables/T04_ข้อมูลการวางบิล/)
- **คอลัมน์/ปุ่มที่จัดรูปแบบ:** `ราคา`, `สถานะการอนุมัติ`
- **ลำดับกติกา:** 1

**เงื่อนไข (If this condition is true):**

```
=[สถานะการอนุมัติ] = "รอการอนุมัติ"
```

**รูปแบบที่ใช้ (Like this):**

```json
{"textColor":"orange","highlightColor":"orange","textSize":1.1,"underline":false,"strikethrough":false,"bold":true,"italic":false,"uppercase":false,"icon":"far fa-alarm-clock","imageSize":null}
```

## แจ้งเตือนราคาหลังวิ่งงาน

- **ใช้กับข้อมูล:** `ข้อมูลการวางบิล` ของ [ข้อมูลการวางบิล](../tables/T04_ข้อมูลการวางบิล/)
- **คอลัมน์/ปุ่มที่จัดรูปแบบ:** `ราคาในระบบหลังส่งสินค้า`
- **ลำดับกติกา:** 1

**เงื่อนไข (If this condition is true):**

```
=AND( [ราคาในระบบหลังส่งสินค้า] <> [ราคา], OR( [ชื่องาน] = "นครหลวง", [ชื่องาน] = "โอนคลัง พว", [ชื่องาน] = "โอนคลัง นำ วิวัฒน์", [ชื่องาน] = "โอนคลัง ซอยฮะ (โกเรีย)", [ชื่องาน] = "โอน คลัง TRW", [ชื่องาน] = "โอนคลัง NocNoc", [ชื่องาน] = "โอนคลังCPF FOOD", [ชื่องาน] = "โอนคลัง BYD", [ชื่องาน] = "ภูมิภาค" ) )
```

**รูปแบบที่ใช้ (Like this):**

```json
{"textColor":"red","highlightColor":"red","textSize":1.0,"underline":false,"strikethrough":false,"bold":true,"italic":false,"uppercase":false,"icon":null,"imageSize":null}
```

## แจ้งเตือนเช็คราคาแล้วปกติ

- **ใช้กับข้อมูล:** `ข้อมูลการวางบิล` ของ [ข้อมูลการวางบิล](../tables/T04_ข้อมูลการวางบิล/)
- **คอลัมน์/ปุ่มที่จัดรูปแบบ:** `ราคาในระบบหลังส่งสินค้า`
- **ลำดับกติกา:** 1

**เงื่อนไข (If this condition is true):**

```
=IF([ราคาในระบบหลังส่งสินค้า] = [ราคา], TRUE, FALSE)
```

**รูปแบบที่ใช้ (Like this):**

```json
{"textColor":"green","highlightColor":"green","textSize":1.2,"underline":false,"strikethrough":false,"bold":true,"italic":false,"uppercase":false,"icon":null,"imageSize":null}
```

## ทำเบิกได้

- **ใช้กับข้อมูล:** `ทำเบิกส่วนต่างScgวังน้อย` ของ [ทำเบิกส่วนต่างScgวังน้อย](../tables/T20_ทำเบิกส่วนต่างScgวังน้อย/)
- **คอลัมน์/ปุ่มที่จัดรูปแบบ:** `ขออนุมัติเบิกค่าขนส่งส่วนเพิ่ม`
- **ลำดับกติกา:** 1

**เงื่อนไข (If this condition is true):**

```
=[ขออนุมัติเบิกค่าขนส่งส่วนเพิ่ม] >0
```

**รูปแบบที่ใช้ (Like this):**

```json
{"textColor":"green","highlightColor":"green","textSize":1.0,"underline":false,"strikethrough":false,"bold":true,"italic":false,"uppercase":false,"icon":"far fa-sack-dollar","imageSize":null}
```

## ทำเบิกไม่ได้

- **ใช้กับข้อมูล:** `ทำเบิกส่วนต่างScgวังน้อย` ของ [ทำเบิกส่วนต่างScgวังน้อย](../tables/T20_ทำเบิกส่วนต่างScgวังน้อย/)
- **คอลัมน์/ปุ่มที่จัดรูปแบบ:** `ขออนุมัติเบิกค่าขนส่งส่วนเพิ่ม`
- **ลำดับกติกา:** 1

**เงื่อนไข (If this condition is true):**

```
=[ขออนุมัติเบิกค่าขนส่งส่วนเพิ่ม] < 0
```

**รูปแบบที่ใช้ (Like this):**

```json
{"textColor":"red","highlightColor":"red","textSize":1.0,"underline":false,"strikethrough":true,"bold":false,"italic":false,"uppercase":false,"icon":"far fa-sack-dollar","imageSize":null}
```

## เตือนตรวจสอบ RW

- **ใช้กับข้อมูล:** `SCGนครหลวงJWDภูมิภาค` ของ [SCGนครหลวงJWDภูมิภาค](../tables/T01_SCGนครหลวงJWDภูมิภาค/)
- **คอลัมน์/ปุ่มที่จัดรูปแบบ:** `Shipment No`
- **ลำดับกติกา:** 1

**เงื่อนไข (If this condition is true):**

```
=IN([Invoice No],ข้อมูลงานRW[เลขที่เอกสาร])
```

**รูปแบบที่ใช้ (Like this):**

```json
{"textColor":"red","highlightColor":"red","textSize":1.3,"underline":false,"strikethrough":false,"bold":true,"italic":false,"uppercase":false,"icon":null,"imageSize":null}
```

## Green_Done

- **ใช้กับข้อมูล:** `ตารางงานประจำวัน` ของ [ตารางงานประจำวัน](../tables/T05_ตารางงานประจำวัน/)
- **คอลัมน์/ปุ่มที่จัดรูปแบบ:** `Plan Delivery`, `Invoice No`, `Shipment No`, `ชื่อ - นามสกุล`, `ทะเบียนรถ`, `ชื่อเจ้าของสินค้า`, `ชื่อปลายทาง`
- **ลำดับกติกา:** 1

**เงื่อนไข (If this condition is true):**

```
=[ScanStatus] = "สแกนแล้ว"
```

**รูปแบบที่ใช้ (Like this):**

```json
{"textColor":"green","highlightColor":"green","textSize":1.0,"underline":false,"strikethrough":false,"bold":true,"italic":false,"uppercase":false,"icon":"fal fa-check-circle","imageSize":null}
```

## ผลการตรวจสอบงานส่ง_FAIL

- **ใช้กับข้อมูล:** `SCGนครหลวงJWDภูมิภาค` ของ [SCGนครหลวงJWDภูมิภาค](../tables/T01_SCGนครหลวงJWDภูมิภาค/)
- **คอลัมน์/ปุ่มที่จัดรูปแบบ:** `ระยะขยับจากจุดเริ่มต้น_เมตร`, `ระยะเวลาใช้งาน_นาที`, `ความเร็วการเคลื่อนที่_เมตร_นาที`, `ผลการตรวจสอบงานส่ง`, `เหตุผิดปกติที่ตรวจพบ`
- **ลำดับกติกา:** 1

**เงื่อนไข (If this condition is true):**

```
=[ผลการตรวจสอบงานส่ง] = "FAIL"
```

**รูปแบบที่ใช้ (Like this):**

```json
{"textColor":"primaryText","highlightColor":"red","textSize":1.0,"underline":false,"strikethrough":false,"bold":true,"italic":false,"uppercase":false,"icon":null,"imageSize":null}
```

## สแกนรับแล้ว

- **ใช้กับข้อมูล:** `ตารางงานประจำวัน` ของ [ตารางงานประจำวัน](../tables/T05_ตารางงานประจำวัน/)
- **คอลัมน์/ปุ่มที่จัดรูปแบบ:** `Invoice No`, `ScanStatus`, `ชื่อเจ้าของสินค้า_Invoice_ที่ต้องสแกน`
- **ลำดับกติกา:** 1

**เงื่อนไข (If this condition is true):**

```
=[ScanStatus] = "สแกนรับแล้ว"
```

**รูปแบบที่ใช้ (Like this):**

```json
{"textColor":"green","highlightColor":"green","textSize":1.0,"underline":false,"strikethrough":false,"bold":true,"italic":false,"uppercase":false,"icon":null,"imageSize":null}
```

## รอสแกน

- **ใช้กับข้อมูล:** `ตารางงานประจำวัน` ของ [ตารางงานประจำวัน](../tables/T05_ตารางงานประจำวัน/)
- **คอลัมน์/ปุ่มที่จัดรูปแบบ:** `Invoice No`, `ScanStatus`, `ชื่อเจ้าของสินค้า_Invoice_ที่ต้องสแกน`
- **ลำดับกติกา:** 1

**เงื่อนไข (If this condition is true):**

```
=[ScanStatus] <> "สแกนรับแล้ว"
```

**รูปแบบที่ใช้ (Like this):**

```json
{"textColor":"red","highlightColor":"red","textSize":1.0,"underline":false,"strikethrough":false,"bold":true,"italic":false,"uppercase":false,"icon":null,"imageSize":null}
```

