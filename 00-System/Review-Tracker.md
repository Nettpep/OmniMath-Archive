---
type: index
tags: #review #system
---
# 📊 ระบบทบทวน (Review Tracker)

> [!abstract] หัวใจสำคัญ
> ใช้หน้านี้เป็นศูนย์กลางสำหรับวางแผนและติดตามการทบทวน — ความจำคงทนเมื่อทบทวนแบบ Spaced Repetition (เว้นช่วง)

## 📅 คู่มือ Spaced Repetition

| ครั้งที่ทบทวน | เวลาถัดไปที่ควรทบทวน |
|---------------|------------------------|
| ครั้งที่ 1 | 1 วัน |
| ครั้งที่ 2 | 3 วัน |
| ครั้งที่ 3 | 1 สัปดาห์ |
| ครั้งที่ 4 | 2 สัปดาห์ |
| ครั้งที่ 5+ | 1 เดือน |

> [!tip] เคล็ดลับ
> ถ้าจำไม่ได้ → เริ่มนับใหม่จาก "ครั้งที่ 1"
> ถ้าจำได้ง่ายมาก → ข้ามไปช่วงถัดไปได้

## 📚 โน้ตทั้งหมดที่ควรทบทวน

### ทฤษฎี (Concepts)
- [ ] [[10-Foundations/101-Rule-of-Signs]] — กฎเครื่องหมาย
- [ ] [[10-Foundations/102-Number-Systems]] — ระบบจำนวน
- [ ] [[20-Pre-Algebra/201-Like-Terms]] — พจน์ที่คล้ายกัน
- [ ] [[20-Pre-Algebra/202-Fractions]] — เศษส่วน
- [ ] [[30-Algebra/301-Linear-Equations]] — สมการเชิงเส้น
- [ ] [[30-Algebra/302-Inequalities]] — อสมการเชิงเส้น
- [ ] [[40-Geometry-Trig/401-Vectors]] — เวกเตอร์
- [ ] [[40-Geometry-Trig/402-Matrices]] — เมทริกซ์
- [ ] [[50-Advanced/501-Derivatives]] — อนุพันธ์
- [ ] [[50-Advanced/502-Probability]] — ความน่าจะเป็น
- [ ] [[50-Advanced/503-Statistics]] — สถิติ
- [ ] [[60-Data-Science/601-Data-Analysis]] — การวิเคราะห์ข้อมูล
- [ ] [[60-Data-Science/602-Linear-Regression]] — การถดถอยเชิงเส้น
- [ ] [[60-Data-Science/603-Clustering]] — การจัดกลุ่ม
- [ ] [[70-AI-ML/701-Linear-Regression]] — Linear Regression ใน ML
- [ ] [[70-AI-ML/702-Neural-Networks]] — Neural Networks
- [ ] [[70-AI-ML/703-Classification]] — การจำแนกประเภท
- [ ] [[70-AI-ML/704-Unsupervised-Learning]] — Unsupervised Learning
- [ ] [[70-AI-ML/705-Deep-Learning]] — Deep Learning
- [ ] [[70-AI-ML/706-AI-Building]] — การสร้าง AI

### โจทย์ (Exercises)
- [ ] [[80-Archives/Ex-001-Basic-Algebra]] ถึง [[80-Archives/Ex-013-Classification]]

## 🔗 ลิงก์ไปยัง Daily Review

- [[00-System/Daily-Review-Template|เทมเพลตทบทวนประจำวัน]] — คัดลอกไปใช้แต่ละวัน

## 📌 สำหรับผู้ใช้ Dataview

ถ้าติดตั้ง [Dataview](https://blacksmithgu.github.io/obsidian-dataview/) แล้ว สามารถเพิ่ม YAML `last_reviewed` และ `next_review` ในโน้ต แล้วใช้ query ด้านล่าง:

````markdown
```dataview
TABLE next_review as "ทบทวนครั้งถัดไป"
FROM #math
WHERE next_review <= date(today) + dur(1 day)
SORT next_review asc
```
````
