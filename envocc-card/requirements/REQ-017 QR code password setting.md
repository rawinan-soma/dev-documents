# REQ-016 QR code password setting
### Use case
- ตั้งรหัส qr code
### ผู้ใช้งานหลัก
- user ผู้ร้องขอมีบัตร
### Objectives
- เพื่อตั้งรหัสขอดูบัตรพนักงานเจ้าหน้าที่แบบ Online
### Functional Requirements
1. ระบบจะต้องมีช่องทางให้ตั้งรหัสผ่านของ QR code ได้
2. ระบบจะต้องมี password policy
3. ระบบจะต้องมีการตรวจสอบ password ตาม password policy
4. ระบบจะต้องมีช่องทางให้ user แก้ไขรหัสผ่านได้
### Pre-conditions
- ก่อนที่จะตั้งรหัสผ่านของ QR code
	- user จะต้องเข้าสู่ระบบ
	- สถานะคำขอมีบัตรจะต้องอยู่ในสถานะ ตั้งรหัสผ่าน
	- user จะต้องได้รับการอนุมัติบัตรพนักงานเจ้าหน้าที่แล้ว
### Post-conditions
- ถ้า user
	- เข้าสู่ระบบ และ
	- ตั้งรหัสผ่านตาม password policy
- ระบบจะต้องบันทึกรหัสผ่านไว้ในฐานข้อมูล
### Alternate conditions
- xxx
### Exception conditions
- ถ้า user ตั้งรหัสผ่านไม่ถูกต้องตาม password policy ระบบจะต้องแจ้งเตือนไปยัง user และให้ user ตั้งรหัสผ่านใหม่
### Flow chart
- xxx