---
type: exercise
difficulty: ⭐⭐⭐
level: Data Science/ML
level_category: advanced
tags: #exercise #level/advanced
status: solved
---
# 📝 บันทึกปริศนา: Linear Regression

## ❓ โจทย์ (The Question)

> [!quote]
> ข้อมูล (x,y): (1,2), (2,4), (3,5) จงหาสมการเส้นตรง $y = wx + b$ ด้วยสูตรปิด

## 🕵️ วิธีคิด (Solution)

> [!info] Linear Regression = หาเส้นตรงที่ "ใกล้จุดข้อมูลที่สุด"
> สูตรปิด: $w = \frac{\sum (x_i-\bar{x})(y_i-\bar{y})}{\sum (x_i-\bar{x})^2}$, $b = \bar{y} - w\bar{x}$

$\bar{x} = 2$, $\bar{y} = 11/3 \approx 3.67$

**หาค่า w (ความชัน):**
$$w = \frac{(1-2)(2-3.67)+(2-2)(4-3.67)+(3-2)(5-3.67)}{(1-2)^2+(2-2)^2+(3-2)^2} = \frac{3}{2} = 1.5$$

**หาค่า b (จุดตัดแกน y):**
$$b = \bar{y} - w\bar{x} = \frac{11}{3} - 3 = \frac{2}{3}$$

**สมการ:** $y = 1.5x + \frac{2}{3}$

> [!example] 🔥 เห็นภาพ
> ลากเส้นตรงให้ใกล้จุด (1,2), (2,4), (3,5) มากที่สุด — w=1.5 = ความชัน, b=2/3 = ตัดแกน y

> [!tip] ใน ML
> Gradient Descent ทำสิ่งเดียวกัน แต่ใช้ iterative แทนสูตรปิด — ใช้ได้กับข้อมูลขนาดใหญ่

## 🧠 ทฤษฎีที่ใช้ (The Links)

- ใช้ความรู้จาก: [[60-Data-Science/602-Linear-Regression|602-Linear-Regression]], [[40-Geometry-Trig/401-Vectors|401-Vectors]]
