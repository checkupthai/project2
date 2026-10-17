# 🏥 Medical Examination Hub (คลินิกบริการตรวจสุขภาพดิจิทัล)

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge)](LICENSE)

> **ผู้พัฒนาและออกแบบระบบ:** **นพ.เฉลิมรัฐ เมฆอุไรพร (Dr. Chalermrat Meyoutam)**  
> *เวชศาสตร์อาชีวอนามัยและสิ่งแวดล้อม | เวชศาสตร์ป้องกัน | สารสนเทศทางการแพทย์*  
> 🌐 **เว็บไซต์ทางการ:** [www.drchalermrat.com](https://www.drchalermrat.com)

---

## 📋 ภาพรวมโครงการ (Project Overview)

**Medical Examination Hub** เป็นระบบเว็บแอปพลิเคชันรวมศูนย์การให้บริการตรวจสุขภาพดิจิทัลแบบครบวงจร พัฒนาขึ้นด้วยเทคโนโลยี Client-Side Web Architecture (Pure HTML5 / Modern CSS / Vanilla JavaScript ES6+) ทำงานได้ทันทีโดยไม่ต้องพึ่งพาเซิร์ฟเวอร์หรือฐานข้อมูลภายนอก (Zero-Backend Dependency) 

สามารถนำขึ้นโฮสต์ฟรีผ่าน **GitHub Pages** หรือเปิดใช้งานแบบออฟไลน์บนคอมพิวเตอร์ในคลินิกหรือสถานพยาบาลได้ทันที

---

## 🚀 ฟังก์ชันหลักของระบบ (Core Features)

ระบบประกอบด้วย 5 โมดูลบริการหลักที่เชื่อมโยงกันอย่างเป็นระบบ:

### 1. 📋 ตรวจสุขภาพประจำปี (Annual Health Checkup Form v3.3)
- แบบบันทึกและประเมินผลการตรวจร่างกายประจำปี (PE: Physical Examination)
- บันทึกการซักประวัติตามระบบ, ผลตรวจทางห้องปฏิบัติการ (Lab), เอกซเรย์ทรวงอก (CXR)
- สรุปความเห็นและคำแนะนำของแพทย์ผู้ตรวจตามมาตรฐานเวชศาสตร์ป้องกัน

### 2. 💼 ตรวจสุขภาพก่อนเข้างาน (Pre-employment Screening 3-Step Pipeline)
กระบวนการตรวจคัดกรองความพร้อมของผู้สมัครงานและพนักงานใหม่แบบต่อเนื่อง 3 ขั้นตอน:
- **ขั้นตอนที่ 1 (`nph.html`):** หน้าสรุปข้อมูลผู้รับการตรวจ รวบรวมผลตรวจสำคัญ และออกเอกสารรับรอง
- **ขั้นตอนที่ 2 (`vision.html`):** ตรวจคัดกรองสายตา Snellen Chart (Corrected/Uncorrected) และตรวจตาบอดสี Ishihara Plates พร้อมจับคู่ความเหมาะสมกับตำแหน่งงาน
- **ขั้นตอนที่ 3 (`hearing.html`):** บันทึกผลตรวจสมรรถภาพการได้ยิน (Occupational Audiogram) ความถี่ 500 – 8,000 Hz พร้อมกราฟ Chart.js แยกหูซ้าย/ขวา และจัดหน้าพิมพ์ขนาด A4

### 3. 🎀 ระบบแปลผล Breast Mammogram & Ultrasound
- โปรแกรมสกัดรายงานผลตรวจแมมโมแกรมและอัลตราซาวด์เต้านมภาษาอังกฤษ คัดกรองเฉพาะรอยโรคสำคัญ:
  - **หินปูน (Calcification):** ระบุข้าง ซ้าย/ขวา/ทั้งสองข้าง พร้อมดึงข้อความอ้างอิง
  - **ถุงน้ำ (Cyst):** ระบุตำแหน่งข้าง ซ้าย/ขวา/ทั้งสองข้าง
  - **ก้อนเนื้อ (Mass):** ระบุขนาดเส้นผ่านศูนย์กลางและตำแหน่ง
- จำแนกกลุ่ม **BI-RADS 1 - 5** พร้อมคำแนะนำแพทย์และการติดตามผล
- **ปุ่ม "วางข้อความที่คัดลอกมา" (Paste from Clipboard):** คลิกเดียวดึงข้อความจากคลิปบอร์ดมาวางและสรุปผลทันที

### 4. 🩺 ระบบแปลผล Abdominal Ultrasound (ช่องท้องส่วนบน/ล่าง)
- โปรแกรมสกัดรายงานผลตรวจอัลตราซาวด์ช่องท้อง (Whole / Upper / Lower Abdomen)
- คัดกรองเฉพาะความผิดปกติที่ตรวจพบจริง และแยกส่งต่อแพทย์เฉพาะทาง 3 สาขา:
  - **สูตินรีเวช:** มดลูก (Myoma, ก้อนเนื้อ), รังไข่, ปีกมดลูก, ถุงน้ำ
  - **ทางเดินอาหาร & ตับ-ถุงน้ำดี:** ไขมันเกาะตับ, ถุงน้ำในตับ, ติ่งเนื้อ/นิ่วถุงน้ำดี
  - **ทางเดินปัสสาวะ:** ไต (ถุงน้ำ, นิ่ว) และต่อมลูกหมากโต (Prostatomegaly/BPH)
- **ปุ่ม "วางข้อความที่คัดลอกมา" (Paste from Clipboard):** คลิกเดียวดึงข้อความจากคลิปบอร์ดมาวางและสรุปผลทันที

### 5. 🤖 ChatGPT Medical Prompt Templates (1-Click Copy)
- ศูนย์รวมแม่แบบคำสั่ง Prompt สำหรับนำไปวางใน ChatGPT
- **Template 1 (U/S):** คำสั่งควบคุม ChatGPT สรุปผลอัลตราซาวด์ช่องท้องแยก 3 ระบบ พร้อมตัวอย่างและคำศัพท์ภาษาอังกฤษในวงเล็บ
- **Template 2 (MMG):** คำสั่งควบคุม ChatGPT สรุปผลแมมโมแกรม คัดกรอง หินปูน, ถุงน้ำ, ก้อนเนื้อ จัดกลุ่ม BI-RADS 1-5
- **ปุ่มคัดลอก 1-Click Copy:** พร้อมการแจ้งเตือน Toast แจ้งเตือนเมื่อคัดลอกสำเร็จ และปุ่มเปิดหน้าต่าง ChatGPT.com ได้ทันที

---

## 📂 โครงสร้างไฟล์ใน Repository

```text
├── index.html                 # หน้าหลักของระบบ (Main Landing Page สำหรับ GitHub Pages)
├── all.html                   # หน้าหลักสำรอง (Alias สำหรับการเรียกเข้า all.html)
├── mammogram.html             # ระบบแปลผลแมมโมแกรม & อัลตราซาวด์เต้านม (Full App)
├── ultrasound.html            # ระบบแปลผลอัลตราซาวด์ช่องท้อง (Full App)
├── pyt3.3.html                # แบบฟอร์มตรวจสุขภาพประจำปี (Annual Exam Form v3.3)
├── nph.html                   # ตรวจก่อนเข้างาน ขั้นตอนที่ 1: บันทึกประวัติและหน้าสรุปผล
├── vision.html                # ตรวจก่อนเข้างาน ขั้นตอนที่ 2: ตรวจสายตาและตาบอดสี
├── hearing.html               # ตรวจก่อนเข้างาน ขั้นตอนที่ 3: ตรวจสมรรถภาพการได้ยิน
├── README.md                  # คู่มือรายละเอียดโครงการและการติดตั้ง
├── LICENSE                    # สัญญาอนุญาตซอฟต์แวร์ MIT License
└── .gitignore                 # ข้อยกเว้นไฟล์ระบบ
```

---

## 🌐 วิธีนำขึ้นโฮสต์บน GitHub Pages (เปิดเว็บใช้งานฟรี)

1. เข้าไปที่ [GitHub.com](https://github.com) แล้วกด **New repository** (ตั้งชื่อ เช่น `medical-examination-hub`)
2. ในหน้า Repository คลิกปุ่ม **"Add file"** ➡️ **"Upload files"**
3. ลากไฟล์ทั้งหมดในโฟลเดอร์นี้ไปวางในหน้าเว็บ
4. เลื่อนลงมากดปุ่ม **"Commit changes"**
5. ไปที่เมนู **Settings** ⚙️ ของ Repository > เลือกแถบ **Pages** (เมนูด้านซ้าย)
6. ในหัวข้อ **Build and deployment > Branch** ให้เลือกเป็น `main` (หรือ `master`) และโฟลเดอร์ `/ (root)` แล้วกด **Save**
7. รอประมาณ 1 นาที เว็บไซต์จะออนไลน์ทันทีที่:
   ```
   https://<ชื่อ-username-ของคุณ>.github.io/<ชื่อ-repository>/
   ```

---

## ⚖️ ข้อสงวนสิทธิ์ทางการแพทย์ (Medical Disclaimer)

ระบบนี้พัฒนาขึ้นเพื่อการสาธิตนวัตกรรมสุขภาพดิจิทัล การศึกษาทางการแพทย์ และเพิ่มประสิทธิภาพกระบวนการทำงานด้านอาชีวอนามัยและเวชศาสตร์ป้องกัน อัลกอริทึมการจำแนกผลตรวจอ้างอิงตามแนวทางเวชปฏิบัติมาตรฐานสากล (BI-RADS, แนวปฏิบัติกระทรวงสาธารณสุขไทย) อย่างไรก็ตาม ระบบนี้เป็นเครื่องมือสนับสนุนการทำงานเท่านั้น มิได้ใช้ทดแทนการตรวจวินิจฉัย ซักประวัติ และตัดสินใจรักษาโดยแพทย์ผู้มีใบอนุญาตประกอบวิชาชีพเวชกรรม

---

## 👨‍⚕️ ผู้จัดทำและติดต่อ (Author & Contact)

**นพ.เฉลิมรัฐ เมฆอุไรพร (Dr. Chalermrat Meyoutam)**  
- เว็บไซต์ทางการ: [www.drchalermrat.com](https://www.drchalermrat.com)  
- ความเชี่ยวชาญ: Occupational Medicine, Preventive Medicine, Medical Informatics, AI Clinical Workflows
