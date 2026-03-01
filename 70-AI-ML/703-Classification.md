---
type: concept
tags: #ai-ml #ml/supervised #status/permanent
---
# 🪐 การจำแนกประเภท (Classification)

> [!abstract] หัวใจสำคัญ
> Classification คือการทำนาย "หมวดหมู่" (เช่น สุนัข/แมว, spam/ไม่ spam) — ต่างจาก Regression ที่ทำนายค่าต่อเนื่อง ใช้ Logistic Regression, Decision Tree หรือ Neural Network

## 📜 กฎและสูตร (The Laws)

### Logistic Regression
$$P(y=1|\mathbf{x}) = \sigma(\mathbf{w}^T \mathbf{x} + b) = \frac{1}{1 + e^{-(\mathbf{w}^T \mathbf{x} + b)}}$$

### Cross-Entropy Loss
$$L = -\sum_i \left[ y_i \log(\hat{y}_i) + (1-y_i) \log(1-\hat{y}_i) \right]$$

### Metrics
- **Accuracy:** $\frac{\text{ถูกต้อง}}{\text{ทั้งหมด}}$
- **Precision, Recall, F1-score** — สำหรับ imbalanced data
- **Confusion Matrix** — TP, TN, FP, FN

## ⛓️ เส้นใยความสัมพันธ์ (Dependencies)

- **ต้องรู้ก่อน:** [[70-AI-ML/701-Linear-Regression|701-Linear-Regression]], [[50-Advanced/502-Probability|502-Probability]]
- **นำไปสู่:** [[70-AI-ML/702-Neural-Networks|702-Neural-Networks]], [[70-AI-ML/706-AI-Building|706-AI-Building]]

## 💡 วิธีการมอง (Mental Model)

> [!example] เปรียบเทียบ: แยกอีเมล
> Input = ข้อความ → โมเดลให้ความน่าจะเป็น spam → ถ้า > 0.5 = spam

> [!example] Multi-class
> Softmax แปลง output เป็นความน่าจะเป็นของแต่ละ class (รวม = 1)

## 📑 รายการโจทย์ที่เกี่ยวข้อง

- [ ] [[80-Archives/Ex-013-Classification|Ex-013-Classification]]
