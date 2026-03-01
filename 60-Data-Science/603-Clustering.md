---
type: concept
tags: #data-science #ml/unsupervised #status/permanent
---
# 🪐 การจัดกลุ่ม (Clustering)

> [!abstract] หัวใจสำคัญ
> Clustering คือการจัดกลุ่มข้อมูลที่ไม่มี label — ข้อมูลที่คล้ายกันอยู่กลุ่มเดียวกัน ใช้สำหรับการค้นพบ pattern, การแบ่ง segment ลูกค้า หรือการลดมิติข้อมูล

## 📜 กฎและสูตร (The Laws)

### K-Means Algorithm
1. เลือก K จุดเป็น centroids เริ่มต้น
2. แบ่งแต่ละจุดไปกลุ่มที่ centroid ใกล้ที่สุด
3. อัปเดต centroid = ค่าเฉลี่ยของจุดในกลุ่ม
4. ทำซ้ำจน centroid ไม่เปลี่ยน

### ระยะทาง (Distance)
$$d(\mathbf{x}, \mathbf{c}) = \sqrt{\sum_j (x_j - c_j)^2} \quad \text{(Euclidean)}$$

### Elbow Method
พล็อต inertia vs K — เลือก K ที่ "ข้อศอก" ของกราฟ

## ⛓️ เส้นใยความสัมพันธ์ (Dependencies)

- **ต้องรู้ก่อน:** [[40-Geometry-Trig/401-Vectors|401-Vectors]], [[60-Data-Science/601-Data-Analysis|601-Data-Analysis]]
- **นำไปสู่:** [[70-AI-ML/704-Unsupervised-Learning|704-Unsupervised-Learning]], การลดมิติ (PCA)

## 💡 วิธีการมอง (Mental Model)

> [!example] เปรียบเทียบ: จัดกลุ่มลูกค้าตามพฤติกรรม
> ลูกค้าที่ซื้อของคล้ายกัน → กลุ่มเดียวกัน → โฆษณาแบบเดียวกัน

> [!example] Unsupervised vs Supervised
> ไม่มีคำตอบถูกต้อง — โมเดลค้นหา pattern เอง

## 📑 รายการโจทย์ที่เกี่ยวข้อง

- [ ] [[80-Archives/Ex-011-Clustering|Ex-011-Clustering]]
