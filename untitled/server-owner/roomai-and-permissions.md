# RoomAI and Permissions

## เปิดและปิดห้อง AI

| คำสั่ง         | ใช้ทำอะไร                                |
| -------------- | ---------------------------------------- |
| `/setroomai`   | เปิด Hana AI ในห้องปัจจุบัน              |
| `/unsetroomai` | ปิด Hana AI ในห้องปัจจุบัน               |
| `/guildbook`   | เปิดคู่มือใช้งานใน Discord               |
| `/hanacontext` | ตั้งข้อมูลหรือกฎของเซิร์ฟเวอร์ (Premium) |

คำสั่งเปิด/ปิดห้อง AI ใช้สำหรับผู้ดูแลเซิร์ฟเวอร์

## สิทธิ์ที่แนะนำ

Hana ไม่จำเป็นต้องเป็น Administrator หากเปิดเฉพาะสิทธิ์ที่ต้องใช้:

* View Channel
* Send Messages
* Read Message History
* Embed Links
* Attach Files
* Use Application Commands
* Send Messages in Threads หากห้องใช้งาน Thread

## เมื่อ Hana ไม่ตอบ

{% stepper %}
{% step %}
## ตรวจสอบการเปิดใช้งานห้อง

ห้องนั้นเปิดด้วย `/setroomai` แล้วหรือไม่
{% endstep %}

{% step %}
## ตรวจสอบสิทธิ์ของ Hana

Hana มองเห็นและส่งข้อความในห้องได้หรือไม่
{% endstep %}

{% step %}
## ตรวจสอบ Channel Override หรือ Thread

มีการ deny สิทธิ์ใน Channel Override หรือ Thread หรือไม่
{% endstep %}

{% step %}
## ตรวจสอบภาษา

ข้อความเป็นภาษาไทย อังกฤษ หรือญี่ปุ่นหรือไม่
{% endstep %}

{% step %}
## ตรวจสอบสถานะระบบ AI

ระบบ AI กำลังคิวเต็มหรือ API ตอบช้าชั่วคราวหรือไม่
{% endstep %}
{% endstepper %}

## เมื่อรูปไม่ขึ้น

คำสั่ง `/travelphoto` ต้องมี `Embed Links` หากสิทธิ์นี้ถูกปิด Discord จะไม่อนุญาตให้ Hana แนบภาพ
