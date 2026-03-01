---
type: exercise
difficulty: ⭐⭐
level: ม.6/ป.ตรี
level_category: advanced
tags: #exercise #level/advanced
status: solved
---
# 📝 บันทึกปริศนา: อนุพันธ์

## ❓ โจทย์ (The Question)

> [!quote]
> จงหา $\frac{d}{dx}(3x^4 - 2x^2 + 5)$

## 🕵️ วิธีคิด (Solution)

> [!info] อนุพันธ์ = อัตราการเปลี่ยนแปลง
> $\frac{d}{dx}(x^n) = nx^{n-1}$ — ลดเลขชี้กำลัง 1 แล้วคูณด้วยเลขชี้กำลังเดิม

$$\frac{d}{dx}(3x^4 - 2x^2 + 5) = 3(4x^3) - 2(2x) + 0 = 12x^3 - 4x$$

> [!example] 🔥 แต่ละพจน์
> - $3x^4$ → 3 คงที่, $x^4$ → $4x^3$ → ได้ $12x^3$
> - $-2x^2$ → $-2(2x) = -4x$
> - $5$ คงที่ → อนุพันธ์ = 0

> [!tip] ใน Gradient Descent (ML)
> อนุพันธ์บอก "ทิศทางที่ loss เพิ่มขึ้น" — เราเดินตรงข้ามเพื่อลด loss

## 🧠 ทฤษฎีที่ใช้ (The Links)

- ใช้ความรู้จาก: [[50-Advanced/501-Derivatives|501-Derivatives]], [[20-Pre-Algebra/201-Like-Terms|201-Like-Terms]]

## ⚠️ บทเรียนที่ได้รับ (Lessons)

- [x] อนุพันธ์ของค่าคงที่ = 0
