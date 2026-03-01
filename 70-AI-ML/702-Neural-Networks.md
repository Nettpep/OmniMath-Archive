---
type: concept
tags: #ai-ml #ml/deep-learning #status/permanent
---
# 🪐 Neural Networks (โครงข่ายประสาทเทียม)

> [!abstract] หัวใจสำคัญ
> Neural Network คือโมเดลที่ประกอบด้วย layers ของ neurons — แต่ละ neuron คำนวณ weighted sum แล้วผ่าน activation function Forward pass คำนวณ output, Backpropagation คำนวณ gradient เพื่ออัปเดต weights

## 📜 กฎและสูตร (The Laws)

### โครงสร้าง
$$\text{Layer } l: \quad \mathbf{a}^{(l)} = \sigma(\mathbf{W}^{(l)} \mathbf{a}^{(l-1)} + \mathbf{b}^{(l)})$$

เมื่อ $\sigma$ = activation function (ReLU, Sigmoid, Softmax)

### Activation Functions
- **ReLU:** $\sigma(x) = \max(0, x)$
- **Sigmoid:** $\sigma(x) = \frac{1}{1+e^{-x}}$
- **Softmax:** สำหรับ output หลาย class

### Backpropagation
ใช้ [[50-Advanced/501-Derivatives|Chain Rule]] คำนวณ $\frac{\partial L}{\partial w}$ สำหรับทุก weight

### Loss Functions
- Regression: MSE
- Classification: Cross-Entropy

## ⛓️ เส้นใยความสัมพันธ์ (Dependencies)

- **ต้องรู้ก่อน:** [[40-Geometry-Trig/402-Matrices|402-Matrices]], [[50-Advanced/501-Derivatives|501-Derivatives]], [[70-AI-ML/701-Linear-Regression|701-Linear-Regression]]
- **นำไปสู่:** [[70-AI-ML/705-Deep-Learning|705-Deep-Learning]], การสร้าง AI จริง

## 💡 วิธีการมอง (Mental Model)

> [!example] เปรียบเทียบ: สมองจำลอง
> Input → Layer 1 (feature extraction) → Layer 2 → ... → Output (คำตอบ)

> [!example] ทำไมต้องหลาย Layer?
> Layer แรกจับ pattern พื้นฐาน (ขอบ, สี) → Layer ถัดไปจับ pattern ซับซ้อน (ตา, จมูก) → Layer สุดท้ายจับ concept (ใบหน้า)

## 📑 รายการโจทย์ที่เกี่ยวข้อง

- [ ] [[80-Archives/Ex-012-Neural-Network|Ex-012-Neural-Network]]
