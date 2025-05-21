**Zenmap lietojumprogrammas rezultāts**
=======================================
```
Starting Nmap 7.95 ( https://nmap.org ) at 2025-05-21 23:55 EEST
NSE: Loaded 157 scripts for scanning.
NSE: Script Pre-scanning.
NSE: Starting runlevel 1 (of 3) scan.
Initiating NSE at 23:55
Completed NSE at 23:55, 0.00s elapsed
NSE: Starting runlevel 2 (of 3) scan.
Initiating NSE at 23:55
Completed NSE at 23:55, 0.00s elapsed
NSE: Starting runlevel 3 (of 3) scan.
Initiating NSE at 23:55
Completed NSE at 23:55, 0.00s elapsed
Initiating ARP Ping Scan at 23:55
Scanning 192.168.1.13 [1 port]
Completed ARP Ping Scan at 23:55, 0.05s elapsed (1 total hosts)
Initiating SYN Stealth Scan at 23:55
Scanning juice-shop.lab.rtu.lv (192.168.1.13) [1000 ports]
Discovered open port 3000/tcp on 192.168.1.13
Completed SYN Stealth Scan at 23:55, 0.10s elapsed (1000 total ports)
Initiating Service scan at 23:55
Scanning 1 service on juice-shop.lab.rtu.lv (192.168.1.13)
Warning: Hit PCRE_ERROR_MATCHLIMIT when probing for service http with the regex                                              '^HTTP/1\.1 \d\d\d (?:[^\r\n]*\r\n(?!\r\n))*?.*\r\nServer: Virata-EmWeb/R([\d_]+                                             )\r\nContent-Type: text/html; ?charset=UTF-8\r\nExpires: .*<title>HP (Color |)La                                             serJet ([\w._ -]+)&nbsp;&nbsp;&nbsp;'
Warning: Hit PCRE_ERROR_MATCHLIMIT when probing for service upnp with the regex                                              '^HTTP/1\.1 \d\d\d (?:[^\r\n]*\r\n(?!\r\n))*?.*SERVER: Linux/([\w._+-]+), UPnP/(                                             [\d.]+), Intel UPnP SDK/([\w._~-]+)\r\n'
Warning: Hit PCRE_ERROR_MATCHLIMIT when probing for service http with the regex                                              '^HTTP/1\.1 \d\d\d (?:[^\r\n]*\r\n(?!\r\n))*?.*\r\nServer: Virata-EmWeb/R([\d_]+                                             )\r\nContent-Type: text/html; ?charset=UTF-8\r\nExpires: .*<title>HP (Color |)La                                             serJet ([\w._ -]+)&nbsp;&nbsp;&nbsp;'
Completed Service scan at 23:56, 11.28s elapsed (1 service on 1 host)
Initiating OS detection (try #1) against juice-shop.lab.rtu.lv (192.168.1.13)
NSE: Script scanning 192.168.1.13.
NSE: Starting runlevel 1 (of 3) scan.
Initiating NSE at 23:56
Completed NSE at 23:56, 0.02s elapsed
NSE: Starting runlevel 2 (of 3) scan.
Initiating NSE at 23:56
Completed NSE at 23:56, 1.01s elapsed
NSE: Starting runlevel 3 (of 3) scan.
Initiating NSE at 23:56
Completed NSE at 23:56, 0.00s elapsed
Nmap scan report for juice-shop.lab.rtu.lv (192.168.1.13)
Host is up, received arp-response (0.00097s latency).
Scanned at 2025-05-21 23:55:50 EEST for 14s
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
|     Last-Modified: Wed, 21 May 2025 20:17:36 GMT
|     ETag: W/"11708-196f47e8c1e"
|     Content-Type: text/html; charset=UTF-8
|     Content-Length: 71432
|     Vary: Accept-Encoding
|     Date: Wed, 21 May 2025 20:56:01 GMT
|     Connection: close
|     <!--
|     Copyright (c) 2014-2025 Bjoern Kimminich & the OWASP Juice Shop contributo
rs.
|     SPDX-License-Identifier: MIT
|     <!doctype html>
|     <html lang="en" data-critters-container>
|     <head>
|     <meta charset="utf-8">
|     <title>OWASP Juice Shop</title>
|     <meta name="description" content="Probably the most modern and sophisticat
ed insecure web application">
|     <meta name="viewport" content="width=device-width, initial-scale=1">
|     <link id="favicon" rel="icon"
|   HTTPOptions, RTSPRequest:
|     HTTP/1.1 204 No Content
|     Access-Control-Allow-Origin: *
|     Access-Control-Allow-Methods: GET,HEAD,PUT,PATCH,POST,DELETE
|     Vary: Access-Control-Request-Headers
|     Content-Length: 0
|     Date: Wed, 21 May 2025 20:56:01 GMT
|     Connection: close
|   Help, NCP:
|     HTTP/1.1 400 Bad Request
|_    Connection: close
1 service unrecognized despite returning data. If you know the service/version,
please submit the following fingerprint at https://nmap.org/cgi-bin/submit.cgi?n
ew-service :
SF-Port3000-TCP:V=7.95%I=7%D=5/21%Time=682E3DE1%P=x86_64-pc-linux-gnu%r(Ge
SF:tRequest,3890,"HTTP/1\.1\x20200\x20OK\r\nAccess-Control-Allow-Origin:\x
SF:20\*\r\nX-Content-Type-Options:\x20nosniff\r\nX-Frame-Options:\x20SAMEO
SF:RIGIN\r\nFeature-Policy:\x20payment\x20'self'\r\nX-Recruiting:\x20/#/jo
SF:bs\r\nAccept-Ranges:\x20bytes\r\nCache-Control:\x20public,\x20max-age=0
SF:\r\nLast-Modified:\x20Wed,\x2021\x20May\x202025\x2020:17:36\x20GMT\r\nE
SF:Tag:\x20W/\"11708-196f47e8c1e\"\r\nContent-Type:\x20text/html;\x20chars
SF:et=UTF-8\r\nContent-Length:\x2071432\r\nVary:\x20Accept-Encoding\r\nDat
SF:e:\x20Wed,\x2021\x20May\x202025\x2020:56:01\x20GMT\r\nConnection:\x20cl
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
SF:ntrol-Request-Headers\r\nContent-Length:\x200\r\nDate:\x20Wed,\x2021\x2
SF:0May\x202025\x2020:56:01\x20GMT\r\nConnection:\x20close\r\n\r\n")%r(RTS
SF:PRequest,EA,"HTTP/1\.1\x20204\x20No\x20Content\r\nAccess-Control-Allow-
SF:Origin:\x20\*\r\nAccess-Control-Allow-Methods:\x20GET,HEAD,PUT,PATCH,PO
SF:ST,DELETE\r\nVary:\x20Access-Control-Request-Headers\r\nContent-Length:
SF:\x200\r\nDate:\x20Wed,\x2021\x20May\x202025\x2020:56:01\x20GMT\r\nConne
SF:ction:\x20close\r\n\r\n");
MAC Address: 0A:28:7D:F7:84:2C (Unknown)
Device type: general purpose|router
Running: Linux 4.X|5.X, MikroTik RouterOS 7.X
OS CPE: cpe:/o:linux:linux_kernel:4 cpe:/o:linux:linux_kernel:5 cpe:/o:mikrotik:
routeros:7 cpe:/o:linux:linux_kernel:5.6.3
OS details: Linux 4.15 - 5.19, OpenWrt 21.02 (Linux 5.4), MikroTik RouterOS 7.2
- 7.5 (Linux 5.6.3)
TCP/IP fingerprint:
OS:SCAN(V=7.95%E=4%D=5/21%OT=3000%CT=1%CU=36257%PV=Y%DS=1%DC=D%G=Y%M=0A287D
OS:%TM=682E3DE4%P=x86_64-pc-linux-gnu)SEQ(SP=105%GCD=1%ISR=10A%TI=Z%CI=Z%II
OS:=I%TS=A)OPS(O1=M5B4ST11NW7%O2=M5B4ST11NW7%O3=M5B4NNT11NW7%O4=M5B4ST11NW7
OS:%O5=M5B4ST11NW7%O6=M5B4ST11)WIN(W1=FE88%W2=FE88%W3=FE88%W4=FE88%W5=FE88%
OS:W6=FE88)ECN(R=Y%DF=Y%T=40%W=FAF0%O=M5B4NNSNW7%CC=Y%Q=)T1(R=Y%DF=Y%T=40%S
OS:=O%A=S+%F=AS%RD=0%Q=)T2(R=N)T3(R=N)T4(R=Y%DF=Y%T=40%W=0%S=A%A=Z%F=R%O=%R
OS:D=0%Q=)T5(R=Y%DF=Y%T=40%W=0%S=Z%A=S+%F=AR%O=%RD=0%Q=)T6(R=Y%DF=Y%T=40%W=
OS:0%S=A%A=Z%F=R%O=%RD=0%Q=)T7(R=Y%DF=Y%T=40%W=0%S=Z%A=S+%F=AR%O=%RD=0%Q=)U
OS:1(R=Y%DF=N%T=40%IPL=164%UN=0%RIPL=G%RID=G%RIPCK=G%RUCK=G%RUD=G)IE(R=Y%DF
OS:I=N%T=40%CD=S)

Uptime guess: 13.177 days (since Thu May  8 19:41:17 2025)
Network Distance: 1 hop
TCP Sequence Prediction: Difficulty=261 (Good luck!)
IP ID Sequence Generation: All zeros

TRACEROUTE
HOP RTT     ADDRESS
1   0.97 ms juice-shop.lab.rtu.lv (192.168.1.13)

NSE: Script Post-scanning.
NSE: Starting runlevel 1 (of 3) scan.
Initiating NSE at 23:56
Completed NSE at 23:56, 0.00s elapsed
NSE: Starting runlevel 2 (of 3) scan.
Initiating NSE at 23:56
Completed NSE at 23:56, 0.00s elapsed
NSE: Starting runlevel 3 (of 3) scan.
Initiating NSE at 23:56
Completed NSE at 23:56, 0.00s elapsed
Read data files from: /usr/share/nmap
OS and Service detection performed. Please report any incorrect results at https
://nmap.org/submit/ .
Nmap done: 1 IP address (1 host up) scanned in 14.03 seconds
           Raw packets sent: 1023 (45.806KB) | Rcvd: 1015 (41.282KB)
```
