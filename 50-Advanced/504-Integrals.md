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

## 🛠️ เทคนิคการหาปริพันธ์ (Integration Techniques)

### 1. การแทนค่า (Substitution Rule)
เป็นเทคนิคที่ใช้เปลี่ยนตัวแปรในปริพันธ์ เพื่อให้ปริพันธ์อยู่ในรูปที่ง่ายต่อการหา โดยมีหลักการคือ ถ้า $u = g(x)$ แล้ว $du = g'(x) dx$ ดังนั้น
$$\int f(g(x))g'(x) dx = \int f(u) du$$

> [!example] ตัวอย่าง
> จงหาค่าของ $\int 2x(x^2+1)^3 dx$
> ให้ $u = x^2+1$ ดังนั้น $du = 2x dx$
> จะได้ $\int u^3 du = \frac{u^4}{4} + C = \frac{(x^2+1)^4}{4} + C$

### 2. การหาปริพันธ์ทีละส่วน (Integration by Parts)
ใช้สำหรับปริพันธ์ที่อยู่ในรูปผลคูณของสองฟังก์ชัน โดยมีสูตรคือ
$$\int u \, dv = uv - \int v \, du$$
การเลือก $u$ และ $dv$ เป็นสิ่งสำคัญ โดยทั่วไปจะใช้หลัก LIATE (Logarithmic, Inverse trigonometric, Algebraic, Trigonometric, Exponential) ในการเลือก $u$ ก่อน

> [!example] ตัวอย่าง
> จงหาค่าของ $\int x e^x dx$
> ให้ $u = x$ และ $dv = e^x dx$
> ดังนั้น $du = dx$ และ $v = e^x$
> จะได้ $\int x e^x dx = x e^x - \int e^x dx = x e^x - e^x + C$

## ⛓️ เส้นใยความสัมพันธ์ (Dependencies)

- **ต้องรู้ก่อน:** [[30-Algebra/301-Linear-Equations|301-Linear-Equations]], [[50-Advanced/501-Derivatives|501-Derivatives]]
- **นำไปสู่:** [[60-Data-Science/601-Data-Analysis|601-Data-Analysis]], [[70-AI-ML/705-Deep-Learning|705-Deep-Learning]], [[50-Advanced/502-Probability|502-Probability]] (สำหรับ PDF/CDF)

## 💡 วิธีการมอง (Mental Model)

> [!example] เปรียบเทียบ: การสะสม
> ถ้าอนุพันธ์คือความเร็ว (อัตราการเปลี่ยนแปลงของระยะทาง) ปริพันธ์ก็คือระยะทางที่สะสมจากการเดินทางด้วยความเร็วต่างๆ

> [!example] ใน ML: Probability Density Functions (PDF) และ Cumulative Distribution Functions (CDF)
> ในสถิติและความน่าจะเป็น ฟังก์ชันความหนาแน่นความน่าจะเป็น (PDF) $f(x)$ จะบอกความน่าจะเป็นสัมพัทธ์ที่ตัวแปรสุ่มจะมีค่า $x$ สำหรับตัวแปรสุ่มต่อเนื่อง พื้นที่ใต้กราฟของ PDF ในช่วงหนึ่งๆ คือความน่าจะเป็นที่ตัวแปรสุ่มจะอยู่ในช่วงนั้น ซึ่งคำนวณได้จากการหาปริพันธ์
> $$P(a \le X \le b) = \int_{a}^{b} f(x) dx$$
> ฟังก์ชันการแจกแจงสะสม (CDF) $F(x)$ คือปริพันธ์ของ PDF ซึ่งบอกความน่าจะเป็นที่ตัวแปรสุ่มจะมีค่าน้อยกว่าหรือเท่ากับ $x$
> $$F(x) = P(X \le x) = \int_{-\infty}^{x} f(t) dt$$
> การทำความเข้าใจปริพันธ์จึงเป็นสิ่งสำคัญในการวิเคราะห์และสร้างแบบจำลองทางสถิติและ Machine Learning โดยเฉพาะอย่างยิ่งในเรื่องของ Distribution และ Bayesian Inference

## 📑 รายการโจทย์ที่เกี่ยวข้อง

- [ ] [[80-Archives/Ex-014-Integrals|Ex-014-Integrals]]
- [ ] [[80-Archives/Ex-015-Integrals-Substitution|Ex-015-Integrals-Substitution]]
- [ ] [[80-Archives/Ex-016-Integrals-by-Parts|Ex-016-Integrals-by-Parts]]
