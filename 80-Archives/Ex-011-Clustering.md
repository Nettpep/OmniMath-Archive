---
type: exercise
difficulty: ⭐⭐⭐
level: Data Science
level_category: advanced
tags: #exercise #level/advanced
status: solved
---
# 📝 บันทึกปริศนา: K-Means

## ❓ โจทย์ (The Question)

> [!quote]
> ข้อมูล 2 มิติ: (1,1), (2,1), (4,3), (5,4) ใช้ K=2 โดย centroid เริ่มต้นที่ (1,1) และ (5,4) จงแบ่งกลุ่ม

## 🕵️ วิธีการพิชิต (Solution)

**ระยะทางถึง (1,1):** (1,1)=0, (2,1)=1, (4,3)=3.6, (5,4)=5  
**ระยะทางถึง (5,4):** (1,1)=5, (2,1)=4.2, (4,3)=1.4, (5,4)=0

**กลุ่ม 1:** (1,1), (2,1) — centroid ใหม่ = (1.5, 1)  
**กลุ่ม 2:** (4,3), (5,4) — centroid ใหม่ = (4.5, 3.5)

## 🧠 ทฤษฎีที่ใช้ (The Links)

- ใช้ความรู้จาก: [[60-Data-Science/603-Clustering|603-Clustering]], [[40-Geometry-Trig/401-Vectors|401-Vectors]]
