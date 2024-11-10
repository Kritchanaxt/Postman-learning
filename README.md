# 🧑🏽‍🚀 คู่มือการใช้งาน Postman 

- #### Postman เป็นเครื่องมือที่สำคัญสำหรับนักพัฒนาในการทดสอบและจัดการ API โดยรองรับการส่งคำขอ HTTP การจัดกลุ่มคำขอ และการทดสอบ API ให้มีประสิทธิภาพมากขึ้น ทำให้การทำงานร่วมกันภายในทีมเป็นเรื่องง่ายยิ่งขึ้น 

### ประเภทคำขอ HTTP หลักใน Postman
1. **GET**: ใช้ดึงข้อมูล เช่น ข้อมูลผู้ใช้หรือรายการสินค้า
2. **POST**: ใช้สร้างข้อมูลใหม่ เช่น การลงทะเบียนผู้ใช้ใหม่
3. **PUT**: ใช้อัปเดตข้อมูล เช่น การแก้ไขข้อมูลผู้ใช้
4. **DELETE**: ใช้ลบข้อมูล เช่น การลบผู้ใช้หรือสินค้าที่ไม่ต้องการ
5. **PATCH**: ใช้อัปเดตข้อมูลบางส่วนในเซิร์ฟเวอร์ โดยไม่ต้องอัปเดตข้อมูลทั้งหมด

### การใช้งาน Postman สำหรับคำขอ API
1. **เลือกประเภทคำขอ** (GET, POST, PUT, DELETE) จากเมนูดรอปดาวน์
2. **ใส่ URL ของ API**: ระบุปลายทางของ API ที่ต้องการ
3. **ตั้งค่า Headers และ Body**: เพิ่ม headers หรือข้อมูลที่ต้องการ เช่น JSON ในคำขอ POST/PUT
4. **ส่งคำขอและดูการตอบสนอง**: คลิก “Send” เพื่อส่งคำขอและดูสถานะ HTTP และข้อมูลที่เซิร์ฟเวอร์ตอบกลับ

### ฟีเจอร์หลักของ Postman
1. **การสร้างและส่งคำขอ**: รองรับคำขอ HTTP ได้หลายประเภท โดยสามารถกำหนดค่า headers และ body ได้อย่างยืดหยุ่น
2. **การจัดการ Collections**: จัดกลุ่มคำขอ API ให้เป็นระบบในโปรเจกต์
3. **Environment Variables**: ใช้ตัวแปรเพื่อสลับระหว่างสภาพแวดล้อม เช่น Development, Testing และ Production
4. **การทดสอบอัตโนมัติ**: เขียน script เพื่อตรวจสอบผลลัพธ์ของการตอบสนอง
5. **Mock Servers**: จำลองการตอบสนองของเซิร์ฟเวอร์ ทำให้สามารถทดสอบได้แม้ยังไม่มีเซิร์ฟเวอร์จริง
6. **การทำงานร่วมกัน**: แชร์ Collections และ environment กับทีมเพื่อพัฒนา API ร่วมกัน


## คู่มือการใช้งาน Postman (เพิ่มเติม)

### Postman รองรับฟีเจอร์เพิ่มเติมที่สำคัญต่อการพัฒนาและทดสอบ API ดังนี้

#### 1. Collection Runner
เครื่องมือทดสอบคำขอหลายคำขอพร้อมกัน โดยสามารถใช้กับ Data Driven Testing เพื่อนำเข้าข้อมูลจากไฟล์ CSV หรือ JSON

#### 2. Script และ Code Snippets
รองรับการเขียน JavaScript เพื่อตรวจสอบ API:
- **Pre-request Scripts**: ใช้กำหนดค่าก่อนส่งคำขอ เช่น สร้าง token
- **Test Scripts**: ตรวจสอบค่าจากคำขอ เช่น สถานะ HTTP หรือข้อมูลใน response body

#### 3. Global Variables, Collection Variables, Environment Variables, Local Variables, Dynamic Variables
ตัวแปรที่ใช้จัดการข้อมูลในสภาพแวดล้อมต่างๆ:
- **Global Variables**: ใช้ในทุก Collection และทุก Environment
- **Collection Variables**: ใช้เฉพาะใน Collection
- **Environment Variables**: ตัวแปรที่แตกต่างกันตาม environment
- **Local Variables**: ตัวแปรเฉพาะใน request นั้นๆ
- **Dynamic Variables**: ตัวแปรที่ Postman กำหนดมา เช่น random email, random number

#### 4. Data Driven Testing (CSV / JSON)
นำเข้าข้อมูลจากไฟล์ CSV/JSON สำหรับทดสอบ API ด้วยข้อมูลที่หลากหลาย ร่วมกับ Collection Runner 

#### 5. Authentication (GitHub API)
รองรับการทำ Authentication หลายรูปแบบ เช่น Basic Auth, OAuth 1.0/2.0, API Key:
- **GitHub API**: ใช้ token ใน Authentication ของ Postman โดยเลือก “Bearer Token” แล้วใส่ token ในฟิลด์


### สรุป
Postman ช่วยให้การทดสอบและการจัดการ API เป็นเรื่องง่ายขึ้นด้วยฟีเจอร์ที่หลากหลายเหมาะสมสำหรับนักพัฒนาที่ต้องการจัดการและทดสอบ API
