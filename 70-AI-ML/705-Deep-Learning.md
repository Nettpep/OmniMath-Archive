---
type: concept
tags: #ai-ml #ml/deep-learning #status/permanent
---
# 🪐 Deep Learning

> [!abstract] หัวใจสำคัญ
> Deep Learning คือ Neural Networks ที่มีหลาย layer — สามารถเรียนรู้ hierarchical features จากข้อมูลดิบ ใช้ใน Computer Vision, NLP, Speech และงานที่ซับซ้อน

## 📜 กฎและสูตร (The Laws)

### โครงสร้าง
- **Input Layer** → **Hidden Layers** (หลายชั้น) → **Output Layer**
- แต่ละ layer: $\mathbf{a} = \sigma(\mathbf{W}\mathbf{x} + \mathbf{b})$

### เทคนิคสำคัญ
- **Dropout** — ปิด neuron แบบสุ่ม ป้องกัน overfitting
- **Batch Normalization** — normalize activation
- **Optimizers** — Adam, SGD, RMSprop

### สถาปัตยกรรม
- **CNN** — สำหรับรูปภาพ (Convolutional layers)
- **RNN/LSTM** — สำหรับลำดับ (ข้อความ, เวลา)
- **Transformer** — สำหรับ NLP (BERT, GPT)

## ⛓️ เส้นใยความสัมพันธ์ (Dependencies)

- **ต้องรู้ก่อน:** [[70-AI-ML/702-Neural-Networks|702-Neural-Networks]], [[40-Geometry-Trig/402-Matrices|402-Matrices]]
- **นำไปสู่:** [[70-AI-ML/706-AI-Building|706-AI-Building]], การสร้าง AI จริง

## 💡 วิธีการมอง (Mental Model)

> [!example] เปรียบเทียบ: โรงงานแปรรูป
> Raw data → Layer 1 (แยกส่วนเล็ก) → Layer 2 (รวมเป็นส่วนกลาง) → ... → Output (คำตอบสุดท้าย)

> [!example] ทำไม "Deep"?
> หลาย layer = หลายระดับ abstraction = เรียนรู้ pattern ที่ซับซ้อนได้

## 📑 รายการโจทย์ที่เกี่ยวข้อง

- [ ] [[80-Archives/Ex-012-Neural-Network|Ex-012-Neural-Network]]
