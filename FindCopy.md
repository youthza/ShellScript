# ใช้สำหรับ ค้นหาไฟล์ โดยกำหนดให้นับจากวันล่าสุดที่ทำการ create แล้วจึงทำการ Copy
~~~
#!/bin/sh
find source path -mtime -1 -exec cp -f {} destination path \;
~~~
