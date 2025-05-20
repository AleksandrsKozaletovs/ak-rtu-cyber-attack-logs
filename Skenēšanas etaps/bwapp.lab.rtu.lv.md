**Zenmap lietojumprogrammas rezultāts**
=======================================
```
Starting Nmap 7.95 ( https://nmap.org ) at 2025-05-20 22:46 EEST
NSE: Loaded 157 scripts for scanning.
NSE: Script Pre-scanning.
NSE: Starting runlevel 1 (of 3) scan.
Initiating NSE at 22:46
Completed NSE at 22:46, 0.00s elapsed
NSE: Starting runlevel 2 (of 3) scan.
Initiating NSE at 22:46
Completed NSE at 22:46, 0.00s elapsed
NSE: Starting runlevel 3 (of 3) scan.
Initiating NSE at 22:46
Completed NSE at 22:46, 0.00s elapsed
Initiating ARP Ping Scan at 22:46
Scanning 192.168.1.14 [1 port]
Completed ARP Ping Scan at 22:46, 0.04s elapsed (1 total hosts)
Initiating SYN Stealth Scan at 22:46
Scanning bwapp.lab.rtu.lv (192.168.1.14) [1000 ports]
Discovered open port 3306/tcp on 192.168.1.14
Discovered open port 80/tcp on 192.168.1.14
Completed SYN Stealth Scan at 22:46, 0.10s elapsed (1000 total ports)
Initiating Service scan at 22:46
Scanning 2 services on bwapp.lab.rtu.lv (192.168.1.14)
Completed Service scan at 22:46, 6.04s elapsed (2 services on 1 host)
Initiating OS detection (try #1) against bwapp.lab.rtu.lv (192.168.1.14)
NSE: Script scanning 192.168.1.14.
NSE: Starting runlevel 1 (of 3) scan.
Initiating NSE at 22:46
Completed NSE at 22:46, 0.18s elapsed
NSE: Starting runlevel 2 (of 3) scan.
Initiating NSE at 22:46
Completed NSE at 22:46, 0.02s elapsed
NSE: Starting runlevel 3 (of 3) scan.
Initiating NSE at 22:46
Completed NSE at 22:46, 0.00s elapsed
Nmap scan report for bwapp.lab.rtu.lv (192.168.1.14)
Host is up, received arp-response (0.00091s latency).
Scanned at 2025-05-20 22:46:38 EEST for 8s
Not shown: 998 closed tcp ports (reset)
PORT     STATE SERVICE REASON         VERSION
80/tcp   open  http    syn-ack ttl 64 Apache httpd 2.4.7 ((Ubuntu))
| http-methods:
|_  Supported Methods: GET HEAD POST OPTIONS
| http-title: Site doesn't have a title (text/html).
|_Requested resource was login.php
| http-robots.txt: 5 disallowed entries
|_/ /admin/ /documents/ /images/ /passwords/
|_http-server-header: Apache/2.4.7 (Ubuntu)
3306/tcp open  mysql   syn-ack ttl 64 MySQL 5.5.47-0ubuntu0.14.04.1
| mysql-info:
|   Protocol: 10
|   Version: 5.5.47-0ubuntu0.14.04.1
|   Thread ID: 2
|   Capabilities flags: 63487
|   Some Capabilities: Support41Auth, SupportsLoadDataLocal, FoundRows, DontAllowDatabaseTableColumn, LongColumnFlag, ConnectWithDatabase, IgnoreSigpipes,
                       Speaks41ProtocolNew, Speaks41ProtocolOld, SupportsTransactions, InteractiveClient, SupportsCompression, LongPassword, ODBCClient,
                       IgnoreSpaceBeforeParenthesis, SupportsMultipleResults, SupportsAuthPlugins, SupportsMultipleStatments
|   Status: Autocommit
|   Salt: 9E-R4NjN%lpnYQi=63@&
|_  Auth Plugin Name: mysql_native_password
MAC Address: 2A:81:49:1E:63:99 (Unknown)
Device type: general purpose|router
Running: Linux 4.X|5.X, MikroTik RouterOS 7.X
OS CPE: cpe:/o:linux:linux_kernel:4 cpe:/o:linux:linux_kernel:5 cpe:/o:mikrotik:routeros:7 cpe:/o:linux:linux_kernel:5.6.3
OS details: Linux 4.15 - 5.19, MikroTik RouterOS 7.2 - 7.5 (Linux 5.6.3)
TCP/IP fingerprint:
OS:SCAN(V=7.95%E=4%D=5/20%OT=80%CT=1%CU=43706%PV=Y%DS=1%DC=D%G=Y%M=2A8149%T
OS:M=682CDC26%P=x86_64-pc-linux-gnu)SEQ(SP=102%GCD=1%ISR=110%TI=Z%CI=Z%II=I
OS:%TS=A)OPS(O1=M5B4ST11NW7%O2=M5B4ST11NW7%O3=M5B4NNT11NW7%O4=M5B4ST11NW7%O
OS:5=M5B4ST11NW7%O6=M5B4ST11)WIN(W1=FE88%W2=FE88%W3=FE88%W4=FE88%W5=FE88%W6
OS:=FE88)ECN(R=Y%DF=Y%T=40%W=FAF0%O=M5B4NNSNW7%CC=Y%Q=)T1(R=Y%DF=Y%T=40%S=O
OS:%A=S+%F=AS%RD=0%Q=)T2(R=N)T3(R=N)T4(R=Y%DF=Y%T=40%W=0%S=A%A=Z%F=R%O=%RD=
OS:0%Q=)T5(R=Y%DF=Y%T=40%W=0%S=Z%A=S+%F=AR%O=%RD=0%Q=)T6(R=Y%DF=Y%T=40%W=0%
OS:S=A%A=Z%F=R%O=%RD=0%Q=)T7(R=Y%DF=Y%T=40%W=0%S=Z%A=S+%F=AR%O=%RD=0%Q=)U1(
OS:R=Y%DF=N%T=40%IPL=164%UN=0%RIPL=G%RID=G%RIPCK=G%RUCK=G%RUD=G)IE(R=Y%DFI=
OS:N%T=40%CD=S)

Uptime guess: 1.787 days (since Mon May 19 03:54:12 2025)
Network Distance: 1 hop
TCP Sequence Prediction: Difficulty=258 (Good luck!)
IP ID Sequence Generation: All zeros

TRACEROUTE
HOP RTT     ADDRESS
1   0.91 ms bwapp.lab.rtu.lv (192.168.1.14)

NSE: Script Post-scanning.
NSE: Starting runlevel 1 (of 3) scan.
Initiating NSE at 22:46
Completed NSE at 22:46, 0.00s elapsed
NSE: Starting runlevel 2 (of 3) scan.
Initiating NSE at 22:46
Completed NSE at 22:46, 0.00s elapsed
NSE: Starting runlevel 3 (of 3) scan.
Initiating NSE at 22:46
Completed NSE at 22:46, 0.00s elapsed
Read data files from: /usr/share/nmap
OS and Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
Nmap done: 1 IP address (1 host up) scanned in 7.97 seconds
           Raw packets sent: 1023 (45.806KB) | Rcvd: 1015 (41.286KB)
```
