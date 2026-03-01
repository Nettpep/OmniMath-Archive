---
type: exercise
difficulty: ⭐⭐⭐
status: solved
---
# 📝 บันทึกปริศนา: EDA

## ❓ โจทย์ (The Question)

> [!quote]
> ข้อมูลมี missing values 10% ในคอลัมน์ "อายุ" คุณจะจัดการอย่างไร?

## 🕵️ วิธีการพิชิต (Solution)

**ทางเลือก:**
1. **ลบแถว** — ถ้า missing น้อยและข้อมูลมาก
2. **เติมค่าเฉลี่ย/มัธยฐาน** — ถ้า missing แบบสุ่ม
3. **เติมด้วยโมเดล** — Predict จาก features อื่น
4. **สร้าง category "Unknown"** — สำหรับ categorical

**แนะนำ:** ดู distribution ก่อน — ถ้า 10% และข้อมูล 1000 แถว อาจเติมมัธยฐานได้

## 🧠 ทฤษฎีที่ใช้ (The Links)

- ใช้ความรู้จาก: [[60-Data-Science/601-Data-Analysis|601-Data-Analysis]], [[50-Advanced/503-Statistics|503-Statistics]]
