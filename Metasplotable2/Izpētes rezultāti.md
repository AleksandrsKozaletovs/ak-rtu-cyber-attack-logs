**ping komandas rezultāts**
===========================
```
PING metasploitable.lab.rtu.lv (192.168.1.200) 56(84) bytes of data.
64 bytes from metasploitable.lab.rtu.lv (192.168.1.200): icmp_seq=1 ttl=64 time=3.57 ms
64 bytes from metasploitable.lab.rtu.lv (192.168.1.200): icmp_seq=2 ttl=64 time=3.97 ms
64 bytes from metasploitable.lab.rtu.lv (192.168.1.200): icmp_seq=3 ttl=64 time=12.1 ms
64 bytes from metasploitable.lab.rtu.lv (192.168.1.200): icmp_seq=4 ttl=64 time=5.17 ms
--- metasploitable.lab.rtu.lv ping statistics ---
4 packets transmitted, 4 received, 0% packet loss, time 3005ms
rtt min/avg/max/mdev = 3.570/6.206/12.111/3.459 ms
```

**dig komandas rezultāts**
==========================
```
; <<>> DiG 9.20.8-6-Debian <<>> metasploitable.lab.rtu.lv
;; global options: +cmd
;; Got answer:
;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 41254
;; flags: qr aa rd ra; QUERY: 1, ANSWER: 1, AUTHORITY: 0, ADDITIONAL: 1

;; OPT PSEUDOSECTION:
; EDNS: version: 0, flags:; udp: 1232
;; QUESTION SECTION:
;metasploitable.lab.rtu.lv.     IN      A

;; ANSWER SECTION:
metasploitable.lab.rtu.lv. 0    IN      A       192.168.1.200

;; Query time: 0 msec
;; SERVER: ::1#53(::1) (UDP)
;; WHEN: Wed May 14 20:16:19 EEST 2025
;; MSG SIZE  rcvd: 70
```

**arp-scan komandas rezultāts**
===============================
```
Interface: eth0, type: EN10MB, MAC: 00:0c:29:49:85:02, IPv4: 192.168.1.175
WARNING: Cannot open MAC/Vendor file ieee-oui.txt: Permission denied
WARNING: Cannot open MAC/Vendor file mac-vendor.txt: Permission denied
Starting arp-scan 1.10.0 with 256 hosts (https://github.com/royhills/arp-scan)
192.168.1.1     24:2f:d0:16:57:a0       (Unknown)
192.168.1.2     d4:6e:0e:6b:ca:d0       (Unknown)
192.168.1.36    f0:a6:54:9f:35:99       (Unknown)
192.168.1.51    12:bc:cc:26:c7:62 (24:2f:d0:16:57:9e)   (Unknown: locally administered)
192.168.1.50    d2:9a:00:43:a7:d7 (24:2f:d0:16:57:9e)   (Unknown: locally administered)
192.168.1.100   00:0c:29:8c:dd:10       (Unknown)
192.168.1.170   00:0c:29:38:7a:5a       (Unknown)
192.168.1.168   00:e0:4c:68:1c:5e       (Unknown)
192.168.1.200   00:0c:29:73:1a:30       (Unknown)
192.168.1.246   1c:1b:0d:5a:06:ea       (Unknown)

10 packets received by filter, 0 packets dropped by kernel
Ending arp-scan 1.10.0: 256 hosts scanned in 1.839 seconds (139.21 hosts/sec). 10 responded
```
