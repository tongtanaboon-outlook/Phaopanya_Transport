# Format Rules ของตาราง SCGนครหลวงJWDภูมิภาค

รวม **2 format rules**

## เตือนตรวจสอบ RW

- **ใช้กับข้อมูล:** `SCGนครหลวงJWDภูมิภาค`
- **รูปแบบที่ใช้กับ:** `Shipment No`
**เงื่อนไข:**

```
=IN([Invoice No],ข้อมูลงานRW[เลขที่เอกสาร])
```

**รูปแบบที่ใช้ (Like this):**

```json
{"textColor":"red","highlightColor":"red","textSize":1.3,"underline":false,"strikethrough":false,"bold":true,"italic":false,"uppercase":false,"icon":null,"imageSize":null}
```

- **ลำดับ:** 1
- **ปิดใช้งาน?:** No
- **การมองเห็น:** ALWAYS

## ผลการตรวจสอบงานส่ง_FAIL

- **ใช้กับข้อมูล:** `SCGนครหลวงJWDภูมิภาค`
- **รูปแบบที่ใช้กับ:** `ระยะขยับจากจุดเริ่มต้น_เมตร`, `ระยะเวลาใช้งาน_นาที`, `ความเร็วการเคลื่อนที่_เมตร_นาที`, `ผลการตรวจสอบงานส่ง`, `เหตุผิดปกติที่ตรวจพบ`
**เงื่อนไข:**

```
=[ผลการตรวจสอบงานส่ง] = "FAIL"
```

**รูปแบบที่ใช้ (Like this):**

```json
{"textColor":"primaryText","highlightColor":"red","textSize":1.0,"underline":false,"strikethrough":false,"bold":true,"italic":false,"uppercase":false,"icon":null,"imageSize":null}
```

- **ลำดับ:** 1
- **ปิดใช้งาน?:** No
- **การมองเห็น:** ALWAYS

