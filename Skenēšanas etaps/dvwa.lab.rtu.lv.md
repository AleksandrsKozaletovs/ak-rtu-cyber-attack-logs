**Zenmap lietojumprogrammas rezultāts**
=======================================
```
Starting Nmap 7.95 ( https://nmap.org ) at 2025-05-20 22:09 EEST
NSE: Loaded 157 scripts for scanning.
NSE: Script Pre-scanning.
NSE: Starting runlevel 1 (of 3) scan.
Initiating NSE at 22:09
Completed NSE at 22:09, 0.00s elapsed
NSE: Starting runlevel 2 (of 3) scan.
Initiating NSE at 22:09
Completed NSE at 22:09, 0.00s elapsed
NSE: Starting runlevel 3 (of 3) scan.
Initiating NSE at 22:09
Completed NSE at 22:09, 0.00s elapsed
Initiating ARP Ping Scan at 22:09
Scanning 192.168.1.12 [1 port]
Completed ARP Ping Scan at 22:09, 0.05s elapsed (1 total hosts)
Initiating SYN Stealth Scan at 22:09
Scanning dvwa.lab.rtu.lv (192.168.1.12) [1000 ports]
Discovered open port 3306/tcp on 192.168.1.12
Discovered open port 80/tcp on 192.168.1.12
Completed SYN Stealth Scan at 22:09, 0.10s elapsed (1000 total ports)
Initiating Service scan at 22:09
Scanning 2 services on dvwa.lab.rtu.lv (192.168.1.12)
Completed Service scan at 22:09, 6.08s elapsed (2 services on 1 host)
Initiating OS detection (try #1) against dvwa.lab.rtu.lv (192.168.1.12)
NSE: Script scanning 192.168.1.12.
NSE: Starting runlevel 1 (of 3) scan.
Initiating NSE at 22:09
Completed NSE at 22:09, 0.21s elapsed
NSE: Starting runlevel 2 (of 3) scan.
Initiating NSE at 22:09
Completed NSE at 22:09, 0.01s elapsed
NSE: Starting runlevel 3 (of 3) scan.
Initiating NSE at 22:09
Completed NSE at 22:09, 0.00s elapsed
Nmap scan report for dvwa.lab.rtu.lv (192.168.1.12)
Host is up, received arp-response (0.0012s latency).
Scanned at 2025-05-20 22:09:01 EEST for 8s
Not shown: 998 closed tcp ports (reset)
PORT     STATE SERVICE REASON         VERSION
80/tcp   open  http    syn-ack ttl 64 Apache httpd 2.4.10 ((Debian))
|_http-favicon: Unknown favicon MD5: 69C728902A3F1DF75CF9EAC73BD55556
|_http-server-header: Apache/2.4.10 (Debian)
| http-cookie-flags:
|   /:
|     PHPSESSID:
|_      httponly flag not set
| http-title: Login :: Damn Vulnerable Web Application (DVWA) v1.10 *Develop...
|_Requested resource was login.php
| http-methods:
|_  Supported Methods: GET HEAD POST OPTIONS
| http-robots.txt: 1 disallowed entry
|_/
3306/tcp open  mysql   syn-ack ttl 64 MySQL 5.5.54-0+deb8u1-log
| mysql-info:
|   Protocol: 10
|   Version: 5.5.54-0+deb8u1-log
|   Thread ID: 39
|   Capabilities flags: 63487
|   Some Capabilities: ConnectWithDatabase, LongPassword, SupportsCompression, Speaks41ProtocolOld, DontAllowDatabaseTableColumn,
                        FoundRows, IgnoreSpaceBeforeParenthesis, IgnoreSigpipes, InteractiveClient, Speaks41ProtocolNew, SupportsTransactions, 
                        LongColumnFlag, Support41Auth, ODBCClient, SupportsLoadDataLocal, SupportsMultipleResults, SupportsAuthPlugins, SupportsMultipleStatments
|   Status: Autocommit
|   Salt: ]1{9JGc@Te"sA)Gkg@L;
|_  Auth Plugin Name: mysql_native_password
MAC Address: 9E:31:BC:E8:49:C7 (Unknown)
Device type: general purpose|router
Running: Linux 4.X|5.X, MikroTik RouterOS 7.X
OS CPE: cpe:/o:linux:linux_kernel:4 cpe:/o:linux:linux_kernel:5 cpe:/o:mikrotik:routeros:7 cpe:/o:linux:linux_kernel:5.6.3
OS details: Linux 4.15 - 5.19, OpenWrt 21.02 (Linux 5.4), MikroTik RouterOS 7.2 - 7.5 (Linux 5.6.3)
TCP/IP fingerprint:
OS:SCAN(V=7.95%E=4%D=5/20%OT=80%CT=1%CU=35651%PV=Y%DS=1%DC=D%G=Y%M=9E31BC%T
OS:M=682CD355%P=x86_64-pc-linux-gnu)SEQ(SP=105%GCD=1%ISR=106%TI=Z%CI=Z%II=I
OS:%TS=A)OPS(O1=M5B4ST11NW7%O2=M5B4ST11NW7%O3=M5B4NNT11NW7%O4=M5B4ST11NW7%O
OS:5=M5B4ST11NW7%O6=M5B4ST11)WIN(W1=FE88%W2=FE88%W3=FE88%W4=FE88%W5=FE88%W6
OS:=FE88)ECN(R=Y%DF=Y%T=40%W=FAF0%O=M5B4NNSNW7%CC=Y%Q=)T1(R=Y%DF=Y%T=40%S=O
OS:%A=S+%F=AS%RD=0%Q=)T2(R=N)T3(R=N)T4(R=Y%DF=Y%T=40%W=0%S=A%A=Z%F=R%O=%RD=
OS:0%Q=)T5(R=Y%DF=Y%T=40%W=0%S=Z%A=S+%F=AR%O=%RD=0%Q=)T6(R=Y%DF=Y%T=40%W=0%
OS:S=A%A=Z%F=R%O=%RD=0%Q=)T7(R=Y%DF=Y%T=40%W=0%S=Z%A=S+%F=AR%O=%RD=0%Q=)U1(
OS:R=Y%DF=N%T=40%IPL=164%UN=0%RIPL=G%RID=G%RIPCK=G%RUCK=G%RUD=G)IE(R=Y%DFI=
OS:N%T=40%CD=S)

Uptime guess: 44.472 days (since Sun Apr  6 10:49:43 2025)
Network Distance: 1 hop
TCP Sequence Prediction: Difficulty=261 (Good luck!)
IP ID Sequence Generation: All zeros

TRACEROUTE
HOP RTT     ADDRESS
1   1.24 ms dvwa.lab.rtu.lv (192.168.1.12)

NSE: Script Post-scanning.
NSE: Starting runlevel 1 (of 3) scan.
Initiating NSE at 22:09
Completed NSE at 22:09, 0.00s elapsed
NSE: Starting runlevel 2 (of 3) scan.
Initiating NSE at 22:09
Completed NSE at 22:09, 0.00s elapsed
NSE: Starting runlevel 3 (of 3) scan.
Initiating NSE at 22:09
Completed NSE at 22:09, 0.00s elapsed
Read data files from: /usr/share/nmap
OS and Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
Nmap done: 1 IP address (1 host up) scanned in 8.08 seconds
           Raw packets sent: 1023 (45.806KB) | Rcvd: 1015 (41.286KB)
```
