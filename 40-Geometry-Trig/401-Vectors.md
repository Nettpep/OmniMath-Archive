---
type: concept
tags: #math/linear-algebra #math/geometry #status/permanent
---
# 🪐 เวกเตอร์ (Vectors)

> [!abstract] หัวใจสำคัญ
> เวกเตอร์คือปริมาณที่มีทั้งขนาดและทิศทาง — ใน AI/ML ใช้แทนข้อมูล (เช่น features ของแต่ละ sample) และน้ำหนักของโมเดล การบวกเวกเตอร์และการคูณด้วยสเกลาร์เป็นพื้นฐานของพีชคณิตเชิงเส้น

## 📜 กฎและสูตร (The Laws)

### นิยาม
$$\vec{v} = \begin{pmatrix} v_1 \\ v_2 \\ \vdots \\ v_n \end{pmatrix} \quad \text{หรือ} \quad \vec{v} = (v_1, v_2, \ldots, v_n)$$

### การบวกและคูณด้วยสเกลาร์
$$\vec{u} + \vec{v} = (u_1+v_1, u_2+v_2, \ldots, u_n+v_n)$$
$$c \cdot \vec{v} = (cv_1, cv_2, \ldots, cv_n)$$

### ขนาด (Magnitude)
$$|\vec{v}| = \sqrt{v_1^2 + v_2^2 + \cdots + v_n^2}$$

### Dot Product (ผลคูณภายใน)
$$\vec{u} \cdot \vec{v} = u_1 v_1 + u_2 v_2 + \cdots + u_n v_n = |\vec{u}||\vec{v}|\cos\theta$$

## ⛓️ เส้นใยความสัมพันธ์ (Dependencies)

- **ต้องรู้ก่อน:** [[30-Algebra/301-Linear-Equations|301-Linear-Equations]], [[20-Pre-Algebra/201-Like-Terms|201-Like-Terms]]
- **นำไปสู่:** [[40-Geometry-Trig/402-Matrices|402-Matrices]], [[70-AI-ML/701-Linear-Regression|701-Linear-Regression]]

## 💡 วิธีการมอง (Mental Model)

> [!example] เปรียบเทียบ: ลูกศร
> เวกเตอร์ = ลูกศรที่ชี้จากจุดหนึ่งไปอีกจุด — ความยาวคือขนาด ทิศทางคือทิศทาง การบวกเวกเตอร์ = ต่อลูกศรหัวต่อหาง

> [!example] ใน Machine Learning
> ข้อมูล 1 แถว = เวกเตอร์ 1 ตัว (เช่น [อายุ, รายได้, จำนวนบุตร])

## 📑 รายการโจทย์ที่เกี่ยวข้อง

- [ ] [[80-Archives/Ex-004-Vectors|Ex-004-Vectors]]
