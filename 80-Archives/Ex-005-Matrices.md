---
type: exercise
difficulty: ⭐⭐⭐
level: ม.5-6
level_category: highschool
tags: #exercise #level/highschool
status: solved
---
# 📝 บันทึกปริศนา: การคูณเมทริกซ์

## ❓ โจทย์ (The Question)

> [!quote]
> จงหา $AB$ เมื่อ $A = \begin{pmatrix} 1 & 2 \\ 3 & 4 \end{pmatrix}$ และ $B = \begin{pmatrix} 5 & 6 \\ 7 & 8 \end{pmatrix}$

## 🕵️ วิธีคิด (Solution)

> [!info] การคูณเมทริกซ์: แถว · คอลัมน์
> Cell $(i,j)$ ของผลลัพธ์ = **แถวที่ i ของ A** · **คอลัมน์ที่ j ของ B** (dot product)

$$AB = \begin{pmatrix} 1(5)+2(7) & 1(6)+2(8) \\ 3(5)+4(7) & 3(6)+4(8) \end{pmatrix} = \begin{pmatrix} 19 & 22 \\ 43 & 50 \end{pmatrix}$$

> [!example] 🔥 เห็นภาพ
> - มุมบนซ้าย (1,1): แถว 1 ของ A [1,2] · คอลัมน์ 1 ของ B [5,7] = 5+14 = 19
> - มุมบนขวา (1,2): [1,2] · [6,8] = 6+16 = 22
> - ฯลฯ

> [!tip] ใน Neural Network
> $Y = XW$ — input X คูณ weight W = output แต่ละ layer

## 🧠 ทฤษฎีที่ใช้ (The Links)

- ใช้ความรู้จาก: [[40-Geometry-Trig/402-Matrices|402-Matrices]], [[40-Geometry-Trig/401-Vectors|401-Vectors]]

## ⚠️ บทเรียนที่ได้รับ (Lessons)

- [x] แถวของ A · คอลัมน์ของ B = 1 cell ของผลลัพธ์
