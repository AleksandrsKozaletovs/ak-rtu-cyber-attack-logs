**Zenmap lietojumprogrammas rezultāts**
=======================================
```
Starting Nmap 7.95 ( https://nmap.org ) at 2025-05-17 21:11 EEST
NSE: Loaded 157 scripts for scanning.
NSE: Script Pre-scanning.
NSE: Starting runlevel 1 (of 3) scan.
Initiating NSE at 21:11
Completed NSE at 21:11, 0.00s elapsed
NSE: Starting runlevel 2 (of 3) scan.
Initiating NSE at 21:11
Completed NSE at 21:11, 0.00s elapsed
NSE: Starting runlevel 3 (of 3) scan.
Initiating NSE at 21:11
Completed NSE at 21:11, 0.00s elapsed
Initiating ARP Ping Scan at 21:11
Scanning 192.168.1.200 [1 port]
Completed ARP Ping Scan at 21:11, 0.05s elapsed (1 total hosts)
Initiating SYN Stealth Scan at 21:11
Scanning 192.168.1.200 [1000 ports]
Discovered open port 22/tcp on 192.168.1.200
Discovered open port 80/tcp on 192.168.1.200
Discovered open port 8082/tcp on 192.168.1.200
Discovered open port 8081/tcp on 192.168.1.200
Discovered open port 8083/tcp on 192.168.1.200
Discovered open port 8084/tcp on 192.168.1.200
Completed SYN Stealth Scan at 21:11, 0.08s elapsed (1000 total ports)
Initiating Service scan at 21:11
Scanning 6 services on 192.168.1.200
Warning: Hit PCRE_ERROR_MATCHLIMIT when probing for service http with the regex '^HTTP/1\.1 \d\d\d (?:[^\r\n]*\r\n(?!\r\n))*?.*\r\nServer: Virata-EmWeb/R([\d_]+)\r\nContent-Type: text/html; ?charset=UTF-8\r\nExpires: .*<title>HP (Color |)LaserJet ([\w._ -]+)&nbsp;&nbsp;&nbsp;'
Warning: Hit PCRE_ERROR_MATCHLIMIT when probing for service upnp with the regex '^HTTP/1\.1 \d\d\d (?:[^\r\n]*\r\n(?!\r\n))*?.*SERVER: Linux/([\w._+-]+), UPnP/([\d.]+), Intel UPnP SDK/([\w._~-]+)\r\n'
Warning: Hit PCRE_ERROR_MATCHLIMIT when probing for service http with the regex '^HTTP/1\.1 \d\d\d (?:[^\r\n]*\r\n(?!\r\n))*?.*\r\nServer: Virata-EmWeb/R([\d_]+)\r\nContent-Type: text/html; ?charset=UTF-8\r\nExpires: .*<title>HP (Color |)LaserJet ([\w._ -]+)&nbsp;&nbsp;&nbsp;'
Warning: Hit PCRE_ERROR_MATCHLIMIT when probing for service http with the regex '^HTTP/1\.[01] \d\d\d.*\r\nDate: .*\r\nServer: Apache-AdvancedExtranetServer\r\n'
Warning: Hit PCRE_ERROR_MATCHLIMIT when probing for service http with the regex '^HTTP/1\.1 \d\d\d .*\nDate: .*\r\nConnection: close\r\nServer: Clearswift\r\n\r\n'
Completed Service scan at 21:12, 11.30s elapsed (6 services on 1 host)
Initiating OS detection (try #1) against 192.168.1.200
NSE: Script scanning 192.168.1.200.
NSE: Starting runlevel 1 (of 3) scan.
Initiating NSE at 21:12
Completed NSE at 21:12, 1.11s elapsed
NSE: Starting runlevel 2 (of 3) scan.
Initiating NSE at 21:12
Completed NSE at 21:12, 1.01s elapsed
NSE: Starting runlevel 3 (of 3) scan.
Initiating NSE at 21:12
Completed NSE at 21:12, 0.00s elapsed
Nmap scan report for 192.168.1.200
Host is up, received arp-response (0.00068s latency).
Scanned at 2025-05-17 21:11:49 EEST for 15s
Not shown: 994 closed tcp ports (reset)
PORT     STATE SERVICE REASON         VERSION
22/tcp   open  ssh     syn-ack ttl 64 OpenSSH 9.6p1 Ubuntu 3ubuntu13.11 (Ubuntu Linux; protocol 2.0)
| ssh-hostkey:
|   256 86:7f:49:a6:47:da:ec:27:94:91:6c:51:88:5c:82:ea (ECDSA)
| ecdsa-sha2-nistp256 AAAAE2VjZHNhLXNoYTItbmlzdHAyNTYAAAAIbmlzdHAyNTYAAABBBMPXlTC74ejuZOg1wtv6q4rbIvqyAzku6YxJer6+XN+//Ktk0pO+EITASultG50UQ8lAGfgWMdvVGoNr4WfJ2Bc=
|   256 bd:c0:33:cd:b6:09:91:c9:26:95:fd:77:2c:cc:fc:c7 (ED25519)
|_ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAID0Ss4hStlD/xxyUHcu0NuhkKYtnIBwKLhwW6esAz1EC
80/tcp   open  http    syn-ack ttl 63 nginx
| http-methods:
|_  Supported Methods: GET HEAD POST OPTIONS
|_http-cors: HEAD GET POST PUT DELETE PATCH
| http-robots.txt: 1 disallowed entry
|_/ftp
|_http-title: OWASP Juice Shop
|_http-favicon: Unknown favicon MD5: 60593CEDA42482E579C25193BD7EC6E1
8081/tcp open  http    syn-ack ttl 63 Apache httpd 2.2.8 ((Ubuntu) DAV/2)
|_http-server-header: Apache/2.2.8 (Ubuntu) DAV/2
| http-methods:
|_  Supported Methods: GET HEAD POST OPTIONS
|_http-title: Metasploitable2 - Linux
8082/tcp open  http    syn-ack ttl 63 Apache httpd 2.4.10 ((Debian))
| http-title: Login :: Damn Vulnerable Web Application (DVWA) v1.10 *Develop...
|_Requested resource was login.php
|_http-server-header: Apache/2.4.10 (Debian)
| http-robots.txt: 1 disallowed entry
|_/
| http-cookie-flags:
|   /:
|     PHPSESSID:
|_      httponly flag not set
|_http-favicon: Unknown favicon MD5: 69C728902A3F1DF75CF9EAC73BD55556
| http-methods:
|_  Supported Methods: GET HEAD POST OPTIONS
8083/tcp open  us-srv? syn-ack ttl 63
| fingerprint-strings:
|   FourOhFourRequest, GetRequest:
|     HTTP/1.1 200 OK
|     Access-Control-Allow-Origin: *
|     X-Content-Type-Options: nosniff
|     X-Frame-Options: SAMEORIGIN
|     Feature-Policy: payment 'self'
|     X-Recruiting: /#/jobs
|     Accept-Ranges: bytes
|     Cache-Control: public, max-age=0
|     Last-Modified: Sat, 17 May 2025 14:54:21 GMT
|     ETag: W/"11708-196debd2c49"
|     Content-Type: text/html; charset=UTF-8
|     Content-Length: 71432
|     Vary: Accept-Encoding
|     Date: Sat, 17 May 2025 18:11:55 GMT
|     Connection: close
|     <!--
|     Copyright (c) 2014-2025 Bjoern Kimminich & the OWASP Juice Shop contributors.
|     SPDX-License-Identifier: MIT
|     <!doctype html>
|     <html lang="en" data-critters-container>
|     <head>
|     <meta charset="utf-8">
|     <title>OWASP Juice Shop</title>
|     <meta name="description" content="Probably the most modern and sophisticated insecure web application">
|     <meta name="viewport" content="width=device-width, initial-scale=1">
|_    <link id="favicon" rel="icon"
8084/tcp open  http    syn-ack ttl 63 Apache httpd 2.4.7 ((Ubuntu))
| http-robots.txt: 5 disallowed entries
|_/ /admin/ /documents/ /images/ /passwords/
| http-methods:
|_  Supported Methods: GET HEAD POST OPTIONS
| http-title: Site doesn't have a title (text/html).
|_Requested resource was login.php
|_http-server-header: Apache/2.4.7 (Ubuntu)
1 service unrecognized despite returning data. If you know the service/version, please submit the following fingerprint at https://nmap.org/cgi-bin/submit.cgi?new-service :
SF-Port8083-TCP:V=7.95%I=7%D=5/17%Time=6828D16B%P=x86_64-pc-linux-gnu%r(Ge
SF:tRequest,3890,"HTTP/1\.1\x20200\x20OK\r\nAccess-Control-Allow-Origin:\x
SF:20\*\r\nX-Content-Type-Options:\x20nosniff\r\nX-Frame-Options:\x20SAMEO
SF:RIGIN\r\nFeature-Policy:\x20payment\x20'self'\r\nX-Recruiting:\x20/#/jo
SF:bs\r\nAccept-Ranges:\x20bytes\r\nCache-Control:\x20public,\x20max-age=0
SF:\r\nLast-Modified:\x20Sat,\x2017\x20May\x202025\x2014:54:21\x20GMT\r\nE
SF:Tag:\x20W/\"11708-196debd2c49\"\r\nContent-Type:\x20text/html;\x20chars
SF:et=UTF-8\r\nContent-Length:\x2071432\r\nVary:\x20Accept-Encoding\r\nDat
SF:e:\x20Sat,\x2017\x20May\x202025\x2018:11:55\x20GMT\r\nConnection:\x20cl
SF:ose\r\n\r\n<!--\n\x20\x20~\x20Copyright\x20\(c\)\x202014-2025\x20Bjoern
SF:\x20Kimminich\x20&\x20the\x20OWASP\x20Juice\x20Shop\x20contributors\.\n
SF:\x20\x20~\x20SPDX-License-Identifier:\x20MIT\n\x20\x20-->\n\n<!doctype\
SF:x20html>\n<html\x20lang=\"en\"\x20data-critters-container>\n<head>\n\x2
SF:0\x20<meta\x20charset=\"utf-8\">\n\x20\x20<title>OWASP\x20Juice\x20Shop
SF:</title>\n\x20\x20<meta\x20name=\"description\"\x20content=\"Probably\x
SF:20the\x20most\x20modern\x20and\x20sophisticated\x20insecure\x20web\x20a
SF:pplication\">\n\x20\x20<meta\x20name=\"viewport\"\x20content=\"width=de
SF:vice-width,\x20initial-scale=1\">\n\x20\x20<link\x20id=\"favicon\"\x20r
SF:el=\"icon\"\x20")%r(FourOhFourRequest,118C1,"HTTP/1\.1\x20200\x20OK\r\n
SF:Access-Control-Allow-Origin:\x20\*\r\nX-Content-Type-Options:\x20nosnif
SF:f\r\nX-Frame-Options:\x20SAMEORIGIN\r\nFeature-Policy:\x20payment\x20's
SF:elf'\r\nX-Recruiting:\x20/#/jobs\r\nAccept-Ranges:\x20bytes\r\nCache-Co
SF:ntrol:\x20public,\x20max-age=0\r\nLast-Modified:\x20Sat,\x2017\x20May\x
SF:202025\x2014:54:21\x20GMT\r\nETag:\x20W/\"11708-196debd2c49\"\r\nConten
SF:t-Type:\x20text/html;\x20charset=UTF-8\r\nContent-Length:\x2071432\r\nV
SF:ary:\x20Accept-Encoding\r\nDate:\x20Sat,\x2017\x20May\x202025\x2018:11:
SF:55\x20GMT\r\nConnection:\x20close\r\n\r\n<!--\n\x20\x20~\x20Copyright\x
SF:20\(c\)\x202014-2025\x20Bjoern\x20Kimminich\x20&\x20the\x20OWASP\x20Jui
SF:ce\x20Shop\x20contributors\.\n\x20\x20~\x20SPDX-License-Identifier:\x20
SF:MIT\n\x20\x20-->\n\n<!doctype\x20html>\n<html\x20lang=\"en\"\x20data-cr
SF:itters-container>\n<head>\n\x20\x20<meta\x20charset=\"utf-8\">\n\x20\x2
SF:0<title>OWASP\x20Juice\x20Shop</title>\n\x20\x20<meta\x20name=\"descrip
SF:tion\"\x20content=\"Probably\x20the\x20most\x20modern\x20and\x20sophist
SF:icated\x20insecure\x20web\x20application\">\n\x20\x20<meta\x20name=\"vi
SF:ewport\"\x20content=\"width=device-width,\x20initial-scale=1\">\n\x20\x
SF:20<link\x20id=\"favicon\"\x20rel=\"icon\"\x20");
MAC Address: 00:0C:29:73:1A:30 (VMware)
Device type: general purpose|router
Running: Linux 4.X|5.X, MikroTik RouterOS 7.X
OS CPE: cpe:/o:linux:linux_kernel:4 cpe:/o:linux:linux_kernel:5 cpe:/o:mikrotik:routeros:7 cpe:/o:linux:linux_kernel:5.6.3
OS details: Linux 4.15 - 5.19, OpenWrt 21.02 (Linux 5.4), MikroTik RouterOS 7.2 - 7.5 (Linux 5.6.3)
TCP/IP fingerprint:
OS:SCAN(V=7.95%E=4%D=5/17%OT=22%CT=1%CU=33071%PV=Y%DS=1%DC=D%G=Y%M=000C29%T
OS:M=6828D174%P=x86_64-pc-linux-gnu)SEQ(SP=107%GCD=1%ISR=10C%TI=Z%CI=Z%II=I
OS:%TS=A)OPS(O1=M5B4ST11NW7%O2=M5B4ST11NW7%O3=M5B4NNT11NW7%O4=M5B4ST11NW7%O
OS:5=M5B4ST11NW7%O6=M5B4ST11)WIN(W1=FE88%W2=FE88%W3=FE88%W4=FE88%W5=FE88%W6
OS:=FE88)ECN(R=Y%DF=Y%T=40%W=FAF0%O=M5B4NNSNW7%CC=Y%Q=)T1(R=Y%DF=Y%T=40%S=O
OS:%A=S+%F=AS%RD=0%Q=)T2(R=N)T3(R=N)T4(R=Y%DF=Y%T=40%W=0%S=A%A=Z%F=R%O=%RD=
OS:0%Q=)T5(R=Y%DF=Y%T=40%W=0%S=Z%A=S+%F=AR%O=%RD=0%Q=)T6(R=Y%DF=Y%T=40%W=0%
OS:S=A%A=Z%F=R%O=%RD=0%Q=)T7(R=Y%DF=Y%T=40%W=0%S=Z%A=S+%F=AR%O=%RD=0%Q=)U1(
OS:R=Y%DF=N%T=40%IPL=164%UN=0%RIPL=G%RID=G%RIPCK=G%RUCK=G%RUD=G)IE(R=Y%DFI=
OS:N%T=40%CD=S)

Uptime guess: 36.052 days (since Fri Apr 11 19:57:50 2025)
Network Distance: 1 hop
TCP Sequence Prediction: Difficulty=263 (Good luck!)
IP ID Sequence Generation: All zeros
Service Info: OS: Linux; CPE: cpe:/o:linux:linux_kernel

TRACEROUTE
HOP RTT     ADDRESS
1   0.68 ms 192.168.1.200

NSE: Script Post-scanning.
NSE: Starting runlevel 1 (of 3) scan.
Initiating NSE at 21:12
Completed NSE at 21:12, 0.00s elapsed
NSE: Starting runlevel 2 (of 3) scan.
Initiating NSE at 21:12
Completed NSE at 21:12, 0.00s elapsed
NSE: Starting runlevel 3 (of 3) scan.
Initiating NSE at 21:12
Completed NSE at 21:12, 0.00s elapsed
Read data files from: /usr/share/nmap
OS and Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
Nmap done: 1 IP address (1 host up) scanned in 15.16 seconds
           Raw packets sent: 1023 (45.806KB) | Rcvd: 1015 (41.302KB)

```
