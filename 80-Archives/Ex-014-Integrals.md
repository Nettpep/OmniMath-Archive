---
type: exercise
difficulty: ⭐⭐
status: solved
last_reviewed: 
next_review: 
---
# 📝 บันทึกปริศนา: การหาปริพันธ์พื้นฐาน

## ❓ โจทย์ (The Question)
> [!quote]
> จงหาค่าของปริพันธ์ไม่จำกัดเขตต่อไปนี้:
> $$\\int (3x^2 + 2x - 5) dx$$

## 🕵️ วิธีการพิชิต (Solution)
เราจะใช้กฎการหาปริพันธ์พื้นฐาน:
$$\\int x^n dx = \\frac{x^{n+1}}{n+1} + C$$
$$\\int c \\cdot f(x) dx = c \\int f(x) dx$$
$$\\int (f(x) + g(x)) dx = \\int f(x) dx + \\int g(x) dx$$

ดังนั้น:
$$\\int (3x^2 + 2x - 5) dx = \\int 3x^2 dx + \\int 2x dx - \\int 5 dx$$
$$= 3\\int x^2 dx + 2\\int x dx - 5\\int 1 dx$$
$$= 3\\left(\\frac{x^{2+1}}{2+1}\\right) + 2\\left(\\frac{x^{1+1}}{1+1}\\right) - 5x + C$$
$$= 3\\left(\\frac{x^3}{3}\\right) + 2\\left(\\frac{x^2}{2}\\right) - 5x + C$$
$$= x^3 + x^2 - 5x + C$$

## 🧠 ทฤษฎีที่ใช้ (The Links)
- ใช้ความรู้จาก: [[50-Advanced/504-Integrals|504-Integrals]]

## ⚠️ บทเรียนที่ได้รับ (Lessons)
- [ ] อย่าลืมเพิ่มค่าคงที่ C เมื่อหาปริพันธ์ไม่จำกัดเขต
- [ ] ใช้กฎการหาปริพันธ์สำหรับแต่ละพจน์แยกกัน
