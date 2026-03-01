---
type: concept
tags: #math/linear-algebra #status/permanent
---
# 🪐 เมทริกซ์ (Matrices)

> [!abstract] หัวใจสำคัญ
> เมทริกซ์คือตารางตัวเลขขนาด m×n — ใน AI/ML ใช้เก็บชุดข้อมูล (แถว = sample, คอลัมน์ = feature) และน้ำหนักของ Neural Network การคูณเมทริกซ์คือหัวใจของ forward propagation

## 📜 กฎและสูตร (The Laws)

### นิยาม
$$A_{m \times n} = \begin{pmatrix} a_{11} & \cdots & a_{1n} \\ \vdots & \ddots & \vdots \\ a_{m1} & \cdots & a_{mn} \end{pmatrix}$$

### การคูณเมทริกซ์
$(AB)_{ij}$ = แถวที่ $i$ ของ $A$ · คอลัมน์ที่ $j$ ของ $B$

$$(AB)_{ij} = \sum_k A_{ik} B_{kj}$$

**เงื่อนไข:** จำนวนคอลัมน์ของ $A$ = จำนวนแถวของ $B$

### การ Transpose
$$(A^T)_{ij} = A_{ji}$$

## ⛓️ เส้นใยความสัมพันธ์ (Dependencies)

- **ต้องรู้ก่อน:** [[40-Geometry-Trig/401-Vectors|401-Vectors]], [[30-Algebra/301-Linear-Equations|301-Linear-Equations]]
- **นำไปสู่:** [[70-AI-ML/702-Neural-Networks|702-Neural-Networks]], [[60-Data-Science/602-Linear-Regression|602-Linear-Regression]]

## 💡 วิธีการมอง (Mental Model)

> [!example] เปรียบเทียบ: ตาราง Excel
> แถว = 1 บรรทัดข้อมูล (1 sample), คอลัมน์ = 1 คุณสมบัติ (1 feature)

> [!example] ใน Neural Network
> $Y = XW + b$ — $X$ = input, $W$ = weight matrix, $Y$ = output

## 📑 รายการโจทย์ที่เกี่ยวข้อง

- [ ] [[80-Archives/Ex-005-Matrices|Ex-005-Matrices]]
