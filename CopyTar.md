# ใช้สำหรับ copy file เป็น .Tar 
## โดยกำหนดการ Backup มาในรูปแบบ Timedate ล่าสุด แล้วตามด้วยชื่อไฟล์ ECCF.tar
~~~
#!/bin/sh
zone=$(date +'%Y%m%d')
tar -cvf DESTINATION_PATH${zone}ECCF.tar SOURCE_PATH
~~~
