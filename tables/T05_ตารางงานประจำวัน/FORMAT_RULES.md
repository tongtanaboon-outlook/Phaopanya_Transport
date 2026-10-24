# Format Rules ของตาราง ตารางงานประจำวัน

รวม **3 format rules**

## Green_Done

- **ใช้กับข้อมูล:** `ตารางงานประจำวัน`
- **รูปแบบที่ใช้กับ:** `Plan Delivery`, `Invoice No`, `Shipment No`, `ชื่อ - นามสกุล`, `ทะเบียนรถ`, `ชื่อเจ้าของสินค้า`, `ชื่อปลายทาง`
**เงื่อนไข:**

```
=[ScanStatus] = "สแกนแล้ว"
```

**รูปแบบที่ใช้ (Like this):**

```json
{"textColor":"green","highlightColor":"green","textSize":1.0,"underline":false,"strikethrough":false,"bold":true,"italic":false,"uppercase":false,"icon":"fal fa-check-circle","imageSize":null}
```

- **ลำดับ:** 1
- **ปิดใช้งาน?:** No
- **การมองเห็น:** ALWAYS

## สแกนรับแล้ว

- **ใช้กับข้อมูล:** `ตารางงานประจำวัน`
- **รูปแบบที่ใช้กับ:** `Invoice No`, `ScanStatus`, `ชื่อเจ้าของสินค้า_Invoice_ที่ต้องสแกน`
**เงื่อนไข:**

```
=[ScanStatus] = "สแกนรับแล้ว"
```

**รูปแบบที่ใช้ (Like this):**

```json
{"textColor":"green","highlightColor":"green","textSize":1.0,"underline":false,"strikethrough":false,"bold":true,"italic":false,"uppercase":false,"icon":null,"imageSize":null}
```

- **ลำดับ:** 1
- **ปิดใช้งาน?:** No
- **การมองเห็น:** ALWAYS

## รอสแกน

- **ใช้กับข้อมูล:** `ตารางงานประจำวัน`
- **รูปแบบที่ใช้กับ:** `Invoice No`, `ScanStatus`, `ชื่อเจ้าของสินค้า_Invoice_ที่ต้องสแกน`
**เงื่อนไข:**

```
=[ScanStatus] <> "สแกนรับแล้ว"
```

**รูปแบบที่ใช้ (Like this):**

```json
{"textColor":"red","highlightColor":"red","textSize":1.0,"underline":false,"strikethrough":false,"bold":true,"italic":false,"uppercase":false,"icon":null,"imageSize":null}
```

- **ลำดับ:** 1
- **ปิดใช้งาน?:** No
- **การมองเห็น:** ALWAYS Behavior

