---
type: concept
tags: #ai-ml #ml/unsupervised #status/permanent
---
# 🪐 การเรียนรู้แบบไม่มีผู้สอน (Unsupervised Learning)

> [!abstract] หัวใจสำคัญ
> Unsupervised Learning ทำงานกับข้อมูลที่ไม่มี label — โมเดลค้นหา pattern, โครงสร้าง หรือการลดมิติด้วยตัวเอง ใช้ใน Clustering, Dimensionality Reduction (PCA), Anomaly Detection

## 📜 กฎและสูตร (The Laws)

### งานหลัก
1. **Clustering** — จัดกลุ่มข้อมูลที่คล้ายกัน ([[60-Data-Science/603-Clustering|603-Clustering]])
2. **Dimensionality Reduction** — ลดจำนวน features (PCA)
3. **Anomaly Detection** — หาจุดที่ผิดปกติ

### PCA (Principal Component Analysis)
หา directions ที่ variance สูงสุด — ลดมิติโดยคงข้อมูลสำคัญ

### Autoencoders (Neural)
Encode → compressed representation → Decode → reconstruct input

## ⛓️ เส้นใยความสัมพันธ์ (Dependencies)

- **ต้องรู้ก่อน:** [[60-Data-Science/603-Clustering|603-Clustering]], [[40-Geometry-Trig/402-Matrices|402-Matrices]]
- **นำไปสู่:** [[70-AI-ML/706-AI-Building|706-AI-Building]], Recommendation systems

## 💡 วิธีการมอง (Mental Model)

> [!example] เปรียบเทียบ: จัดเอกสารโดยไม่มีป้ายชื่อ
> ดูว่าเอกสารไหนคล้ายกัน → ใส่โฟลเดอร์เดียวกัน

> [!example] ใช้เมื่อไร?
> เมื่อไม่มี label, ต้องการค้นพบ pattern, หรือลดมิติข้อมูล

## 📑 รายการโจทย์ที่เกี่ยวข้อง

- [ ] [[80-Archives/Ex-011-Clustering|Ex-011-Clustering]]
