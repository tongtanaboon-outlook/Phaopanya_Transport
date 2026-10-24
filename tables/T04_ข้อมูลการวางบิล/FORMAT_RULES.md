# Format Rules ของตาราง ข้อมูลการวางบิล

รวม **4 format rules**

## อนุมัติ

- **ใช้กับข้อมูล:** `ข้อมูลการวางบิล`
- **รูปแบบที่ใช้กับ:** `ราคา`, `สถานะการอนุมัติ`
**เงื่อนไข:**

```
=[สถานะการอนุมัติ] = "อนุมัติ"
```

**รูปแบบที่ใช้ (Like this):**

```json
{"textColor":"green","highlightColor":"green","textSize":1.1,"underline":false,"strikethrough":false,"bold":true,"italic":false,"uppercase":false,"icon":"fal fa-check","imageSize":null}
```

- **ลำดับ:** 1
- **ปิดใช้งาน?:** No
- **การมองเห็น:** ALWAYS

## รอการอนุมัติ

- **ใช้กับข้อมูล:** `ข้อมูลการวางบิล`
- **รูปแบบที่ใช้กับ:** `ราคา`, `สถานะการอนุมัติ`
**เงื่อนไข:**

```
=[สถานะการอนุมัติ] = "รอการอนุมัติ"
```

**รูปแบบที่ใช้ (Like this):**

```json
{"textColor":"orange","highlightColor":"orange","textSize":1.1,"underline":false,"strikethrough":false,"bold":true,"italic":false,"uppercase":false,"icon":"far fa-alarm-clock","imageSize":null}
```

- **ลำดับ:** 1
- **ปิดใช้งาน?:** No
- **การมองเห็น:** ALWAYS

## แจ้งเตือนราคาหลังวิ่งงาน

- **ใช้กับข้อมูล:** `ข้อมูลการวางบิล`
- **รูปแบบที่ใช้กับ:** `ราคาในระบบหลังส่งสินค้า`
**เงื่อนไข:**

```
=AND( [ราคาในระบบหลังส่งสินค้า] <> [ราคา], OR( [ชื่องาน] = "นครหลวง", [ชื่องาน] = "โอนคลัง พว", [ชื่องาน] = "โอนคลัง นำ วิวัฒน์", [ชื่องาน] = "โอนคลัง ซอยฮะ (โกเรีย)", [ชื่องาน] = "โอน คลัง TRW", [ชื่องาน] = "โอนคลัง NocNoc", [ชื่องาน] = "โอนคลังCPF FOOD", [ชื่องาน] = "โอนคลัง BYD", [ชื่องาน] = "ภูมิภาค" ) )
```

**รูปแบบที่ใช้ (Like this):**

```json
{"textColor":"red","highlightColor":"red","textSize":1.0,"underline":false,"strikethrough":false,"bold":true,"italic":false,"uppercase":false,"icon":null,"imageSize":null}
```

- **ลำดับ:** 1
- **ปิดใช้งาน?:** No
- **การมองเห็น:** ALWAYS

## แจ้งเตือนเช็คราคาแล้วปกติ

- **ใช้กับข้อมูล:** `ข้อมูลการวางบิล`
- **รูปแบบที่ใช้กับ:** `ราคาในระบบหลังส่งสินค้า`
**เงื่อนไข:**

```
=IF([ราคาในระบบหลังส่งสินค้า] = [ราคา], TRUE, FALSE)
```

**รูปแบบที่ใช้ (Like this):**

```json
{"textColor":"green","highlightColor":"green","textSize":1.2,"underline":false,"strikethrough":false,"bold":true,"italic":false,"uppercase":false,"icon":null,"imageSize":null}
```

- **ลำดับ:** 1
- **ปิดใช้งาน?:** No
- **การมองเห็น:** ALWAYS

