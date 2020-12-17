# ใช้สำหรับ Remove file ที่มีการ Create มากกว่า 7 วันขึ้นไป
~~~
#!/bin/sh
find /mnt/backup7day/ECCF/* /mnt/backup7day/dict/* /mnt/backup7day/cifsdata/* /mnt/backup7day/globalimagestorage/* -mmin +9660 -exec rm -f {} \;
~~~

# ใช้สำหรับ Remove file ที่มีการ Create มากกว่า 7 วันขึ้นไปเหมือนกัน แต่ใช้กันแล้วแต่กรณั
~~~
#!/bin/sh
find /mnt/backup7day/ECCF/* /mnt/backup7day/dict/* /mnt/backup7day/cifsdata/* /mnt/backup7day/globalimagestorage/* -time +6 -exec rm -f {} \;
~~~
