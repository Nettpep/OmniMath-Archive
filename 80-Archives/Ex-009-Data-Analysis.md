---
type: exercise
difficulty: ⭐⭐⭐
level: Data Science
level_category: advanced
tags: #exercise #level/advanced
status: solved
---
# 📝 บันทึกปริศนา: EDA

## ❓ โจทย์ (The Question)

> [!quote]
> ข้อมูลมี missing values 10% ในคอลัมน์ "อายุ" คุณจะจัดการอย่างไร?

## 🕵️ วิธีคิด (Solution)

> [!question] ทำไมต้องจัดการ missing values?
> โมเดล ML รับข้อมูลตัวเลขได้เท่านั้น — ค่าว่าง (NaN) ทำให้คำนวณไม่ได้ ต้องตัดสินใจว่าจะ "ทิ้ง" หรือ "เติม"

**ทางเลือกและเมื่อไหร่ใช้:**

| วิธี | ใช้เมื่อ |
|------|----------|
| **ลบแถว** | missing น้อย (<5%) และข้อมูลมาก |
| **เติมมัธยฐาน** | missing แบบสุ่ม (MCAR) — มัธยฐานทน outlier กว่าค่าเฉลี่ย |
| **เติมด้วยโมเดล** | มีความสัมพันธ์กับ features อื่น (predict ได้) |
| **"Unknown"** | categorical — เพิ่ม category ใหม่ |

> [!example] 🔥 กรณีนี้ (10% ใน "อายุ")
> ดู distribution ก่อน — ถ้า 1000 แถว และ missing สุ่ม → เติมมัธยฐานอายุได้ | ถ้า missing ไม่สุ่ม (เช่น คนสูงอายุไม่กรอก) → ต้องระวัง bias

## 🧠 ทฤษฎีที่ใช้ (The Links)

- ใช้ความรู้จาก: [[60-Data-Science/601-Data-Analysis|601-Data-Analysis]], [[50-Advanced/503-Statistics|503-Statistics]]
