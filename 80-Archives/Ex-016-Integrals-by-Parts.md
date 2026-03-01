---
type: exercise
difficulty: ⭐⭐⭐⭐
status: solved
last_reviewed: 
next_review: 
---
# 📝 บันทึกปริศนา: การหาปริพันธ์ทีละส่วน

## ❓ โจทย์ (The Question)

> [!quote]
> จงหาค่าของปริพันธ์ไม่จำกัดเขตต่อไปนี้:
> $$\int x^2 \sin(x) dx$$

## 🕵️ วิธีการพิชิต (Solution)

เราจะใช้เทคนิคการหาปริพันธ์ทีละส่วน (Integration by Parts) ซึ่งมีสูตรคือ:
$$\int u \, dv = uv - \int v \, du$$

ในกรณีนี้ เราต้องใช้เทคนิคนี้สองครั้ง

### ครั้งที่ 1:

1.  **เลือก $u$ และ $dv$:**
    ตามหลัก LIATE (Logarithmic, Inverse trigonometric, Algebraic, Trigonometric, Exponential) เราเลือก $u = x^2$ (Algebraic) และ $dv = \sin(x) dx$ (Trigonometric)

2.  **หา $du$ และ $v$:**
    $du = 2x dx$
    $v = \int \sin(x) dx = -\cos(x)$

3.  **แทนค่าในสูตร:**
    $$\int x^2 \sin(x) dx = x^2(-\cos(x)) - \int (- \cos(x))(2x) dx$$
    $$= -x^2 \cos(x) + 2 \int x \cos(x) dx$$

เรายังคงมีปริพันธ์ $\int x \cos(x) dx$ ซึ่งต้องใช้ Integration by Parts อีกครั้ง

### ครั้งที่ 2 (สำหรับ $\int x \cos(x) dx$):

1.  **เลือก $u$ และ $dv$:**
    เลือก $u = x$ (Algebraic) และ $dv = \cos(x) dx$ (Trigonometric)

2.  **หา $du$ และ $v$:**
    $du = dx$
    $v = \int \cos(x) dx = \sin(x)$

3.  **แทนค่าในสูตร:**
    $$\int x \cos(x) dx = x \sin(x) - \int \sin(x) dx$$
    $$= x \sin(x) - (-\cos(x)) + C_1$$
    $$= x \sin(x) + \cos(x) + C_1$$

### รวมผลลัพธ์:

นำผลลัพธ์จากครั้งที่ 2 กลับไปแทนในผลลัพธ์จากครั้งที่ 1:
$$\int x^2 \sin(x) dx = -x^2 \cos(x) + 2 (x \sin(x) + \cos(x)) + C$$
$$= -x^2 \cos(x) + 2x \sin(x) + 2 \cos(x) + C$$

ดังนั้น $\int x^2 \sin(x) dx = -x^2 \cos(x) + 2x \sin(x) + 2 \cos(x) + C$

## 🧠 ทฤษฎีที่ใช้ (The Links)
- ใช้ความรู้จาก: [[50-Advanced/504-Integrals|504-Integrals]] (ส่วนเทคนิคการหาปริพันธ์ทีละส่วน)

## ⚠️ บทเรียนที่ได้รับ (Lessons)
- [ ] การหาปริพันธ์ทีละส่วนอาจต้องทำซ้ำหลายครั้งสำหรับบางฟังก์ชัน
- [ ] การเลือก $u$ และ $dv$ ที่ถูกต้องตามหลัก LIATE มีความสำคัญมาก
- [ ] ระมัดระวังเครื่องหมายลบและค่าคงที่ C
