# Introduction
สวัสดีครับ กลุ่ม POS System เราได้สร้าง โปรแกรมที่นำไปใช้กับเครื่องคิดเงิน (หรือที่เรียกว่า ระบบ POS) อย่างเต็มรูปแบบ โดยการใช้เพียง ภาษา C ในการเขียน 100%

สำหรับวิธีการใช้งานอย่างละเอียด สามารถเข้าไปดูได้ที่ : [https://github.com/sagelga/ComPro_Project/wiki](https://github.com/sagelga/ComPro_Project/wiki/)

***

# How to use
สำหรับวิธีการใช้งาน ให้ไปที่โฟล์เดอร์หลัก แล้วพิมพ์
`make && make run`
เพื่อเป็นการ Compile ไฟล์ภาษา .c และ .h (C Header file) หลายไฟล์เข้าด้วยกัน โดยหากทำผ่านแล้ว จะขื้นเป็นหน้า Interface ที่มีการให้ปรับขนาดหน้าจอ

## Optimized Device Configurations
โปรแกรมของเรา จะรันได้อย่างราบรื่นมากที่สุดโดยการใช้ระบบปฏิบัติการ MacOS (OSX) แต่ยังใช้งานได้กับระบบอื่นๆ เช่น Ubuntu Linux

สำหรับการตั้งขนาด Terminal เป็นค่าแนะนำ เนื่องจากข้อมูลเรามีมาก **เราจึงแนะนำให้ใช้ความกว้างหน้าจอขนาด 140 pixel และยาว 40 pixel** ผู้้ใช้สามารถเลือกใช้ขนาดที่ใหญ่กว่าขนาดที่ได้แนะนำไว้ได้ แต่ไม่สำหรับขนาดความละเอียดที่น้อยกว่านี้

***

# Into the core
ก่อนที่จะใช้งานระบบ POS ลูกค้าจำเป็นที่จะต้อง login เพื่อจะเข้าระบบเสียก่อน โดยการเข้าระบบจากหน้าแรก (หน้าปรับขนาดหน้าจอ)​ 
1. ให้กด 'Y' แล้วกด ENTER
2. พิมพ์ username (หรือใช้ scanner เช่นตัวยิงบาร์โค้ด) เข้าไปที่ระบบ
3. พิมพ์ password ของผู้ใช้งาน (user) นั้น
4. ระบบจะเช็คหาถึงความถูกต้องของ username / password และนำผู้ใช้ไปที่หน้่าหลัก

## Features
สำหรับการใช้งานระบบ POS ก็จะมีระบบย่อยๆ ต่างๆ เพื่อช่วยในการขาย เช่น
* เช็คสินค้าคงคลัง (Inventory)
* เช็คถึงยอดขาย (Sales)
* เช็คถึงยอดขายในอนาคต (Forecast)
* เช็คผู้ใช้งานอื่น (Personnel)
* เช็คประเภทของสินค้า (Category)
* เปลี่ยนระบบโปรโมชั่นสำหรับลูกค้า (Promotion)
* แก้ไขข้อมูลพื้นฐานของร้านค้า (Settings)

โดยทุกระบบที่ได้เกล่ามานั้น ผู้ใช้งานที่เป็น admin สามารถเข้าไปปรับแก้ได้ทั้งหมด และ**สามารถเปลี่ยน/เพื่ม/ลด ได้ตลอดเวลา**

***

# How to use POS Sales System
วิธีการใช้หน้า POS System
1. กรอก Customer ID (หากมี) เพื่อเป็นการเก็บข้อมูลของลูกค้าคนนั้นๆ
2. เรี่มใช้งานโดยการกรอก Barcode หรือใช้ barcode scanner ในการสแกนสินค้า
(หากสินค้าที่สแกน ไม่ได้อยู่ในระบบ หรือของในคลงคลัง (Inventory) หมด ระบบจะไม่เพื่มข้อมูล และแจ้งว่าสินค้านั้นไม่อยู่ในระบบ
3. เมื่อสแกนสินค้่าเสร็จเรียบร้อยแล้ว ให้กด ENTER
4. หากลูกค้าอยากใช้คะแนนเป็นส่วนลด หรือใช้ Voucher เงินสด ก็สามารถสแกนเข้่าไปได้ในขั้นตอนนี้
5. ยอดการใช้จ่ายใหม่ และ ยอดคะแนนใหม่ จะถูกแสดงในขั้นตอนนี้ หากคิดเงินเสร็จเรียบร้อยแล้ว ก็สามารถกด ENTER และเรื่มขั้นตอนใหม่่ได้

***

# Contributors
ลำดับที่|ชื่อ|นามสกุล|GitHub Username|รหัสนักศึกษา
-|-|-|-|-
1|Kunanon|Srisuntiroj|@sagelga|59070022
2|Thanawat|Laodkaew|@skydddoogg|59070071
3|Noppanut|Ploywong|@noppanut15|59070082
4|Vasanchai|Prakobkij|@59070156|59070156
5|Weerakorn|Pongpum|@fablemay|59070163

## Status Check
Master|Development
-|-
[![Build Status](https://travis-ci.com/sagelga/ComPro_Project.svg?token=hxfRmfpCpbnunWcyMpkC&branch=master)](https://travis-ci.com/sagelga/ComPro_Project)|[![Build Status](https://travis-ci.com/sagelga/ComPro_Project.svg?token=hxfRmfpCpbnunWcyMpkC&branch=development)](https://travis-ci.com/sagelga/ComPro_Project)

