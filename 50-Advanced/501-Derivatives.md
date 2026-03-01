---
type: concept
tags: #math/calculus #status/permanent
---
# 🪐 อนุพันธ์ (Derivatives)

> [!abstract] หัวใจสำคัญ
> อนุพันธ์วัด "อัตราการเปลี่ยนแปลง" ของฟังก์ชัน ณ จุดใดจุดหนึ่ง — ใน ML ใช้คำนวณ gradient สำหรับ Gradient Descent เพื่ออัปเดตน้ำหนักให้ loss ลดลง

## 📜 กฎและสูตร (The Laws)

### นิยาม
$$f'(x) = \lim_{h \to 0} \frac{f(x+h) - f(x)}{h}$$

### กฎพื้นฐาน
$$\frac{d}{dx}(x^n) = nx^{n-1}$$
$$\frac{d}{dx}(cf) = c \cdot f'$$
$$\frac{d}{dx}(f + g) = f' + g'$$

### กฎลูกโซ่ (Chain Rule) — สำคัญมากสำหรับ Backpropagation!
$$\frac{d}{dx}f(g(x)) = f'(g(x)) \cdot g'(x)$$

หรือเขียนเป็น: $\frac{dy}{dx} = \frac{dy}{du} \cdot \frac{du}{dx}$

### อนุพันธ์ของฟังก์ชันสำคัญ
$$\frac{d}{dx}(e^x) = e^x, \quad \frac{d}{dx}(\ln x) = \frac{1}{x}$$

## ⛓️ เส้นใยความสัมพันธ์ (Dependencies)

- **ต้องรู้ก่อน:** [[30-Algebra/301-Linear-Equations|301-Linear-Equations]], [[20-Pre-Algebra/201-Like-Terms|201-Like-Terms]]
- **นำไปสู่:** [[70-AI-ML/701-Linear-Regression|701-Linear-Regression]], [[70-AI-ML/702-Neural-Networks|702-Neural-Networks]]

## 💡 วิธีการมอง (Mental Model)

> [!example] เปรียบเทียบ: ความเร็ว
> อนุพันธ์ของตำแหน่ง = ความเร็ว (อัตราการเปลี่ยนตำแหน่ง)

> [!example] ใน Gradient Descent
> gradient = อนุพันธ์ของ loss เทียบกับ weight — บอกทิศทางที่ loss เพิ่มขึ้น เราเดินไปทางตรงข้ามเพื่อให้ loss ลดลง

## 📑 รายการโจทย์ที่เกี่ยวข้อง

- [ ] [[80-Archives/Ex-006-Derivatives|Ex-006-Derivatives]]
