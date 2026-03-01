---
type: exercise
difficulty: ⭐⭐
status: solved
last_reviewed: 
next_review: 
---
# 📝 บันทึกปริศนา: การหาปริพันธ์พื้นฐานและประยุกต์

## ❓ โจทย์ (The Question)

> [!quote]
> **โจทย์ที่ 1:** จงหาค่าของปริพันธ์ไม่จำกัดเขตต่อไปนี้:
> $$\int (3x^2 + 2x - 5) dx$$
>
> **โจทย์ที่ 2:** จงหาค่าของปริพันธ์ไม่จำกัดเขตต่อไปนี้:
> $$\int (4x^3 - \frac{1}{x^2} + \sqrt{x}) dx$$

## 🕵️ วิธีการพิชิต (Solution)

### โจทย์ที่ 1: $\int (3x^2 + 2x - 5) dx$

เราจะใช้กฎการหาปริพันธ์พื้นฐาน:
$$\int x^n dx = \frac{x^{n+1}}{n+1} + C$$
$$\int c \cdot f(x) dx = c \int f(x) dx$$
$$\int (f(x) + g(x)) dx = \int f(x) dx + \int g(x) dx$$

ดังนั้น:
$$\int (3x^2 + 2x - 5) dx = \int 3x^2 dx + \int 2x dx - \int 5 dx$$
$$= 3\int x^2 dx + 2\int x dx - 5\int 1 dx$$
$$= 3\left(\frac{x^{2+1}}{2+1}\right) + 2\left(\frac{x^{1+1}}{1+1}\right) - 5x + C$$
$$= 3\left(\frac{x^3}{3}\right) + 2\left(\frac{x^2}{2}\right) - 5x + C$$
$$= x^3 + x^2 - 5x + C$$

### โจทย์ที่ 2: $\int (4x^3 - \frac{1}{x^2} + \sqrt{x}) dx$

ก่อนอื่น เราจะเขียนฟังก์ชันให้อยู่ในรูป $x^n$ เพื่อให้ง่ายต่อการหาปริพันธ์:
$$\frac{1}{x^2} = x^{-2}$$
$$\sqrt{x} = x^{\frac{1}{2}}$$

ดังนั้น โจทย์จะกลายเป็น:
$$\int (4x^3 - x^{-2} + x^{\frac{1}{2}}) dx$$

ใช้กฎการหาปริพันธ์พื้นฐานสำหรับแต่ละพจน์:
$$= 4\int x^3 dx - \int x^{-2} dx + \int x^{\frac{1}{2}} dx$$
$$= 4\left(\frac{x^{3+1}}{3+1}\right) - \left(\frac{x^{-2+1}}{-2+1}\right) + \left(\frac{x^{\frac{1}{2}+1}}{\frac{1}{2}+1}\right) + C$$
$$= 4\left(\frac{x^4}{4}\right) - \left(\frac{x^{-1}}{-1}\right) + \left(\frac{x^{\frac{3}{2}}}{\frac{3}{2}}\right) + C$$
$$= x^4 - (-x^{-1}) + \frac{2}{3}x^{\frac{3}{2}} + C$$
$$= x^4 + \frac{1}{x} + \frac{2}{3}x\sqrt{x} + C$$

## 🧠 ทฤษฎีที่ใช้ (The Links)
- ใช้ความรู้จาก: [[50-Advanced/504-Integrals|504-Integrals]]

## ⚠️ บทเรียนที่ได้รับ (Lessons)
- [ ] อย่าลืมเพิ่มค่าคงที่ C เมื่อหาปริพันธ์ไม่จำกัดเขต
- [ ] ใช้กฎการหาปริพันธ์สำหรับแต่ละพจน์แยกกัน
- [ ] แปลงรูปฟังก์ชันให้อยู่ในรูป $x^n$ ก่อนหาปริพันธ์เสมอสำหรับพจน์ที่เป็นเศษส่วนหรือราก
