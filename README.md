# Week 3 Lab: CSS Fundamentals

## ปฏิบัติการนี้ครอบคลุมเนื้อหา CSS ตั้งแต่พื้นฐาน ได้แก่

1. **CSS Syntax & Properties** - โครงสร้างและคุณสมบัติพื้นฐาน
2. **CSS Units** - หน่วยวัดต่าง ๆ ของ CSS
3. **CSS Selectors** - การเลือก element ด้วย selector ต่างๆ
4. **Colors & Text** - การจัดรูปแบบสี และข้อความ
5. **Box Model** - การทําความเข้าใจ Content, Padding, Border, Margin
6. **Positioning** - Static, Relative, Absolute, Fixed, Sticky
7. **Display & Layout** - Block, Inline, Flexbox, Grid

---

## File Structure

```
wk03-lab/
├── index.html           # หน้าแรก
├── styles.css           # External CSS stylesheet
├── units.html           # CSS Units - หน่วยวัด
├── box-model.html       # Box Model & Colors & Text
├── positioning.html     # Positioning examples
├── display-layout.html  # Display & Layout
└── README.md            # Documentation
```

---

## Key Concepts

### CSS Selectors Priority (Specificity)

```
Universal (*) < Element < Class < ID < Inline Style
```

ยิ่งเฉพาะเจาะจง priority ยิ่งสูง

### Box Model

```
Content → Padding → Border → Margin
```

- **Content**: เนื้อหาจริง (text, images, etc.)
- **Padding**: ระยะห่างด้านใน (ระหว่าง content และ border)
- **Border**: กรอบรอบ element
- **Margin**: ระยะห่างด้านนอก (ระหว่าง element นี้กับ element อื่น)

### Positioning Values

| Position     | อ้างอิงกับ            | ใช้เมื่อ            | ตัวอย่าง        |
| ------------ | --------------------- | ------------------- | --------------- |
| **static**   | Document flow         | ไม่ต้องย้าย         | ข้อความปกติ     |
| **relative** | ตําแหน่งเดิม          | ปรับแต่งเล็กน้อย    | ย้ายข้อความขึ้น |
| **absolute** | Parent ที่มี position | วางตําแหน่งอิสระ    | Badge, tooltip  |
| **fixed**    | Viewport              | ติดกับหน้าจอ        | Navbar, button  |
| **sticky**   | Parent + Viewport     | ติดเมื่อ scroll ถึง | Table header    |

### Display Values

| Display          | Width/Height | Line Break | ใช้เมื่อ          |
| ---------------- | ------------ | ---------- | ----------------- |
| **block**        | Yes          | Yes        | Paragraph, div    |
| **inline**       | No           | No         | span, link        |
| **inline-block** | Yes          | No         | Button, small box |
| **flex**         | Yes          | Flexible   | Flexible layout   |
| **grid**         | Yes          | Flexible   | Complex layout    |
| **none**         | N/A          | N/A        | Hide element      |

### CSS Units (หน่วยวัด)

| Unit                | ตัวอักษร | อ้างอิงกับ       | Responsive | ใช้เมื่อ                  |
| ------------------- | -------- | ---------------- | ---------- | ------------------------- |
| **Pixel**           | px       | ไม่มี (fixed)    | No         | Borders, fixed layouts    |
| **Percentage**      | %        | Parent element   | Yes        | Responsive widths         |
| **Em**              | em       | Parent font-size | Yes        | Scalable components       |
| **Rem**             | rem      | Root font-size   | Yes        | Consistent sizing (แนะนำ) |
| **Viewport Width**  | vw       | Viewport width   | Yes        | Full-width sections       |
| **Viewport Height** | vh       | Viewport height  | Yes        | Full-height sections      |

**ทิป:** ใช้ `rem` และ `%` เป็นหลัก เพราะช่วยให้เว็บไซต์ตอบสนองต่อขนาดจอต่างๆ ได้ดีขึ้น

---

## Author

- **Name:** Chutiphon Jitrungraungsuk
- **Email:** 67160003@go.buu.ac.th
