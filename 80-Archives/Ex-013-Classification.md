---
type: exercise
difficulty: ⭐⭐⭐
level: AI/ML
level_category: advanced
tags: #exercise #level/advanced
status: solved
---
# 📝 บันทึกปริศนา: Logistic Regression

## ❓ โจทย์ (The Question)

> [!quote]
> โมเดลให้ P(spam)=0.8 สำหรับอีเมลหนึ่ง ควรจัดเป็น spam หรือไม่? และถ้า threshold = 0.7?

## 🕵️ วิธีการพิชิต (Solution)

**Threshold = 0.5 (default):** 0.8 > 0.5 → **spam** ✓  
**Threshold = 0.7:** 0.8 > 0.7 → **spam** ✓  

ทั้งสองกรณีจัดเป็น spam เพราะความน่าจะเป็นสูงกว่า threshold

## 🧠 ทฤษฎีที่ใช้ (The Links)

- ใช้ความรู้จาก: [[70-AI-ML/703-Classification|703-Classification]], [[50-Advanced/502-Probability|502-Probability]]
