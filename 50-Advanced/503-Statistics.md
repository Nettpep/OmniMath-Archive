---
type: concept
tags: #math/statistics #status/permanent
---
# 🪐 สถิติเชิงพรรณนา (Descriptive Statistics)

> [!abstract] หัวใจสำคัญ
> สถิติเชิงพรรณนาสรุปข้อมูลเป็นตัวเลขที่เข้าใจง่าย — ค่าเฉลี่ย, มัธยฐาน, ความแปรปรวน ใช้ในการวิเคราะห์ข้อมูลก่อนสร้างโมเดล และประเมินผลลัพธ์

## 📜 กฎและสูตร (The Laws)

### ค่ากลาง
$$\bar{x} = \frac{1}{n}\sum_{i=1}^n x_i \quad \text{(ค่าเฉลี่ย)}$$

มัธยฐาน = ค่ากลางเมื่อเรียงข้อมูล

### การกระจาย
$$\text{Variance: } \sigma^2 = \frac{1}{n}\sum_{i=1}^n (x_i - \bar{x})^2$$
$$\text{Standard Deviation: } \sigma = \sqrt{\sigma^2}$$

### Correlation
$$r = \frac{\sum (x_i - \bar{x})(y_i - \bar{y})}{\sqrt{\sum (x_i - \bar{x})^2} \sqrt{\sum (y_i - \bar{y})^2}} \in [-1, 1]$$

## ⛓️ เส้นใยความสัมพันธ์ (Dependencies)

- **ต้องรู้ก่อน:** [[50-Advanced/502-Probability|502-Probability]], [[20-Pre-Algebra/202-Fractions|202-Fractions]]
- **นำไปสู่:** [[60-Data-Science/601-Data-Analysis|601-Data-Analysis]], [[60-Data-Science/602-Linear-Regression|602-Linear-Regression]]

## 💡 วิธีการมอง (Mental Model)

> [!example] เปรียบเทียบ: สรุปคะแนนสอบ
> ค่าเฉลี่ย = ระดับโดยรวม, ความแปรปรวน = ความแตกต่างระหว่างคน

> [!example] ใน Data Science
> ก่อน train โมเดล ต้องดู distribution ของ features — มี outlier ไหม? ต้อง normalize ไหม?

## 📑 รายการโจทย์ที่เกี่ยวข้อง

- [ ] [[80-Archives/Ex-008-Statistics|Ex-008-Statistics]]
