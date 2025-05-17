**ping komandas rezultāts**
===========================
```
PING juice-shop.lab.rtu.lv (192.168.1.200) 56(84) bytes of data.
64 bytes from juice-shop.lab.rtu.lv (192.168.1.200): icmp_seq=1 ttl=64 time=0.358 ms
64 bytes from juice-shop.lab.rtu.lv (192.168.1.200): icmp_seq=2 ttl=64 time=0.560 ms
64 bytes from juice-shop.lab.rtu.lv (192.168.1.200): icmp_seq=3 ttl=64 time=0.622 ms
64 bytes from juice-shop.lab.rtu.lv (192.168.1.200): icmp_seq=4 ttl=64 time=0.768 ms
--- juice-shop.lab.rtu.lv ping statistics ---
4 packets transmitted, 4 received, 0% packet loss, time 3051ms
rtt min/avg/max/mdev = 0.358/0.577/0.768/0.147 ms
```

**dig komandas rezultāts**
==========================
```
; <<>> DiG 9.20.8-6-Debian <<>> juice-shop.lab.rtu.lv
;; global options: +cmd
;; Got answer:
;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 14624
;; flags: qr rd ra ad; QUERY: 1, ANSWER: 0, AUTHORITY: 1, ADDITIONAL: 1

;; OPT PSEUDOSECTION:
; EDNS: version: 0, flags:; udp: 1232
;; QUESTION SECTION:
;juice-shop.lab.rtu.lv.         IN      A

;; ANSWER SECTION:
juice-shop.lab.rtu.lv. 0    IN      A       192.168.1.200

;; Query time: 0 msec
;; SERVER: 192.168.1.1#53(192.168.1.1) (UDP)
;; WHEN: Sat May 17 18:37:25 EEST 2025
;; MSG SIZE  rcvd: 113
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
192.168.1.100   00:0c:29:8c:dd:10       (Unknown)
192.168.1.168   00:e0:4c:68:1c:5e       (Unknown)
192.168.1.170   00:0c:29:38:7a:5a       (Unknown)
192.168.1.200   00:0c:29:73:1a:30       (Unknown)
192.168.1.246   1c:1b:0d:5a:06:ea       (Unknown)

9 packets received by filter, 0 packets dropped by kernel
Ending arp-scan 1.10.0: 256 hosts scanned in 1.869 seconds (136.97 hosts/sec). 7 responded
```
