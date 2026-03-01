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

## 🕵️ วิธีคิด (Solution)

> [!info] K-Means = แบ่งกลุ่มโดยให้จุดใกล้ centroid ของกลุ่มมากที่สุด
> 1) แต่ละจุดไปกลุ่มที่ centroid ใกล้ที่สุด  
> 2) อัปเดต centroid = ค่าเฉลี่ยของจุดในกลุ่ม  
> 3) ทำซ้ำจน centroid ไม่เปลี่ยน

**ขั้นที่ 1: คำนวณระยะทาง (Euclidean)**
- ถึง (1,1): (1,1)=0, (2,1)=1, (4,3)=√13≈3.6, (5,4)=5
- ถึง (5,4): (1,1)=5, (2,1)=√18≈4.2, (4,3)=√2≈1.4, (5,4)=0

**ขั้นที่ 2: แบ่งกลุ่ม** (เลือก centroid ใกล้กว่า)
- **กลุ่ม 1:** (1,1), (2,1) → centroid ใหม่ = (1.5, 1)
- **กลุ่ม 2:** (4,3), (5,4) → centroid ใหม่ = (4.5, 3.5)

> [!example] 🔥 เห็นภาพ
> จุด 4 จุดบนระนาบ — จับคู่เป็น 2 กลุ่มที่ "อยู่ใกล้กัน" — กลุ่มซ้ายล่าง vs กลุ่มขวาบน

## 🧠 ทฤษฎีที่ใช้ (The Links)

- ใช้ความรู้จาก: [[60-Data-Science/603-Clustering|603-Clustering]], [[40-Geometry-Trig/401-Vectors|401-Vectors]]
