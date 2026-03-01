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

## 🕵️ วิธีการพิชิต (Solution)

$\bar{x} = 2$, $\bar{y} = 11/3 \approx 3.67$

$$w = \frac{\sum (x_i-\bar{x})(y_i-\bar{y})}{\sum (x_i-\bar{x})^2} = \frac{(1-2)(2-3.67)+(2-2)(4-3.67)+(3-2)(5-3.67)}{(1-2)^2+(2-2)^2+(3-2)^2}$$
$$= \frac{1.67 + 0 + 1.33}{2} = \frac{3}{2} = 1.5$$

$$b = \bar{y} - w\bar{x} = \frac{11}{3} - 1.5(2) = \frac{11}{3} - 3 = \frac{2}{3}$$

**สมการ:** $y = 1.5x + \frac{2}{3}$

## 🧠 ทฤษฎีที่ใช้ (The Links)

- ใช้ความรู้จาก: [[60-Data-Science/602-Linear-Regression|602-Linear-Regression]], [[40-Geometry-Trig/401-Vectors|401-Vectors]]
