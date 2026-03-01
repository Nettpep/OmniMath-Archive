---
type: concept
tags: #math/statistics #math/probability #status/permanent
---
# 🪐 ความน่าจะเป็น (Probability)

> [!abstract] หัวใจสำคัญ
> ความน่าจะเป็นวัด "โอกาส" ที่เหตุการณ์จะเกิดขึ้น (ค่าระหว่าง 0 ถึง 1) — ใน ML ใช้ใน Loss functions (เช่น Cross-Entropy), Bayesian methods, และการประเมินโมเดล

## 📜 กฎและสูตร (The Laws)

### สัจพจน์พื้นฐาน
$$0 \leq P(A) \leq 1, \quad P(\text{ทั้งหมด}) = 1$$

### กฎการบวก
$$P(A \cup B) = P(A) + P(B) - P(A \cap B)$$

เมื่อ $A$ และ $B$ ไม่เกิดร่วมกัน: $P(A \cup B) = P(A) + P(B)$

### ความน่าจะเป็นแบบมีเงื่อนไข
$$P(A|B) = \frac{P(A \cap B)}{P(B)}$$

### Bayes' Theorem
$$P(A|B) = \frac{P(B|A) \cdot P(A)}{P(B)}$$

### การแจกแจงที่สำคัญ
- **Normal:** $\mathcal{N}(\mu, \sigma^2)$
- **Bernoulli:** การทดลอง 1 ครั้ง (สำเร็จ/ล้มเหลว)

## ⛓️ เส้นใยความสัมพันธ์ (Dependencies)

- **ต้องรู้ก่อน:** [[20-Pre-Algebra/202-Fractions|202-Fractions]], [[10-Foundations/102-Number-Systems|102-Number-Systems]]
- **นำไปสู่:** [[50-Advanced/503-Statistics|503-Statistics]], [[70-AI-ML/703-Classification|703-Classification]]

## 💡 วิธีการมอง (Mental Model)

> [!example] เปรียบเทียบ: สถิติการเกิด
> $P(ฝนตก) = 0.3$ = จาก 100 วัน คาดว่าฝนตก 30 วัน

> [!example] ใน ML
> โมเดล classification ให้ความน่าจะเป็นของแต่ละ class — เลือก class ที่มีความน่าจะเป็นสูงสุด

## 📑 รายการโจทย์ที่เกี่ยวข้อง

- [ ] [[80-Archives/Ex-007-Probability|Ex-007-Probability]]
