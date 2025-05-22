**metasploitable.lab.rtu.lv ierīces parbaude pēc uzbrukuma**
```
root@b2bd6545425e:~# ls -al /var/log/apache2/
total 32
drwxr-x--- 1 root adm  4096 May 22 16:31 .
drwxr-xr-x 1 root root 4096 Jan 27  2018 ..
-rw-r--r-- 1 root root 8950 May 22 11:46 access.log
-rw-r----- 1 root adm  3530 May 22 11:46 error.log
root@b2bd6545425e:~#
```

**metasploit-framework termināla izvade**
```
ls /var/log/apache2/
access.log
error.log
error.log.1
rm /var/log/apache2/error.log.1
ls var/log/apache2
access.log
error.log
```
