---
type: concept
tags: #data-science #math/regression #status/permanent
---
# 🪐 การถดถอยเชิงเส้น (Linear Regression)

> [!abstract] หัวใจสำคัญ
> Linear Regression หาความสัมพันธ์เชิงเส้นระหว่าง features กับ target — สูตร $y = wx + b$ หา $w$ (slope) และ $b$ (intercept) ที่ทำให้ error น้อยที่สุด เป็นโมเดลพื้นฐานที่สุดของ ML

## 📜 กฎและสูตร (The Laws)

### โมเดล
$$y = w_1 x_1 + w_2 x_2 + \cdots + w_n x_n + b = \mathbf{w}^T \mathbf{x} + b$$

### Loss Function (MSE)
$$\text{MSE} = \frac{1}{n}\sum_{i=1}^n (y_i - \hat{y}_i)^2$$

### Gradient Descent
$$\mathbf{w} \leftarrow \mathbf{w} - \alpha \frac{\partial \text{MSE}}{\partial \mathbf{w}}$$

เมื่อ $\alpha$ = learning rate

### สูตรปิด (Closed Form) สำหรับ Simple Linear Regression
$$w = \frac{\sum (x_i - \bar{x})(y_i - \bar{y})}{\sum (x_i - \bar{x})^2}, \quad b = \bar{y} - w\bar{x}$$

## ⛓️ เส้นใยความสัมพันธ์ (Dependencies)

- **ต้องรู้ก่อน:** [[40-Geometry-Trig/401-Vectors|401-Vectors]], [[40-Geometry-Trig/402-Matrices|402-Matrices]], [[50-Advanced/501-Derivatives|501-Derivatives]]
- **นำไปสู่:** [[70-AI-ML/701-Linear-Regression|701-Linear-Regression]], [[70-AI-ML/702-Neural-Networks|702-Neural-Networks]]

## 💡 วิธีการมอง (Mental Model)

> [!example] เปรียบเทียบ: ลากเส้นตรงให้ใกล้จุดข้อมูลมากที่สุด
> เป้าหมาย = ลดระยะห่างรวมระหว่างเส้นกับจุด (minimize error)

> [!example] ใน Python
> `from sklearn.linear_model import LinearRegression` — โมเดลพื้นฐานที่ใช้บ่อยที่สุด

## 📑 รายการโจทย์ที่เกี่ยวข้อง

- [ ] [[80-Archives/Ex-010-Linear-Regression|Ex-010-Linear-Regression]]
