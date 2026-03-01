---
type: concept
tags: #ai-ml #ml/supervised #status/permanent
---
# 🪐 Linear Regression ใน ML

> [!abstract] หัวใจสำคัญ
> Linear Regression คือโมเดล ML แบบ Supervised ที่ทำนายค่าต่อเนื่อง — ใช้ Gradient Descent หา weights ที่ minimize MSE เป็นจุดเริ่มต้นที่ดีสำหรับเข้าใจ ML pipeline ทั้งหมด

## 📜 กฎและสูตร (The Laws)

### โมเดล
$$\hat{y} = \mathbf{X}\mathbf{w} + b$$

เมื่อ $\mathbf{X}$ = matrix ของ features, $\mathbf{w}$ = weight vector

### Gradient Descent Update
$$w_j \leftarrow w_j - \alpha \frac{\partial}{\partial w_j} \text{MSE}$$

$$\frac{\partial \text{MSE}}{\partial w_j} = -\frac{2}{n}\sum_i (y_i - \hat{y}_i) x_{ij}$$

### Pipeline
1. โหลดข้อมูล → 2. แยก train/test → 3. Normalize → 4. Train → 5. Evaluate (MSE, MAE, R²)

## ⛓️ เส้นใยความสัมพันธ์ (Dependencies)

- **ต้องรู้ก่อน:** [[60-Data-Science/602-Linear-Regression|602-Linear-Regression]], [[50-Advanced/501-Derivatives|501-Derivatives]], [[40-Geometry-Trig/402-Matrices|402-Matrices]]
- **นำไปสู่:** [[70-AI-ML/702-Neural-Networks|702-Neural-Networks]], [[70-AI-ML/703-Classification|703-Classification]]

## 💡 วิธีการมอง (Mental Model)

> [!example] เปรียบเทียบ: การเดินลงเขา
> Gradient = ทิศทางที่สูงขึ้น → เดินตรงข้าม = ลงเขา = ลด loss

> [!example] Hyperparameters
> learning_rate ($\alpha$), num_epochs, batch_size — ต้อง tune

## 📑 รายการโจทย์ที่เกี่ยวข้อง

- [ ] [[80-Archives/Ex-010-Linear-Regression|Ex-010-Linear-Regression]]
