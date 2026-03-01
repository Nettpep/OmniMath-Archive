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

## 🕵️ วิธีการพิชิต (Solution)

$$\mathbf{z} = \mathbf{Wx} + \mathbf{b} = \begin{pmatrix} 0.5(1)+0.3(2)+0.1 \\ 0.2(1)+0.4(2)+0.2 \end{pmatrix} = \begin{pmatrix} 1.2 \\ 1.2 \end{pmatrix}$$

$$\mathbf{a} = \text{ReLU}(\mathbf{z}) = \begin{pmatrix} \max(0, 1.2) \\ \max(0, 1.2) \end{pmatrix} = \begin{pmatrix} 1.2 \\ 1.2 \end{pmatrix}$$

## 🧠 ทฤษฎีที่ใช้ (The Links)

- ใช้ความรู้จาก: [[70-AI-ML/702-Neural-Networks|702-Neural-Networks]], [[40-Geometry-Trig/402-Matrices|402-Matrices]]
