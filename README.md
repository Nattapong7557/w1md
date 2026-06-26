# ระบบร้านขายรูปภาพศิลปะออนไลน์ (Art Gallery Platform)
## Workshop #1: Analysis & Design (CSI204)

ยินดีต้อนรับสู่ระบบร้านขายรูปภาพศิลปะออนไลน์ โครงสร้างเว็บไซต์สำหรับนำเสนอเอกสารการวิเคราะห์และออกแบบระบบเชิงโต้ตอบระดับพรีเมียม (Interactive System Architecture Dashboard) ที่พัฒนาด้วยการใช้ HTML, CSS (Vanilla CSS), และ JavaScript (Modern ES6) 

หน้าเว็บได้รับการจัดแต่งด้วยธีมสีมืดแบบ **Obsidian Glassmorphism** พร้อมระบบการแปลงเอกสาร Markdown และการวาดไดอะแกรม Mermaid.js สถาปัตยกรรมระบบโดยตรงจากซอฟต์แวร์

---

## 🚀 คุณสมบัติที่สำคัญ (Key Features)
1. **Interactive Markdown Document View**: โหลดและจัดรูปแบบเอกสารความต้องการของระบบ (`srs.md`) ผ่าน `marked.js` อย่างอัตโนมัติ
2. **Dynamic Table of Contents (TOC)**: สร้างรายการสารบัญฝั่งซ้ายแบบมีระบบระบุการอ่านปัจจุบัน (Scroll Spy) คอยเปลี่ยนไฮไลต์เมื่อผู้ใช้เลื่อนลงไปอ่านหัวข้อต่างๆ
3. **Live Mermaid Rendering**: ประมวลผลและแปลงบล็อก Mermaid code ให้กลายเป็นแผนภาพสถาปัตยกรรมระบบ (System Architecture & ER Diagrams) บนหน้าเว็บทันที
4. **Dual Themes Switcher (Dark/Light)**: สลับชุดสีการแสดงผลระหว่างธีมมืดและธีมสว่างเพื่อความเหมาะสมในทุกช่วงเวลา
5. **Obsidian Glassmorphic UI**: การดีไซน์แบบพรีเมียมโดยเน้นการใช้เฉดสีมืด คลื่นแสงไฟนีออนพัลส์ และหน้าต่างโปร่งแสง (Backdrop Blur)
6. **Mobile First Responsive Layout**: สามารถจัดเรียงองค์ประกอบและเปิดเมนูสารบัญด้วยปุ่มแฮมเบอร์เกอร์บนทุกขนาดหน้าจอ
7. **Marketing Landing Page**: หน้า Marketing สำหรับร้านขายรูปภาพศิลปะ พร้อม Gallery, Pricing, Testimonials
8. **Analysis & Design Document**: เอกสาร Analysis & Design ครบถ้วน พร้อม Software Architecture 3 ชั้น

---

## 📂 โครงสร้างของไฟล์งาน

```
w1md/
├── index.html            # หน้า SRS Dashboard (Interactive Viewer)
├── marketing.html        # หน้า Marketing Landing Page
├── srs.md                # เอกสาร Software Requirements Specification
├── analysis_design.md    # เอกสาร Analysis & Design + Software Architecture
├── architecture.mmd      # Mermaid Diagram ไฟล์แยก (เปิดใน mermaid.live ได้)
├── README.md             # คำอธิบายโปรเจกต์
└── img/                  # รูปภาพศิลปะสำหรับหน้า Marketing
    ├── art1.png
    ├── art2.png
    ├── art3.png
    └── art4.png
```

---

## 🛠️ วิธีการเปิดใช้งาน
คุณสามารถใช้งานแดชบอร์ดนี้ได้ทันทีโดยไม่ต้องรันเซอร์เวอร์หลังบ้านที่ยุ่งยาก:
1. ดับเบิลคลิกเปิดไฟล์ `index.html` บนเบราว์เซอร์ใดก็ได้ (Chrome, Firefox, Safari, Edge)
2. หรือใช้เครื่องมือไลฟ์เซิร์ฟเวอร์ในการทดสอบบนเครื่องเช่น:
   - Live Server extension ใน VS Code
   - รันคำสั่งไพธอน: `python -m http.server 8000` แล้วเข้าชมผ่าน `http://localhost:8000`

---

## 📄 รายละเอียดหน้าเว็บ

| หน้า | ไฟล์ | รายละเอียด |
|---|---|---|
| **SRS Dashboard** | `index.html` | แสดงเอกสาร SRS แบบ Interactive พร้อม TOC, Mermaid Diagram, Dark/Light Theme |
| **Marketing** | `marketing.html` | Landing Page ร้านขายรูปภาพศิลปะ พร้อม Gallery, Features, Pricing, Testimonials |
| **SRS Document** | `srs.md` | เอกสารข้อกำหนดความต้องการซอฟต์แวร์ (Functional & Non-Functional Requirements, API, Database) |
| **Analysis & Design** | `analysis_design.md` | เอกสารวิเคราะห์และออกแบบระบบ (Use Case, ERD, Sequence Diagram, Software Architecture) |

---

## 📝 รายงานการทำแบบฝึกหัด (Workshop 1 Checklist)
ตามข้อกำหนดในการตรวจงาน 6 ข้อหลักในสไลด์เรียน CSI204:
- [x] **1. GitHub Repository Setup**: มีระบบการติดตั้ง Git ภายในโฟลเดอร์เรียบร้อย
- [x] **2. Commit History (SourceTree ready)**: จัดแบ่งและบันทึกประวัติการพัฒนาออกมาเป็นขั้นตอนแบบมีความหมายชัดเจน
- [x] **3. Markdown in HTML**: ใช้สคริปต์แยกส่วน Markdown มาแปลงเป็นโครงสร้าง HTML สวยงามในหน้าจอเดียว
- [x] **4. Analysis & Design Documentation**: มีเอกสาร `srs.md` และ `analysis_design.md` ระบุสเปกอย่างครบถ้วน
- [x] **5. System Architecture (Mermaid)**: แผนภาพสถาปัตยกรรมเชื่อมต่อและประมวลผลอัตโนมัติ
- [x] **6. GitHub Pages Ready**: ลิงก์และไฟล์อ้างอิงทั้งหมดทำงานผ่าน Relative Paths พร้อมเผยแพร่ขึ้นโฮสติ้งของกิตฮับได้ทันที