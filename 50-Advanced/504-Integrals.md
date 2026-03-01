---
type: concept
tags: #math/calculus #status/permanent
---
# 🪐 ปริพันธ์ (Integrals)

> [!abstract] หัวใจสำคัญ
> ปริพันธ์คือการหาพื้นที่ใต้กราฟ หรือการรวมค่าของฟังก์ชันในช่วงหนึ่งๆ ซึ่งเป็นกระบวนการย้อนกลับของอนุพันธ์ (Antiderivative) — ใน ML ใช้ในการหาค่าเฉลี่ย, ความน่าจะเป็นสะสม, และการคำนวณ Loss function ที่ซับซ้อน

## 📜 กฎและสูตร (The Laws)

### นิยาม (ปริพันธ์ไม่จำกัดเขต)
$$\int f(x) dx = F(x) + C \quad \text{เมื่อ } F'(x) = f(x)$$

### นิยาม (ปริพันธ์จำกัดเขต)
$$\int_{a}^{b} f(x) dx = F(b) - F(a)$$

### ทฤษฎีบทหลักมูลของแคลคูลัส (Fundamental Theorem of Calculus)
$$\frac{d}{dx} \int_{a}^{x} f(t) dt = f(x)$$

### กฎพื้นฐาน
$$\int x^n dx = \frac{x^{n+1}}{n+1} + C \quad (n \neq -1)$$
$$\int c \cdot f(x) dx = c \int f(x) dx$$
$$\int (f(x) + g(x)) dx = \int f(x) dx + \int g(x) dx$$

### ปริพันธ์ของฟังก์ชันสำคัญ
$$\int e^x dx = e^x + C, \quad \int \frac{1}{x} dx = \ln|x| + C$$

## ⛓️ เส้นใยความสัมพันธ์ (Dependencies)

- **ต้องรู้ก่อน:** [[30-Algebra/301-Linear-Equations|301-Linear-Equations]], [[50-Advanced/501-Derivatives|501-Derivatives]]
- **นำไปสู่:** [[60-Data-Science/601-Data-Analysis|601-Data-Analysis]], [[70-AI-ML/705-Deep-Learning|705-Deep-Learning]]

## 💡 วิธีการมอง (Mental Model)

> [!example] เปรียบเทียบ: การสะสม
> ถ้าอนุพันธ์คือความเร็ว (อัตราการเปลี่ยนแปลงของระยะทาง) ปริพันธ์ก็คือระยะทางที่สะสมจากการเดินทางด้วยความเร็วต่างๆ

> [!example] ใน ML
> ใช้ในการคำนวณพื้นที่ใต้กราฟของฟังก์ชันความหนาแน่นความน่าจะเป็น (PDF) เพื่อหาความน่าจะเป็นสะสม (CDF) หรือใช้ในการหาค่าเฉลี่ยของฟังก์ชันต่อเนื่อง

## 📑 รายการโจทย์ที่เกี่ยวข้อง

- [ ] [[80-Archives/Ex-014-Integrals|Ex-014-Integrals]]
