# ใช้สำหรับ copy file เป็น .Tar 
## โดยกำหนดการ Backup มาในรูปแบบ Timedate ล่าสุด แล้วตามด้วยชื่อไฟล์ ECCF.tar
~~~
#!/bin/sh
zone=$(date +'%Y%m%d')
tar -cvf destination path${zone}ECCF.tar source path
~~~
