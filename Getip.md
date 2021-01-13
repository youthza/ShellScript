# การ Set ให้แสดงเฉพาะ Ip
~~~
#!/bin/sh
netstat -anpt |grep 22 |grep ESTABLISHED | awk '{ print $5 }' | cut -d: -f1 | sort -u
~~~
