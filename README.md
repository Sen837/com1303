# com1303
# week1
# นายภาคิน คุ้มเกรง รหัสนักศึกษา :69143837
1.Gitคืออะไร
:=เป็นโปรแกรมเก็บไฟล์ถูกลบหรือแก้ไข สามารถแก้ไขเมื่อไหร่ก็ได้เราสามารถย้อนดูเวอร์ชันเก่าก่อนที่โค้ดจะพัง
เป็นโปรแกรมที่่ทำงานเหมือนGoogle Diveเขียนโค้ดอิสระไม่กระทบโค้ดหลัก
-------------------------------------------------------------------------------------------
2.การทำงานของเว็บไซต์ทำงานอย่างไร
:= 1.(โฟลเดอร์ทำงาน)เป็นโปรแกรมแก้ไขโค้ดทำเว็บไซต์ index.html, style.css,JavaScript
2.(พื้นที่เตรียมไฟล์)มีการบันทึกการเปลี่ยนแปลงในการคำสั่ง git add
3.(พื้นที่เก็บบันทึกหรือ.git)
ใช้คำสั่งgit commit หรือ snapshortในฐานข้อมูลถาวร
--------------------------------------------------------------------------------------------
3.เว็บไซต์ต่างจากเว็บแอพพลิเคชั่น อย่างไร
:=1.เว็บไซต์
จุดประสงค์ เป็นการให้ข้อมูลธุรกิจ หรือนำเสนอเนื้อหาให้คนมาดู
การทำงาน มีข้อความ ภาพหรือวีดีโอ เช่นเว็บบริษัท หรือสำนักงานข่าว
2.เว็บแอปพลิเคชั่น
จุดประสงค์ เน้นการดึงดูดให้มีผู้ใช้งานผ่านระบบ
การทำงาน มีระบซับซ้อน แต่มีแบบแผน เช่นชำระเงิน จองตั๋ว ล็อกอิน
--------------------------------------------------------------------------------------------
4.ให้สร้างคู่มือการใช้งาน Github
:=การเริ่มต้นใช้งาน GitHub
1. การสร้างบัญชี GitHub
ไปที่ GitHub และสร้างบัญชีผู้ใช้
2. การสร้าง Repository ใหม่
ล็อกอินเข้าสู่ GitHub
คลิกที่ปุ่ม New ที่มุมบนขวาของหน้าจอ
กรอกข้อมูลชื่อ repository และรายละเอียดอื่นๆ
เลือกว่าจะตั้งค่า repository เป็น Public หรือ Private
คลิกที่ปุ่ม Create repository
3. การเชื่อมต่อกับ GitHub จากเครื่องคอมพิวเตอร์
ติดตั้ง Git บนเครื่องคอมพิวเตอร์ของคุณ จากนั้นเปิด terminal หรือ command prompt และตั้งค่า Git ด้วยคำสั่งต่อไปนี้:
bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
4. การโคลน (Clone) Repository
เพื่อโคลน repository จาก GitHub มายังเครื่องคอมพิวเตอร์ของคุณ:
bash
git clone https://github.com/username/repository.git

5. การเพิ่มและคอมมิตไฟล์
เพิ่มไฟล์ใหม่หรือแก้ไขไฟล์ใน repository
เพิ่มไฟล์ที่เปลี่ยนแปลงไปยัง staging area:
bash
git add .
คอมมิตการเปลี่ยนแปลง:
bash
git commit -m "Initial commit"
ดันการเปลี่ยนแปลงไปยัง GitHub:
bash
git push origin main
6. การสร้างและใช้งาน Branch
สร้าง branch ใหม่:

bash
git checkout -b new-branch
สลับไปยัง branch ที่สร้างใหม่:

bash
git checkout new-branch
ดัน branch ใหม่ไปยัง GitHub:

bash
git push origin new-branch

7. การสร้าง Pull Request
ไปที่หน้า repository บน GitHub
คลิกที่แท็บ Pull requests
คลิกที่ปุ่ม New pull request
เลือก branch ที่ต้องการรวมเข้าด้วยกัน
คลิกที่ปุ่ม Create pull request และกรอกข้อมูลที่เกี่ยวข้อง
คลิกที่ปุ่ม Create pull request เพื่อส่ง pull request
การใช้งาน GitHub Actions
GitHub Actions ช่วยในการตั้งค่า CI/CD เพื่อทดสอบและปรับใช้โค้ดอัตโนมัติ
สร้างไฟล์ workflow ในโฟลเดอร์ .github/workflows:
yaml
name: CI
on: [push, pull_request]
jobs:
  build:
    runs-on: ubuntu-latest
    steps:
    - uses: actions/checkout@v2
    - name: Set up Node.js
      uses: actions/setup-node@v2
      with:
        node-version: '14'
    - name: Install dependencies
      run: npm install
    - name: Run tests
      run: npm test
คอมมิตและดันไฟล์ workflow ไปยัง repository
GitHub จะรัน workflow ทุกครั้งที่มีการ push หรือ pull request ตามที่กำหนดไว้ในไฟล์ workflow
------------------------------------------------------------------------------------------
(Link)(https://classroom.google.com/c/ODc0MTU2NTcwMDM3/m/ODc0MzMzMjgxNDY0/details)
