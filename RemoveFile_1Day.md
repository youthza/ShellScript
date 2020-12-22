# ใช้สำหรับ Remove file ที่ทำการ Create มากกว่า 1 วัน
~~~
#!/bin/sh
find SOURCE_PATH DESTINATION_PATH -mmin +1020 -exec rm -f {} 
~~~

# ใช้สำหรับ Remove file ที่ทำการ Create มากกว่า 1 วันเหมือนกัน แต่ใช้งานแล้วแต่กรณี
~~~
#!/bin/sh
find SOURCE_PATH DESTINATION_PATH -mtime -1 -exec rm -f {} 
~~~

