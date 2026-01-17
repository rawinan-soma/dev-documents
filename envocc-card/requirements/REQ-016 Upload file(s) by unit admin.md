# REQ-015 Upload file(s) by unit admin
### Use case
- upload เอกสารคำขอมีบัตร
- upload เอกสารประสบการณ์
- upload บัตรประจำตัวเจ้าหน้าที่รัฐ
### ผู้ใช้งานหลัก
- unit admin
### Objectives
- เพื่อเพิ่มไฟล์ที่จำเป็นต่อการอนุมัติคำขอมีบัตรต่อไป
### Functional Requirements
1. ระบบจะต้องมีช่องทางให้ unit admin เข้าถึงการเพิ่มไฟล์
2. ระบบจะต้องมีการตรวจสอบสถานะของคำร้องก่อนที่จะเพิ่ม file
3. ระบบจะต้องมีที่กรอกข้อมูลของไฟล์นั้นๆ (metadata)
4. ระบบจะต้องให้ user upload ไฟล์ได้
5. ระบบจะต้องมีการตรวจสอบไฟล์ภาพก่อนบันทึกลงระบบ
6. ระบบจะต้องมีการ update สถานะของคำร้องขอมีบัตรหลังจากการบันทึกไฟล์และข้อมูล
### Pre-conditions
- ก่อนที่จะมีการ upload file 
	- unit admin ต้องทำการเข้าสู่ระบบ
	- สถานะคำร้องของ user จะต้องอยู่ในขั้นตอนการ upload file
### Post-conditions
- ถ้า unit admin
	- กรอกข้อมูลถูกต้อง และ
	- Upload file  และ
	- file ถูกต้องตามรูปแบบ
- ระบบจะต้อง
	- บันทึก file ลงใน storage
	- บันทึกข้อมูลของไฟล์ (metadata) ลงในฐานข้อมูล
### Alternate conditions
- ไม่มี
### Exception conditions
- ถ้า unit admin
	- กรอกข้อมูลไม่ถูกต้อง
	- ไม่ upload file
	- upload file ไม่ถูกต้องตามรูปแบบที่กำหนด
- ระบบจะต้อง
	- ปฏิเสธการเพิ่มไฟล์
	- แจ้งเตือนไปยัง admin
### Flow chart
- xxx