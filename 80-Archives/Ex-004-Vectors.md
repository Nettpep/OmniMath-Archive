---
type: exercise
difficulty: ⭐⭐
level: ม.4-5
level_category: highschool
tags: #exercise #level/highschool
status: solved
---
# 📝 บันทึกปริศนา: การคำนวณเวกเตอร์

## ❓ โจทย์ (The Question)

> [!quote]
> ให้ $\vec{u} = (3, -2)$ และ $\vec{v} = (1, 4)$ จงหา $\vec{u} + \vec{v}$, $2\vec{u}$, และ $\vec{u} \cdot \vec{v}$

## 🕵️ วิธีคิด (Solution)

### บวกเวกเตอร์
> [!info] บวกเวกเตอร์ = บวกทีละองค์ประกอบ
> เวกเตอร์ = ลูกศรที่มีองค์ประกอบ (x, y) — บวกกัน = เอา x กับ x, y กับ y มารวม

$$\vec{u} + \vec{v} = (3+1, -2+4) = (4, 2)$$

### คูณด้วยสเกลาร์
> [!info] คูณสเกลาร์ = คูณทุกองค์ประกอบ
> $2\vec{u}$ = ยืดเวกเตอร์ 2 เท่า

$$2\vec{u} = (2 \times 3, 2 \times (-2)) = (6, -4)$$

### Dot Product (ผลคูณภายใน)
> [!question] Dot product คิดยังไง?
> คูณองค์ประกอบที่ตรงกันแล้วบวก — ได้**ตัวเลข** (scalar) ไม่ใช่เวกเตอร์!

$$\vec{u} \cdot \vec{v} = 3(1) + (-2)(4) = 3 - 8 = -5$$

> [!example] 🔥 ใน Machine Learning
> เวกเตอร์ = features ของ 1 sample — dot product กับ weight vector = คะแนน/การทำนาย

## 🧠 ทฤษฎีที่ใช้ (The Links)

- ใช้ความรู้จาก: [[40-Geometry-Trig/401-Vectors|401-Vectors]], [[10-Foundations/101-Rule-of-Signs|101-Rule-of-Signs]]

## ⚠️ บทเรียนที่ได้รับ (Lessons)

- [x] Dot product ได้ scalar ไม่ใช่ vector
