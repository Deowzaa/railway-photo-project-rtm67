# คู่มืออัปโหลดเว็บไซต์ขึ้น GitHub

## ส่วนที่ 1 สร้าง Repository

1. เข้าสู่เว็บไซต์ https://github.com และเข้าสู่ระบบ
2. กดเครื่องหมาย **+** บริเวณมุมขวาบน
3. เลือก **New repository**
4. ช่อง **Repository name** ใส่ `railway-photo-project-rtm67`
5. ช่อง **Description** ใส่ `เว็บไซต์นำเสนอโครงงานประกวดภาพถ่ายส่งเสริมการท่องเที่ยวทางรถไฟ`
6. เลือก **Public**
7. ไม่ต้องเลือก Add a README file เพราะในชุดไฟล์มี README แล้ว
8. กด **Create repository**

## ส่วนที่ 2 อัปโหลดไฟล์

1. แตกไฟล์ ZIP ที่ดาวน์โหลดไว้
2. เปิด Repository ที่เพิ่งสร้าง
3. กด **uploading an existing file** หรือเลือก **Add file > Upload files**
4. เปิดโฟลเดอร์ที่แตกไฟล์แล้ว
5. เลือกไฟล์ทั้งหมดภายในโฟลเดอร์ แล้วลากไปวางในหน้า GitHub
6. ตรวจว่ามีไฟล์ `index.html`, `README.md`, `CHANGELOG.md` และ `VERSION`
7. ช่อง Commit message ใส่ `Release v1.1.0`
8. กด **Commit changes**

> ควรอัปโหลดไฟล์ที่อยู่ “ภายในโฟลเดอร์” ไม่ใช่อัปโหลดโฟลเดอร์ครอบอีกชั้น เพื่อให้ `index.html` อยู่หน้าแรกของ Repository

## ส่วนที่ 3 เปิดใช้งาน GitHub Pages

1. เข้าเมนู **Settings** ของ Repository
2. เลือก **Pages** ทางด้านซ้าย
3. หัวข้อ **Build and deployment** เลือก **Deploy from a branch**
4. ช่อง Branch เลือก **main**
5. ช่อง Folder เลือก **/(root)**
6. กด **Save**
7. รอประมาณ 1–5 นาที แล้วรีเฟรชหน้า Pages
8. GitHub จะแสดงลิงก์เว็บไซต์ในรูปแบบ `https://ชื่อบัญชี.github.io/railway-photo-project-rtm67/`

## ส่วนที่ 4 สร้างแท็กเวอร์ชัน

1. กลับหน้าหลัก Repository
2. เลือก **Releases**
3. กด **Draft a new release**
4. กด **Choose a tag**
5. พิมพ์ `v1.1.0` แล้วเลือก **Create new tag**
6. ช่อง Release title ใส่ `Railway Photo Project v1.1.0`
7. คัดลอกรายละเอียดจากหัวข้อ 1.1.0 ในไฟล์ `CHANGELOG.md`
8. กด **Publish release**

## วิธีอัปเดตเวอร์ชันครั้งถัดไป

- แก้บั๊กเล็กน้อย: เพิ่มเลข PATCH เช่น `1.1.0 → 1.1.1`
- เพิ่มเนื้อหาหรือฟังก์ชันใหม่: เพิ่มเลข MINOR เช่น `1.1.0 → 1.2.0`
- เปลี่ยนโครงสร้างครั้งใหญ่และไม่รองรับของเดิม: เพิ่มเลข MAJOR เช่น `1.1.0 → 2.0.0`

ทุกครั้งที่อัปเดต ให้ทำ 4 อย่าง:

1. แก้หมายเลขในไฟล์ `VERSION`
2. เพิ่มรายการใหม่บนสุดของ `CHANGELOG.md`
3. Commit ด้วยข้อความ เช่น `Release v1.2.0`
4. สร้าง Release และ Tag ให้ตรงกับเวอร์ชัน

