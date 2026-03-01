---
type: exercise
difficulty: ⭐⭐⭐⭐
level: AI/ML
level_category: advanced
tags: #exercise #level/advanced
status: solved
---
# 📝 บันทึกปริศนา: Neural Network Forward Pass

## ❓ โจทย์ (The Question)

> [!quote]
> Layer 1: input (1, 2), weights [[0.5, 0.3], [0.2, 0.4]], bias (0.1, 0.2) ใช้ ReLU จงหาออกของ Layer 1

## 🕵️ วิธีคิด (Solution)

> [!info] Forward Pass = input → weighted sum → activation → output
> แต่ละ layer: $\mathbf{z} = \mathbf{Wx} + \mathbf{b}$ แล้ว $\mathbf{a} = \sigma(\mathbf{z})$

**ขั้นที่ 1: Weighted sum + bias**
$$\mathbf{z} = \mathbf{Wx} + \mathbf{b} = \begin{pmatrix} 0.5(1)+0.3(2)+0.1 \\ 0.2(1)+0.4(2)+0.2 \end{pmatrix} = \begin{pmatrix} 1.2 \\ 1.2 \end{pmatrix}$$

**ขั้นที่ 2: ReLU activation**
$$\text{ReLU}(x) = \max(0, x) \quad \Rightarrow \quad \mathbf{a} = \begin{pmatrix} 1.2 \\ 1.2 \end{pmatrix}$$

(1.2 > 0 ทั้งคู่ จึงไม่เปลี่ยน)

> [!example] 🔥 เห็นภาพ
> input (1,2) → คูณกับ weights (เหมือน dot product) → บวก bias → ผ่าน ReLU (ตัดค่าติดลบ) → ได้ output ของ layer นี้

## 🧠 ทฤษฎีที่ใช้ (The Links)

- ใช้ความรู้จาก: [[70-AI-ML/702-Neural-Networks|702-Neural-Networks]], [[40-Geometry-Trig/402-Matrices|402-Matrices]]
