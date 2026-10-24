# Format Rules ของตาราง ทำเบิกส่วนต่างScgวังน้อย

รวม **2 format rules**

## ทำเบิกได้

- **ใช้กับข้อมูล:** `ทำเบิกส่วนต่างScgวังน้อย`
- **รูปแบบที่ใช้กับ:** `ขออนุมัติเบิกค่าขนส่งส่วนเพิ่ม`
**เงื่อนไข:**

```
=[ขออนุมัติเบิกค่าขนส่งส่วนเพิ่ม] >0
```

**รูปแบบที่ใช้ (Like this):**

```json
{"textColor":"green","highlightColor":"green","textSize":1.0,"underline":false,"strikethrough":false,"bold":true,"italic":false,"uppercase":false,"icon":"far fa-sack-dollar","imageSize":null}
```

- **ลำดับ:** 1
- **ปิดใช้งาน?:** No
- **การมองเห็น:** ALWAYS

## ทำเบิกไม่ได้

- **ใช้กับข้อมูล:** `ทำเบิกส่วนต่างScgวังน้อย`
- **รูปแบบที่ใช้กับ:** `ขออนุมัติเบิกค่าขนส่งส่วนเพิ่ม`
**เงื่อนไข:**

```
=[ขออนุมัติเบิกค่าขนส่งส่วนเพิ่ม] < 0
```

**รูปแบบที่ใช้ (Like this):**

```json
{"textColor":"red","highlightColor":"red","textSize":1.0,"underline":false,"strikethrough":true,"bold":false,"italic":false,"uppercase":false,"icon":"far fa-sack-dollar","imageSize":null}
```

- **ลำดับ:** 1
- **ปิดใช้งาน?:** No
- **การมองเห็น:** ALWAYS

