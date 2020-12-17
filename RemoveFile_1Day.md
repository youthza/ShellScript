# ใช้สำหรับ Remove ไฟล์ล่าสุด โดยนับจาก นาทีที่ทำการ Create
~~~
#!/bin/sh
find source path destination path -mmin +1020 -exec rm -f {} 
~~~

# เป็นคำสั่งที่ใช้ Remove ไฟล์ล่าสุดเหมือนกัน แต่ใช้กันคนละกรณี
~~~
#!/bin/sh
find source path destination path -mtime -1 -exec rm -f {} 
~~~

