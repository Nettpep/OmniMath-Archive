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

## 🕵️ วิธีคิด (Solution)

> [!info] Classification = เลือก class ตามความน่าจะเป็น
> โมเดลให้ P(spam) = 0.8 → เปรียบเทียบกับ **threshold** (ค่าแบ่ง) → ถ้าเกิน = spam

**Threshold = 0.5 (default):**  
$0.8 > 0.5$ → **spam** ✓

**Threshold = 0.7:**  
$0.8 > 0.7$ → **spam** ✓

> [!example] 🔥 เห็นภาพ
> P(spam)=0.8 = โมเดลมั่นใจ 80% ว่าเป็น spam — ไม่ว่า threshold จะ 0.5 หรือ 0.7 ก็ยังเกินทั้งคู่ → จัดเป็น spam

> [!tip] เมื่อไหร่ปรับ threshold?
> ถ้าไม่อยากพลาด spam (false negative) → ลด threshold | ถ้าไม่อยากแจ้ง spam ผิด (false positive) → เพิ่ม threshold

## 🧠 ทฤษฎีที่ใช้ (The Links)

- ใช้ความรู้จาก: [[70-AI-ML/703-Classification|703-Classification]], [[50-Advanced/502-Probability|502-Probability]]
