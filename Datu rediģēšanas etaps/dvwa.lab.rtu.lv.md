**Datu izgūšana no dvwa.lab.rtu.lv tīmekļa vietnes ar pingu komandu** 
```
PING 192.168.1.12 (192.168.1.12): 56 data bytes
64 bytes from 192.168.1.12: icmp_seq=0 ttl=64 time=0.051 ms
64 bytes from 192.168.1.12: icmp_seq=1 ttl=64 time=0.068 ms
64 bytes from 192.168.1.12: icmp_seq=2 ttl=64 time=0.074 ms
64 bytes from 192.168.1.12: icmp_seq=3 ttl=64 time=0.086 ms
--- 192.168.1.12 ping statistics ---
4 packets transmitted, 4 packets received, 0% packet loss
round-trip min/avg/max/stddev = 0.051/0.070/0.086/0.000 ms
total 20
drwxrwxr-x  4 root root 4096 Jan  4  2017 .
drwxrwxr-x 12 root root 4096 Jan  4  2017 ..
drwxrwxr-x  2 root root 4096 Jan  4  2017 help
-rw-rw-r--  1 root root 1830 Jan  4  2017 index.php
drwxrwxr-x  2 root root 4096 Jan  4  2017 source
www-data
www-data
/var/www/html/vulnerabilities/exec

```

**Failu meklēšana, kurus www-data lietotājs spēj rediģēt**
```
PING 192.168.1.12 (192.168.1.12): 56 data bytes
64 bytes from 192.168.1.12: icmp_seq=0 ttl=64 time=0.097 ms
64 bytes from 192.168.1.12: icmp_seq=1 ttl=64 time=0.066 ms
64 bytes from 192.168.1.12: icmp_seq=2 ttl=64 time=0.072 ms
64 bytes from 192.168.1.12: icmp_seq=3 ttl=64 time=0.065 ms
--- 192.168.1.12 ping statistics ---
4 packets transmitted, 4 packets received, 0% packet loss
round-trip min/avg/max/stddev = 0.065/0.075/0.097/0.000 ms
/var/cache/apache2/mod_cache_disk
/var/www/html (visi faili html mapē)
```
**Failu rediģēšanas rezultāts**

```php
        <!-- <img src=\"" . DVWA_WEB_PAGE_TO_ROOT . "dvwa/images/RandomStorm.png\" /> -->
        </div > <!--<div id=\"content\">-->

        <div id=\"footer\">

        <p>" . dvwaExternalLinkUrlGet( 'http://www.dvwa.co.uk/', 'Damn Vulnerable Web Application (DVWA)' ) . "</p>

        </div> <!--<div id=\"footer\"> -->

        </div> <!--<div id=\"wrapper\"> -->

        </body>

</html>";

?>
Kiberdrosibas tests

```
![image](https://github.com/user-attachments/assets/180f98aa-3aed-4deb-8b34-c64d9cdecda5)


**Failu dzēšanas process**
* Pirms komandu izpildīšanas (html mapēs saturs) *
```
root@6ead2f4de120:/var/cache/apache2/mod_cache_disk# ls -al /var/www/html
total 180
drwxrwxrwx 1 www-data www-data  4096 Mar 20  2017 .
drwxr-xr-x 1 root     root      4096 Mar 20  2017 ..
-rw-rw-r-- 1 www-data www-data   500 Jan  4  2017 .htaccess
-rw-rw-r-- 1 www-data www-data  7296 Jan  4  2017 CHANGELOG.md
-rw-rw-r-- 1 www-data www-data 33107 Jan  4  2017 COPYING.txt
-rw-rw-r-- 1 www-data www-data  7805 Jan  4  2017 README.md
-rw-rw-r-- 1 www-data www-data  3798 Jan  4  2017 about.php
drwxrwxr-x 1 www-data www-data  4096 Mar 20  2017 config
drwxrwxr-x 1 www-data www-data  4096 Jan  4  2017 docs
drwxrwxr-x 1 www-data www-data  4096 Jan  4  2017 dvwa
drwxrwxr-x 1 www-data www-data  4096 Mar 20  2017 external
-rw-rw-r-- 1 www-data www-data  1406 Jan  4  2017 favicon.ico
drwxrwxr-x 1 www-data www-data  4096 Mar 20  2017 hackable
-rw-rw-r-- 1 www-data www-data   895 Jan  4  2017 ids_log.php
-rw-rw-r-- 1 www-data www-data  4389 Jan  4  2017 index.php
-rw-rw-r-- 1 www-data www-data  1869 Jan  4  2017 instructions.php
-rw-rw-r-- 1 www-data www-data  4183 May 23 18:36 login.php
-rw-rw-r-- 1 www-data www-data   414 Jan  4  2017 logout.php
-rw-rw-r-- 1 www-data www-data   148 Jan  4  2017 php.ini
-rw-rw-r-- 1 www-data www-data   199 Jan  4  2017 phpinfo.php
-rw-rw-r-- 1 www-data www-data    26 Jan  4  2017 robots.txt
-rw-rw-r-- 1 www-data www-data  4686 Jan  4  2017 security.php
-rw-rw-r-- 1 www-data www-data  2551 Jan  4  2017 setup.php
drwxrwxr-x 1 www-data www-data  4096 Jan  4  2017 vulnerabilities
```
* Pēc komandu izpildīšanas (html mapēs saturs) *

```
root@6ead2f4de120:/var/www/html# ls -al
total 16
drwxrwxrwx 1 www-data www-data 4096 May 23 18:48 .
drwxr-xr-x 1 root     root     4096 Mar 20  2017 ..
```

![image](https://github.com/user-attachments/assets/6d0e577e-af1a-43ef-a9e3-024d5ff5cdef)
