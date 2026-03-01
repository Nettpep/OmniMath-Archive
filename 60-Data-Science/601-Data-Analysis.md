---
type: concept
tags: #data-science #status/permanent
---
# 🪐 การวิเคราะห์ข้อมูล (Data Analysis)

> [!abstract] หัวใจสำคัญ
> การวิเคราะห์ข้อมูลคือกระบวนการสำรวจ ทำความเข้าใจ และสรุปข้อมูล — ขั้นตอนแรกก่อนสร้างโมเดล ML ประกอบด้วย EDA (Exploratory Data Analysis), การทำความสะอาดข้อมูล และการเลือก features

## 📜 กฎและสูตร (The Laws)

### ขั้นตอนหลัก
1. **โหลดข้อมูล** — อ่าน CSV, JSON, Database
2. **สำรวจ (EDA)** — ดู distribution, missing values, outliers
3. **ทำความสะอาด** — แก้ missing, ลบ/จัดการ outliers
4. **Feature Engineering** — สร้าง/แปลง features
5. **เตรียมข้อมูล** — train/test split, normalization

### สถิติที่ใช้
- [[50-Advanced/503-Statistics|503-Statistics]] — mean, median, std, correlation
- Histogram, Box plot, Scatter plot

## ⛓️ เส้นใยความสัมพันธ์ (Dependencies)

- **ต้องรู้ก่อน:** [[50-Advanced/503-Statistics|503-Statistics]], [[50-Advanced/502-Probability|502-Probability]], [[40-Geometry-Trig/402-Matrices|402-Matrices]]
- **นำไปสู่:** [[60-Data-Science/602-Linear-Regression|602-Linear-Regression]], [[60-Data-Science/603-Clustering|603-Clustering]], [[70-AI-ML/701-Linear-Regression|701-Linear-Regression]]

## 💡 วิธีการมอง (Mental Model)

> [!example] เปรียบเทียบ: ตรวจสุขภาพก่อนวิ่งมาราธอน
> ต้องรู้ข้อมูลพื้นฐานก่อน — อายุ, น้ำหนัก, ประวัติ — จึงวางแผนได้

> [!example] Garbage In, Garbage Out
> ข้อมูลไม่ดี → โมเดลไม่ดี — การวิเคราะห์ข้อมูลที่ดีคือรากฐานของ ML ที่ดี

## 📑 รายการโจทย์ที่เกี่ยวข้อง

- [ ] [[80-Archives/Ex-009-Data-Analysis|Ex-009-Data-Analysis]]
