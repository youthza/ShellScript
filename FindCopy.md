# ใช้สำหรับ ค้นหาไฟล์ โดยกำหนดให้นับจากวันล่าสุดที่ทำการ create แล้วจึงทำการ Copy
~~~
#!/bin/sh
find SOURCE_PATH -mtime -1 -exec cp -f {} DESTINATION_PATH \;
~~~
