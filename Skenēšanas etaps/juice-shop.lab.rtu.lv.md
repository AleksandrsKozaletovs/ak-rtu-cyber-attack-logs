**Zenmap lietojumprogrammas rezultāts**
=======================================
```
Starting Nmap 7.95 ( https://nmap.org ) at 2025-05-20 22:44 EEST
NSE: Loaded 157 scripts for scanning.
NSE: Script Pre-scanning.
NSE: Starting runlevel 1 (of 3) scan.
Initiating NSE at 22:44
Completed NSE at 22:44, 0.00s elapsed
NSE: Starting runlevel 2 (of 3) scan.
Initiating NSE at 22:44
Completed NSE at 22:44, 0.00s elapsed
NSE: Starting runlevel 3 (of 3) scan.
Initiating NSE at 22:44
Completed NSE at 22:44, 0.00s elapsed
Initiating ARP Ping Scan at 22:44
Scanning 192.168.1.13 [1 port]
Completed ARP Ping Scan at 22:44, 0.06s elapsed (1 total hosts)
Initiating SYN Stealth Scan at 22:44
Scanning juice-shop.lab.rtu.lv (192.168.1.13) [1000 ports]
Discovered open port 3000/tcp on 192.168.1.13
Completed SYN Stealth Scan at 22:44, 0.12s elapsed (1000 total ports)
Initiating Service scan at 22:44
Scanning 1 service on juice-shop.lab.rtu.lv (192.168.1.13)
Warning: Hit PCRE_ERROR_MATCHLIMIT when probing for service http with the regex '^HTTP/1\.1 \d\d\d (?:[^\r\n]*\r\n(?!\r\n))*?.*\r\nServer: Virata-EmWeb/R([\d_]+)\r\nContent-Type: text/html; ?charset=UTF-8\r\nExpires: .*<title>HP (Color |)LaserJet ([\w._ -]+)&nbsp;&nbsp;&nbsp;'
Warning: Hit PCRE_ERROR_MATCHLIMIT when probing for service upnp with the regex '^HTTP/1\.1 \d\d\d (?:[^\r\n]*\r\n(?!\r\n))*?.*SERVER: Linux/([\w._+-]+), UPnP/([\d.]+), Intel UPnP SDK/([\w._~-]+)\r\n'
Warning: Hit PCRE_ERROR_MATCHLIMIT when probing for service http with the regex '^HTTP/1\.1 \d\d\d (?:[^\r\n]*\r\n(?!\r\n))*?.*\r\nServer: Virata-EmWeb/R([\d_]+)\r\nContent-Type: text/html; ?charset=UTF-8\r\nExpires: .*<title>HP (Color |)LaserJet ([\w._ -]+)&nbsp;&nbsp;&nbsp;'
Completed Service scan at 22:44, 11.26s elapsed (1 service on 1 host)
Initiating OS detection (try #1) against juice-shop.lab.rtu.lv (192.168.1.13)
NSE: Script scanning 192.168.1.13.
NSE: Starting runlevel 1 (of 3) scan.
Initiating NSE at 22:44
Completed NSE at 22:44, 0.02s elapsed
NSE: Starting runlevel 2 (of 3) scan.
Initiating NSE at 22:44
Completed NSE at 22:44, 1.00s elapsed
NSE: Starting runlevel 3 (of 3) scan.
Initiating NSE at 22:44
Completed NSE at 22:44, 0.00s elapsed
Nmap scan report for juice-shop.lab.rtu.lv (192.168.1.13)
Host is up, received arp-response (0.0012s latency).
Scanned at 2025-05-20 22:44:06 EEST for 14s
Not shown: 999 closed tcp ports (reset)
PORT     STATE SERVICE REASON         VERSION
3000/tcp open  ppp?    syn-ack ttl 64
| fingerprint-strings:
|   GetRequest:
|     HTTP/1.1 200 OK
|     Access-Control-Allow-Origin: *
|     X-Content-Type-Options: nosniff
|     X-Frame-Options: SAMEORIGIN
|     Feature-Policy: payment 'self'
|     X-Recruiting: /#/jobs
|     Accept-Ranges: bytes
|     Cache-Control: public, max-age=0
|     Last-Modified: Tue, 20 May 2025 16:56:20 GMT
|     ETag: W/"11708-196ee9feebe"
|     Content-Type: text/html; charset=UTF-8
|     Content-Length: 71432
|     Vary: Accept-Encoding
|     Date: Tue, 20 May 2025 19:44:17 GMT
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
|     <link id="favicon" rel="icon"
|   HTTPOptions, RTSPRequest:
|     HTTP/1.1 204 No Content
|     Access-Control-Allow-Origin: *
|     Access-Control-Allow-Methods: GET,HEAD,PUT,PATCH,POST,DELETE
|     Vary: Access-Control-Request-Headers
|     Content-Length: 0
|     Date: Tue, 20 May 2025 19:44:18 GMT
|     Connection: close
|   Help, NCP:
|     HTTP/1.1 400 Bad Request
|_    Connection: close
1 service unrecognized despite returning data. If you know the service/version, please submit the following fingerprint at https://nmap.org/cgi-bin/submit.cgi?new-service :
SF-Port3000-TCP:V=7.95%I=7%D=5/20%Time=682CDB91%P=x86_64-pc-linux-gnu%r(Ge
SF:tRequest,1C48,"HTTP/1\.1\x20200\x20OK\r\nAccess-Control-Allow-Origin:\x
SF:20\*\r\nX-Content-Type-Options:\x20nosniff\r\nX-Frame-Options:\x20SAMEO
SF:RIGIN\r\nFeature-Policy:\x20payment\x20'self'\r\nX-Recruiting:\x20/#/jo
SF:bs\r\nAccept-Ranges:\x20bytes\r\nCache-Control:\x20public,\x20max-age=0
SF:\r\nLast-Modified:\x20Tue,\x2020\x20May\x202025\x2016:56:20\x20GMT\r\nE
SF:Tag:\x20W/\"11708-196ee9feebe\"\r\nContent-Type:\x20text/html;\x20chars
SF:et=UTF-8\r\nContent-Length:\x2071432\r\nVary:\x20Accept-Encoding\r\nDat
SF:e:\x20Tue,\x2020\x20May\x202025\x2019:44:17\x20GMT\r\nConnection:\x20cl
SF:ose\r\n\r\n<!--\n\x20\x20~\x20Copyright\x20\(c\)\x202014-2025\x20Bjoern
SF:\x20Kimminich\x20&\x20the\x20OWASP\x20Juice\x20Shop\x20contributors\.\n
SF:\x20\x20~\x20SPDX-License-Identifier:\x20MIT\n\x20\x20-->\n\n<!doctype\
SF:x20html>\n<html\x20lang=\"en\"\x20data-critters-container>\n<head>\n\x2
SF:0\x20<meta\x20charset=\"utf-8\">\n\x20\x20<title>OWASP\x20Juice\x20Shop
SF:</title>\n\x20\x20<meta\x20name=\"description\"\x20content=\"Probably\x
SF:20the\x20most\x20modern\x20and\x20sophisticated\x20insecure\x20web\x20a
SF:pplication\">\n\x20\x20<meta\x20name=\"viewport\"\x20content=\"width=de
SF:vice-width,\x20initial-scale=1\">\n\x20\x20<link\x20id=\"favicon\"\x20r
SF:el=\"icon\"\x20")%r(Help,2F,"HTTP/1\.1\x20400\x20Bad\x20Request\r\nConn
SF:ection:\x20close\r\n\r\n")%r(NCP,2F,"HTTP/1\.1\x20400\x20Bad\x20Request
SF:\r\nConnection:\x20close\r\n\r\n")%r(HTTPOptions,EA,"HTTP/1\.1\x20204\x
SF:20No\x20Content\r\nAccess-Control-Allow-Origin:\x20\*\r\nAccess-Control
SF:-Allow-Methods:\x20GET,HEAD,PUT,PATCH,POST,DELETE\r\nVary:\x20Access-Co
SF:ntrol-Request-Headers\r\nContent-Length:\x200\r\nDate:\x20Tue,\x2020\x2
SF:0May\x202025\x2019:44:18\x20GMT\r\nConnection:\x20close\r\n\r\n")%r(RTS
SF:PRequest,EA,"HTTP/1\.1\x20204\x20No\x20Content\r\nAccess-Control-Allow-
SF:Origin:\x20\*\r\nAccess-Control-Allow-Methods:\x20GET,HEAD,PUT,PATCH,PO
SF:ST,DELETE\r\nVary:\x20Access-Control-Request-Headers\r\nContent-Length:
SF:\x200\r\nDate:\x20Tue,\x2020\x20May\x202025\x2019:44:18\x20GMT\r\nConne
SF:ction:\x20close\r\n\r\n");
MAC Address: 7A:19:F1:1B:94:54 (Unknown)
Device type: general purpose
Running: Linux 4.X|5.X
OS CPE: cpe:/o:linux:linux_kernel:4 cpe:/o:linux:linux_kernel:5
OS details: Linux 4.15 - 5.19
TCP/IP fingerprint:
OS:SCAN(V=7.95%E=4%D=5/20%OT=3000%CT=1%CU=44304%PV=Y%DS=1%DC=D%G=Y%M=7A19F1
OS:%TM=682CDB94%P=x86_64-pc-linux-gnu)SEQ(SP=FE%GCD=1%ISR=104%TI=Z%CI=Z%II=
OS:I%TS=A)OPS(O1=M5B4ST11NW7%O2=M5B4ST11NW7%O3=M5B4NNT11NW7%O4=M5B4ST11NW7%
OS:O5=M5B4ST11NW7%O6=M5B4ST11)WIN(W1=FE88%W2=FE88%W3=FE88%W4=FE88%W5=FE88%W
OS:6=FE88)ECN(R=Y%DF=Y%T=40%W=FAF0%O=M5B4NNSNW7%CC=Y%Q=)T1(R=Y%DF=Y%T=40%S=
OS:O%A=S+%F=AS%RD=0%Q=)T2(R=N)T3(R=N)T4(R=Y%DF=Y%T=40%W=0%S=A%A=Z%F=R%O=%RD
OS:=0%Q=)T5(R=Y%DF=Y%T=40%W=0%S=Z%A=S+%F=AR%O=%RD=0%Q=)T6(R=Y%DF=Y%T=40%W=0
OS:%S=A%A=Z%F=R%O=%RD=0%Q=)T7(R=Y%DF=Y%T=40%W=0%S=Z%A=S+%F=AR%O=%RD=0%Q=)U1
OS:(R=Y%DF=N%T=40%IPL=164%UN=0%RIPL=G%RID=G%RIPCK=G%RUCK=G%RUD=G)IE(R=Y%DFI
OS:=N%T=40%CD=S)

Uptime guess: 46.380 days (since Fri Apr  4 13:37:24 2025)
Network Distance: 1 hop
TCP Sequence Prediction: Difficulty=254 (Good luck!)
IP ID Sequence Generation: All zeros

TRACEROUTE
HOP RTT     ADDRESS
1   1.16 ms juice-shop.lab.rtu.lv (192.168.1.13)

NSE: Script Post-scanning.
NSE: Starting runlevel 1 (of 3) scan.
Initiating NSE at 22:44
Completed NSE at 22:44, 0.00s elapsed
NSE: Starting runlevel 2 (of 3) scan.
Initiating NSE at 22:44
Completed NSE at 22:44, 0.00s elapsed
NSE: Starting runlevel 3 (of 3) scan.
Initiating NSE at 22:44
Completed NSE at 22:44, 0.00s elapsed
Read data files from: /usr/share/nmap
OS and Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
Nmap done: 1 IP address (1 host up) scanned in 14.06 seconds
           Raw packets sent: 1023 (45.806KB) | Rcvd: 1015 (41.282KB)

```
