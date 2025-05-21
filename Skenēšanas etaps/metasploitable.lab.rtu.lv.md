**Zenmap lietojumprogrammas rezultāts**
=======================================
```
Starting Nmap 7.95 ( https://nmap.org ) at 2025-05-21 23:18 EEST
NSE: Loaded 157 scripts for scanning.
NSE: Script Pre-scanning.
NSE: Starting runlevel 1 (of 3) scan.
Initiating NSE at 23:18
Completed NSE at 23:18, 0.00s elapsed
NSE: Starting runlevel 2 (of 3) scan.
Initiating NSE at 23:18
Completed NSE at 23:18, 0.00s elapsed
NSE: Starting runlevel 3 (of 3) scan.
Initiating NSE at 23:18
Completed NSE at 23:18, 0.00s elapsed
Initiating ARP Ping Scan at 23:18
Scanning 192.168.1.11 [1 port]
Completed ARP Ping Scan at 23:18, 0.08s elapsed (1 total hosts)
Initiating SYN Stealth Scan at 23:18
Scanning metasploitable.lab.rtu.lv (192.168.1.11) [1000 ports]
Discovered open port 3306/tcp on 192.168.1.11
Discovered open port 21/tcp on 192.168.1.11
Discovered open port 22/tcp on 192.168.1.11
Discovered open port 23/tcp on 192.168.1.11
Discovered open port 139/tcp on 192.168.1.11
Discovered open port 25/tcp on 192.168.1.11
Discovered open port 445/tcp on 192.168.1.11
Discovered open port 80/tcp on 192.168.1.11
Discovered open port 111/tcp on 192.168.1.11
Discovered open port 513/tcp on 192.168.1.11
Discovered open port 5432/tcp on 192.168.1.11
Discovered open port 512/tcp on 192.168.1.11
Discovered open port 6667/tcp on 192.168.1.11
Discovered open port 514/tcp on 192.168.1.11
Discovered open port 1099/tcp on 192.168.1.11
Discovered open port 8009/tcp on 192.168.1.11
Discovered open port 2121/tcp on 192.168.1.11
Discovered open port 8180/tcp on 192.168.1.11
Discovered open port 1524/tcp on 192.168.1.11
Completed SYN Stealth Scan at 23:18, 0.12s elapsed (1000 total ports)
Initiating Service scan at 23:18
Scanning 19 services on metasploitable.lab.rtu.lv (192.168.1.11)
Completed Service scan at 23:20, 151.39s elapsed (19 services on 1 host)
Initiating OS detection (try #1) against metasploitable.lab.rtu.lv (192.168.1.11                                                                                                                                                                             )
NSE: Script scanning 192.168.1.11.
NSE: Starting runlevel 1 (of 3) scan.
Initiating NSE at 23:20
NSE: [ftp-bounce 192.168.1.11:21] PORT response: 500 Illegal PORT command.
Completed NSE at 23:21, 7.69s elapsed
NSE: Starting runlevel 2 (of 3) scan.
Initiating NSE at 23:21
Completed NSE at 23:21, 1.15s elapsed
NSE: Starting runlevel 3 (of 3) scan.
Initiating NSE at 23:21
Completed NSE at 23:21, 0.00s elapsed
Nmap scan report for metasploitable.lab.rtu.lv (192.168.1.11)
Host is up, received arp-response (0.0017s latency).
Scanned at 2025-05-21 23:18:20 EEST for 162s
Not shown: 981 closed tcp ports (reset)
PORT     STATE SERVICE     REASON         VERSION
21/tcp   open  ftp         syn-ack ttl 64 vsftpd 2.3.4
| ftp-syst:
|   STAT:
| FTP server status:
|      Connected to 192.168.1.175
|      Logged in as ftp
|      TYPE: ASCII
|      No session bandwidth limit
|      Session timeout in seconds is 300
|      Control connection is plain text
|      Data connections will be plain text
|      vsFTPd 2.3.4 - secure, fast, stable
|_End of status
|_ftp-anon: Anonymous FTP login allowed (FTP code 230)
22/tcp   open  ssh         syn-ack ttl 64 OpenSSH 4.7p1 Debian 8ubuntu1 (protoco                                                                                                                                                                             l 2.0)
| ssh-hostkey:
|   1024 60:0f:cf:e1:c0:5f:6a:74:d6:90:24:fa:c4:d5:6c:cd (DSA)
| ssh-dss AAAAB3NzaC1kc3MAAACBALz4hsc8a2Srq4nlW960qV8xwBG0JC+jI7fWxm5METIJH4tKr/                                                                                                                                                                             xUTwsTYEYnaZLzcOiy21D3ZvOwYb6AA3765zdgCd2Tgand7F0YD5UtXG7b7fbz99chReivL0SIWEG/E9                                                                                                                                                                             6Ai+pqYMP2WD5KaOJwSIXSUajnU5oWmY5x85sBw+XDAAAAFQDFkMpmdFQTF+oRqaoSNVU7Z+hjSwAAAI                                                                                                                                                                             BCQxNKzi1TyP+QJIFa3M0oLqCVWI0We/ARtXrzpBOJ/dt0hTJXCeYisKqcdwdtyIn8OUCOyrIjqNuA2Q                                                                                                                                                                             W217oQ6wXpbFh+5AQm8Hl3b6C6o8lX3Ptw+Y4dp0lzfWHwZ/jzHwtuaDQaok7u1f971lEazeJLqfiWrA                                                                                                                                                                             zoklqSWyDQJAAAAIA1lAD3xWYkeIeHv/R3P9i+XaoI7imFkMuYXCDTq843YU6Td+0mWpllCqAWUV/CQa                                                                                                                                                                             mGgQLtYy5S0ueoks01MoKdOMMhKVwqdr08nvCBdNKjIEd3gH6oBk/YRnjzxlEAYBsvCmM4a0jmhz0oNi                                                                                                                                                                             RWlc/F+bkUeFKrBx/D2fdfZmhrGg==
|   2048 56:56:24:0f:21:1d:de:a7:2b:ae:61:b1:24:3d:e8:f3 (RSA)
|_ssh-rsa AAAAB3NzaC1yc2EAAAABIwAAAQEAstqnuFMBOZvO3WTEjP4TUdjgWkIVNdTq6kboEDjteO                                                                                                                                                                             fc65TlI7sRvQBwqAhQjeeyyIk8T55gMDkOD0akSlSXvLDcmcdYfxeIF0ZSuT+nkRhij7XSSA/Oc5QSk3                                                                                                                                                                             sJ/SInfb78e3anbRHpmkJcVgETJ5WhKObUNf1AKZW++4Xlc63M4KI5cjvMMIPEVOyR3AKmI78Fo3HJjY                                                                                                                                                                             ucg87JjLeC66I7+dlEYX6zT8i1XYwa/L1vZ3qSJISGVu8kRPikMv/cNSvki4j+qDYyZ2E5497W87+Ed4                                                                                                                                                                             6/8P42LNGoOV8OcX/ro6pAcbEPUdUEfkJrqi2YXbhvwIJ0gFMb6wfe5cnQew==
23/tcp   open  telnet      syn-ack ttl 64 Linux telnetd
25/tcp   open  smtp        syn-ack ttl 64 Postfix smtpd
|_ssl-date: 2025-05-21T20:21:02+00:00; 0s from scanner time.
|_smtp-commands: metasploitable.localdomain, PIPELINING, SIZE 10240000, VRFY, ET                                                                                                                                                                             RN, STARTTLS, ENHANCEDSTATUSCODES, 8BITMIME, DSN
| sslv2:
|   SSLv2 supported
|   ciphers:
|     SSL2_DES_192_EDE3_CBC_WITH_MD5
|     SSL2_DES_64_CBC_WITH_MD5
|     SSL2_RC4_128_WITH_MD5
|     SSL2_RC4_128_EXPORT40_WITH_MD5
|     SSL2_RC2_128_CBC_EXPORT40_WITH_MD5
|_    SSL2_RC2_128_CBC_WITH_MD5
| ssl-cert: Subject: commonName=ubuntu804-base.localdomain/organizationName=OCOS                                                                                                                                                                             A/stateOrProvinceName=There is no such thing outside US/countryName=XX/emailAddr                                                                                                                                                                             ess=root@ubuntu804-base.localdomain/organizationalUnitName=Office for Complicati                                                                                                                                                                             on of Otherwise Simple Affairs/localityName=Everywhere
| Issuer: commonName=ubuntu804-base.localdomain/organizationName=OCOSA/stateOrPr                                                                                                                                                                             ovinceName=There is no such thing outside US/countryName=XX/emailAddress=root@ub                                                                                                                                                                             untu804-base.localdomain/organizationalUnitName=Office for Complication of Other                                                                                                                                                                             wise Simple Affairs/localityName=Everywhere
| Public Key type: rsa
| Public Key bits: 1024
| Signature Algorithm: sha1WithRSAEncryption
| Not valid before: 2010-03-17T14:07:45
| Not valid after:  2010-04-16T14:07:45
| MD5:   dcd9:ad90:6c8f:2f73:74af:383b:2540:8828
| SHA-1: ed09:3088:7066:03bf:d5dc:2373:99b4:98da:2d4d:31c6
| -----BEGIN CERTIFICATE-----
| MIIDWzCCAsQCCQD6+TpMf7a5zDANBgkqhkiG9w0BAQUFADCB8TELMAkGA1UEBhMC
| WFgxKjAoBgNVBAgTIVRoZXJlIGlzIG5vIHN1Y2ggdGhpbmcgb3V0c2lkZSBVUzET
| MBEGA1UEBxMKRXZlcnl3aGVyZTEOMAwGA1UEChMFT0NPU0ExPDA6BgNVBAsTM09m
| ZmljZSBmb3IgQ29tcGxpY2F0aW9uIG9mIE90aGVyd2lzZSBTaW1wbGUgQWZmYWly
| czEjMCEGA1UEAxMadWJ1bnR1ODA0LWJhc2UubG9jYWxkb21haW4xLjAsBgkqhkiG
| 9w0BCQEWH3Jvb3RAdWJ1bnR1ODA0LWJhc2UubG9jYWxkb21haW4wHhcNMTAwMzE3
| MTQwNzQ1WhcNMTAwNDE2MTQwNzQ1WjCB8TELMAkGA1UEBhMCWFgxKjAoBgNVBAgT
| IVRoZXJlIGlzIG5vIHN1Y2ggdGhpbmcgb3V0c2lkZSBVUzETMBEGA1UEBxMKRXZl
| cnl3aGVyZTEOMAwGA1UEChMFT0NPU0ExPDA6BgNVBAsTM09mZmljZSBmb3IgQ29t
| cGxpY2F0aW9uIG9mIE90aGVyd2lzZSBTaW1wbGUgQWZmYWlyczEjMCEGA1UEAxMa
| dWJ1bnR1ODA0LWJhc2UubG9jYWxkb21haW4xLjAsBgkqhkiG9w0BCQEWH3Jvb3RA
| dWJ1bnR1ODA0LWJhc2UubG9jYWxkb21haW4wgZ8wDQYJKoZIhvcNAQEBBQADgY0A
| MIGJAoGBANa0EzYzmpVxexvefIN12nGxPKl//q1kG3fpT66+ytT4y++uu0N5JHP/
| POWeO238yLGs+kxNXptMmVQL16hKULqp3h0f9ORrAqP0a0XNTK+NiWIzj2W7NmGf
| xCxzwU4uoKgUTphwRmG70bkx34yZ7nVreTxAoK6XAJCd3JkNM6S1AgMBAAEwDQYJ
| KoZIhvcNAQEFBQADgYEAkqS0uBRVYyVRSgvDKiLPOvgXagzPZqqnZS9Ibc3jPlyf
| d2zURFQfHoRPjtSN3awtiAkhqNpWLKkFPEloNRl1DNpTI4iIGS10JsEiZe4RaINq
| U0qcJ8ugtOmNKQyyPBhcZ8xTph4w0Komex6uQLkpAWwuvKIZlHwVbo0wOPbKLnU=
|_-----END CERTIFICATE-----
80/tcp   open  http        syn-ack ttl 64 Apache httpd 2.2.8 ((Ubuntu) DAV/2)
| http-methods:
|_  Supported Methods: GET HEAD POST OPTIONS
|_http-title: Metasploitable2 - Linux
|_http-server-header: Apache/2.2.8 (Ubuntu) DAV/2
111/tcp  open  rpcbind     syn-ack ttl 64
139/tcp  open  netbios-ssn syn-ack ttl 64 Samba smbd 3.X - 4.X (workgroup: WORKG                                                                                                                                                                             ROUP)
445/tcp  open  netbios-ssn syn-ack ttl 64 Samba smbd 3.0.20-Debian (workgroup: W                                                                                                                                                                             ORKGROUP)
512/tcp  open  exec        syn-ack ttl 64 netkit-rsh rexecd
513/tcp  open  login       syn-ack ttl 64 OpenBSD or Solaris rlogind
514/tcp  open  tcpwrapped  syn-ack ttl 64
1099/tcp open  java-rmi    syn-ack ttl 64 GNU Classpath grmiregistry
1524/tcp open  ingreslock? syn-ack ttl 64
| fingerprint-strings:
|   GenericLines:
|     ]0;@b2bd6545425e: /
|     root@b2bd6545425e:/#
|     ]0;@b2bd6545425e: /
|     root@b2bd6545425e:/#
|     ]0;@b2bd6545425e: /
|     root@b2bd6545425e:/#
|     ]0;@b2bd6545425e: /
|     root@b2bd6545425e:/#
|     ]0;@b2bd6545425e: /
|     root@b2bd6545425e:/#
|   GetRequest:
|     ]0;@b2bd6545425e: /
|     root@b2bd6545425e:/# GET / HTTP/1.0
|     <HTML>
|     <HEAD>
|     <TITLE>Directory /</TITLE>
|     <BASE HREF="file:/">
|     </HEAD>
|     <BODY>
|     <H1>Directory listing of /</H1>
|     <UL>
|     <LI><A HREF="./">./</A>
|     <LI><A HREF="../">../</A>
|     <LI><A HREF=".dockerenv">.dockerenv</A>
|     <LI><A HREF="bin/">bin/</A>
|     <LI><A HREF="boot/">boot/</A>
|     <LI><A HREF="cdrom/">cdrom/</A>
|     <LI><A HREF="core">core</A>
|     <LI><A HREF="dev/">dev/</A>
|     <LI><A HREF="etc/">etc/</A>
|     <LI><A HREF="home/">home/</A>
|     <LI><A HREF="initrd/">initrd/</A>
|     <LI><A HREF="initrd.img">initrd.img</A>
|     <LI><A HREF="lib/">lib/</A>
|     <LI><A HREF="lost%2Bfound/">lost+found/</A>
|     <LI><A HREF="media/">media/</A>
|     <LI><A HREF="mnt/">mnt/</A>
|     <LI><A HREF="nohup.out">nohup.out</A>
|     <LI><A HREF="opt/">opt/</A>
|     <LI><A HREF="proc/">proc/</A>
|     <LI><A HREF="root/">root/</A>
|     <LI><A HREF="sbin/">sbin/</A>
|     <LI><A HREF="srv/">srv/</A>
|     <LI><A HREF="sys/">sys/</A>
|     <LI><A HREF="tmp/
|   HTTPOptions:
|     ]0;@b2bd6545425e: /
|     root@b2bd6545425e:/# OPTIONS / HTTP/1.0
|     bash: OPTIONS: command not found
|     ]0;@b2bd6545425e: /
|     root@b2bd6545425e:/#
|     ]0;@b2bd6545425e: /
|     root@b2bd6545425e:/#
|     ]0;@b2bd6545425e: /
|     root@b2bd6545425e:/#
|     ]0;@b2bd6545425e: /
|     root@b2bd6545425e:/#
|   NULL:
|     ]0;@b2bd6545425e: /
|     root@b2bd6545425e:/#
|   RTSPRequest:
|     ]0;@b2bd6545425e: /
|     root@b2bd6545425e:/# OPTIONS / RTSP/1.0
|     bash: OPTIONS: command not found
|     ]0;@b2bd6545425e: /
|     root@b2bd6545425e:/#
|     ]0;@b2bd6545425e: /
|     root@b2bd6545425e:/#
|     ]0;@b2bd6545425e: /
|     root@b2bd6545425e:/#
|     ]0;@b2bd6545425e: /
|_    root@b2bd6545425e:/#
2121/tcp open  ftp         syn-ack ttl 64 ProFTPD 1.3.1
3306/tcp open  mysql       syn-ack ttl 64 MySQL 5.0.51a-3ubuntu5
| mysql-info:
|   Protocol: 10
|   Version: 5.0.51a-3ubuntu5
|   Thread ID: 8
|   Capabilities flags: 43564
|   Some Capabilities: Support41Auth, SupportsCompression, Speaks41ProtocolNew,                                                                                                                                                                              SupportsTransactions, SwitchToSSLAfterHandshake, ConnectWithDatabase, LongColumn                                                                                                                                                                             Flag
|   Status: Autocommit
|_  Salt: 37W1-.=+]rIRC8.{C{dd
5432/tcp open  postgresql  syn-ack ttl 64 PostgreSQL DB 8.3.0 - 8.3.7
| ssl-cert: Subject: commonName=ubuntu804-base.localdomain/organizationName=OCOS                                                                                                                                                                             A/stateOrProvinceName=There is no such thing outside US/countryName=XX/emailAddr                                                                                                                                                                             ess=root@ubuntu804-base.localdomain/organizationalUnitName=Office for Complicati                                                                                                                                                                             on of Otherwise Simple Affairs/localityName=Everywhere
| Issuer: commonName=ubuntu804-base.localdomain/organizationName=OCOSA/stateOrPr                                                                                                                                                                             ovinceName=There is no such thing outside US/countryName=XX/emailAddress=root@ub                                                                                                                                                                             untu804-base.localdomain/organizationalUnitName=Office for Complication of Other                                                                                                                                                                             wise Simple Affairs/localityName=Everywhere
| Public Key type: rsa
| Public Key bits: 1024
| Signature Algorithm: sha1WithRSAEncryption
| Not valid before: 2010-03-17T14:07:45
| Not valid after:  2010-04-16T14:07:45
| MD5:   dcd9:ad90:6c8f:2f73:74af:383b:2540:8828
| SHA-1: ed09:3088:7066:03bf:d5dc:2373:99b4:98da:2d4d:31c6
| -----BEGIN CERTIFICATE-----
| MIIDWzCCAsQCCQD6+TpMf7a5zDANBgkqhkiG9w0BAQUFADCB8TELMAkGA1UEBhMC
| WFgxKjAoBgNVBAgTIVRoZXJlIGlzIG5vIHN1Y2ggdGhpbmcgb3V0c2lkZSBVUzET
| MBEGA1UEBxMKRXZlcnl3aGVyZTEOMAwGA1UEChMFT0NPU0ExPDA6BgNVBAsTM09m
| ZmljZSBmb3IgQ29tcGxpY2F0aW9uIG9mIE90aGVyd2lzZSBTaW1wbGUgQWZmYWly
| czEjMCEGA1UEAxMadWJ1bnR1ODA0LWJhc2UubG9jYWxkb21haW4xLjAsBgkqhkiG
| 9w0BCQEWH3Jvb3RAdWJ1bnR1ODA0LWJhc2UubG9jYWxkb21haW4wHhcNMTAwMzE3
| MTQwNzQ1WhcNMTAwNDE2MTQwNzQ1WjCB8TELMAkGA1UEBhMCWFgxKjAoBgNVBAgT
| IVRoZXJlIGlzIG5vIHN1Y2ggdGhpbmcgb3V0c2lkZSBVUzETMBEGA1UEBxMKRXZl
| cnl3aGVyZTEOMAwGA1UEChMFT0NPU0ExPDA6BgNVBAsTM09mZmljZSBmb3IgQ29t
| cGxpY2F0aW9uIG9mIE90aGVyd2lzZSBTaW1wbGUgQWZmYWlyczEjMCEGA1UEAxMa
| dWJ1bnR1ODA0LWJhc2UubG9jYWxkb21haW4xLjAsBgkqhkiG9w0BCQEWH3Jvb3RA
| dWJ1bnR1ODA0LWJhc2UubG9jYWxkb21haW4wgZ8wDQYJKoZIhvcNAQEBBQADgY0A
| MIGJAoGBANa0EzYzmpVxexvefIN12nGxPKl//q1kG3fpT66+ytT4y++uu0N5JHP/
| POWeO238yLGs+kxNXptMmVQL16hKULqp3h0f9ORrAqP0a0XNTK+NiWIzj2W7NmGf
| xCxzwU4uoKgUTphwRmG70bkx34yZ7nVreTxAoK6XAJCd3JkNM6S1AgMBAAEwDQYJ
| KoZIhvcNAQEFBQADgYEAkqS0uBRVYyVRSgvDKiLPOvgXagzPZqqnZS9Ibc3jPlyf
| d2zURFQfHoRPjtSN3awtiAkhqNpWLKkFPEloNRl1DNpTI4iIGS10JsEiZe4RaINq
| U0qcJ8ugtOmNKQyyPBhcZ8xTph4w0Komex6uQLkpAWwuvKIZlHwVbo0wOPbKLnU=
|_-----END CERTIFICATE-----
|_ssl-date: 2025-05-21T20:21:02+00:00; 0s from scanner time.
6667/tcp open  irc         syn-ack ttl 64 UnrealIRCd
| irc-info:
|   users: 1
|   servers: 1
|   lusers: 1
|   lservers: 0
|   server: irc.Metasploitable.LAN
|   version: Unreal3.2.8.1. irc.Metasploitable.LAN
|   uptime: 0 days, 0:03:13
|   source ident: nmap
|   source host: 262C3E94.78DED367.FFFA6D49.IP
|_  error: Closing Link: nwstmgerq[192.168.1.175] (Quit: nwstmgerq)
8009/tcp open  ajp13       syn-ack ttl 64 Apache Jserv (Protocol v1.3)
|_ajp-methods: Failed to get a valid response for the OPTION request
8180/tcp open  http        syn-ack ttl 64 Apache Tomcat/Coyote JSP engine 1.1
|_http-title: Apache Tomcat/5.5
|_http-favicon: Apache Tomcat
| http-methods:
|_  Supported Methods: GET HEAD POST OPTIONS
|_http-server-header: Apache-Coyote/1.1
1 service unrecognized despite returning data. If you know the service/version,                                                                                                                                                                              please submit the following fingerprint at https://nmap.org/cgi-bin/submit.cgi?n                                                                                                                                                                             ew-service :
SF-Port1524-TCP:V=7.95%I=7%D=5/21%Time=682E3513%P=x86_64-pc-linux-gnu%r(NU
SF:LL,2A,"\x1b\]0;@b2bd6545425e:\x20/\x07root@b2bd6545425e:/#\x20")%r(Gene
SF:ricLines,D6,"\x1b\]0;@b2bd6545425e:\x20/\x07root@b2bd6545425e:/#\x20\n\
SF:x1b\]0;@b2bd6545425e:\x20/\x07root@b2bd6545425e:/#\x20\n\x1b\]0;@b2bd65
SF:45425e:\x20/\x07root@b2bd6545425e:/#\x20\n\x1b\]0;@b2bd6545425e:\x20/\x
SF:07root@b2bd6545425e:/#\x20\n\x1b\]0;@b2bd6545425e:\x20/\x07root@b2bd654
SF:5425e:/#\x20")%r(GetRequest,507,"\x1b\]0;@b2bd6545425e:\x20/\x07root@b2
SF:bd6545425e:/#\x20GET\x20/\x20HTTP/1\.0\n<HTML>\n<HEAD>\n<TITLE>Director
SF:y\x20/</TITLE>\n<BASE\x20HREF=\"file:/\">\n</HEAD>\n<BODY>\n<H1>Directo
SF:ry\x20listing\x20of\x20/</H1>\n<UL>\n<LI><A\x20HREF=\"\./\">\./</A>\n<L
SF:I><A\x20HREF=\"\.\./\">\.\./</A>\n<LI><A\x20HREF=\"\.dockerenv\">\.dock
SF:erenv</A>\n<LI><A\x20HREF=\"bin/\">bin/</A>\n<LI><A\x20HREF=\"boot/\">b
SF:oot/</A>\n<LI><A\x20HREF=\"cdrom/\">cdrom/</A>\n<LI><A\x20HREF=\"core\"
SF:>core</A>\n<LI><A\x20HREF=\"dev/\">dev/</A>\n<LI><A\x20HREF=\"etc/\">et
SF:c/</A>\n<LI><A\x20HREF=\"home/\">home/</A>\n<LI><A\x20HREF=\"initrd/\">
SF:initrd/</A>\n<LI><A\x20HREF=\"initrd\.img\">initrd\.img</A>\n<LI><A\x20
SF:HREF=\"lib/\">lib/</A>\n<LI><A\x20HREF=\"lost%2Bfound/\">lost\+found/</
SF:A>\n<LI><A\x20HREF=\"media/\">media/</A>\n<LI><A\x20HREF=\"mnt/\">mnt/<
SF:/A>\n<LI><A\x20HREF=\"nohup\.out\">nohup\.out</A>\n<LI><A\x20HREF=\"opt
SF:/\">opt/</A>\n<LI><A\x20HREF=\"proc/\">proc/</A>\n<LI><A\x20HREF=\"root
SF:/\">root/</A>\n<LI><A\x20HREF=\"sbin/\">sbin/</A>\n<LI><A\x20HREF=\"srv
SF:/\">srv/</A>\n<LI><A\x20HREF=\"sys/\">sys/</A>\n<LI><A\x20HREF=\"tmp/")
SF:%r(HTTPOptions,109,"\x1b\]0;@b2bd6545425e:\x20/\x07root@b2bd6545425e:/#
SF:\x20OPTIONS\x20/\x20HTTP/1\.0\nbash:\x20OPTIONS:\x20command\x20not\x20f
SF:ound\n\x1b\]0;@b2bd6545425e:\x20/\x07root@b2bd6545425e:/#\x20\n\x1b\]0;
SF:@b2bd6545425e:\x20/\x07root@b2bd6545425e:/#\x20\n\x1b\]0;@b2bd6545425e:
SF:\x20/\x07root@b2bd6545425e:/#\x20\n\x1b\]0;@b2bd6545425e:\x20/\x07root@
SF:b2bd6545425e:/#\x20")%r(RTSPRequest,109,"\x1b\]0;@b2bd6545425e:\x20/\x0
SF:7root@b2bd6545425e:/#\x20OPTIONS\x20/\x20RTSP/1\.0\nbash:\x20OPTIONS:\x
SF:20command\x20not\x20found\n\x1b\]0;@b2bd6545425e:\x20/\x07root@b2bd6545
SF:425e:/#\x20\n\x1b\]0;@b2bd6545425e:\x20/\x07root@b2bd6545425e:/#\x20\n\
SF:x1b\]0;@b2bd6545425e:\x20/\x07root@b2bd6545425e:/#\x20\n\x1b\]0;@b2bd65
SF:45425e:\x20/\x07root@b2bd6545425e:/#\x20");
MAC Address: 1A:EB:36:67:C3:40 (Unknown)
Device type: general purpose|router
Running: Linux 4.X|5.X, MikroTik RouterOS 7.X
OS CPE: cpe:/o:linux:linux_kernel:4 cpe:/o:linux:linux_kernel:5 cpe:/o:mikrotik:                                                                                                                                                                             routeros:7 cpe:/o:linux:linux_kernel:5.6.3
OS details: Linux 4.15 - 5.19, OpenWrt 21.02 (Linux 5.4), MikroTik RouterOS 7.2                                                                                                                                                                              - 7.5 (Linux 5.6.3)
TCP/IP fingerprint:
OS:SCAN(V=7.95%E=4%D=5/21%OT=21%CT=1%CU=34777%PV=Y%DS=1%DC=D%G=Y%M=1AEB36%T
OS:M=682E35AE%P=x86_64-pc-linux-gnu)SEQ(SP=101%GCD=1%ISR=10F%TI=Z%CI=Z%II=I
OS:%TS=A)OPS(O1=M5B4ST11NW7%O2=M5B4ST11NW7%O3=M5B4NNT11NW7%O4=M5B4ST11NW7%O
OS:5=M5B4ST11NW7%O6=M5B4ST11)WIN(W1=FE88%W2=FE88%W3=FE88%W4=FE88%W5=FE88%W6
OS:=FE88)ECN(R=Y%DF=Y%T=40%W=FAF0%O=M5B4NNSNW7%CC=Y%Q=)T1(R=Y%DF=Y%T=40%S=O
OS:%A=S+%F=AS%RD=0%Q=)T2(R=N)T3(R=N)T4(R=Y%DF=Y%T=40%W=0%S=A%A=Z%F=R%O=%RD=
OS:0%Q=)T5(R=Y%DF=Y%T=40%W=0%S=Z%A=S+%F=AR%O=%RD=0%Q=)T6(R=Y%DF=Y%T=40%W=0%
OS:S=A%A=Z%F=R%O=%RD=0%Q=)T7(R=Y%DF=Y%T=40%W=0%S=Z%A=S+%F=AR%O=%RD=0%Q=)U1(
OS:R=Y%DF=N%T=40%IPL=164%UN=0%RIPL=G%RID=G%RIPCK=G%RUCK=G%RUD=G)IE(R=Y%DFI=
OS:N%T=40%CD=S)

Uptime guess: 46.300 days (since Sat Apr  5 16:08:53 2025)
Network Distance: 1 hop
TCP Sequence Prediction: Difficulty=257 (Good luck!)
IP ID Sequence Generation: All zeros
Service Info: Hosts:  metasploitable.localdomain, irc.Metasploitable.LAN; OSs: U                                                                                                                                                                             nix, Linux; CPE: cpe:/o:linux:linux_kernel

Host script results:
|_smb2-time: Protocol negotiation failed (SMB2)
|_smb2-security-mode: Couldn't establish a SMBv2 connection.
| smb-security-mode:
|   account_used: guest
|   authentication_level: user
|   challenge_response: supported
|_  message_signing: disabled (dangerous, but default)
| smb-os-discovery:
|   OS: Unix (Samba 3.0.20-Debian)
|   Computer name: b2bd6545425e
|   NetBIOS computer name:
|   Domain name:
|   FQDN: b2bd6545425e
|_  System time: 2025-05-21T16:20:54-04:00
| p2p-conficker:
|   Checking for Conficker.C or higher...
|   Check 1 (port 47320/tcp): CLEAN (Couldn't connect)
|   Check 2 (port 39256/tcp): CLEAN (Couldn't connect)
|   Check 3 (port 40039/udp): CLEAN (Failed to receive data)
|   Check 4 (port 33974/udp): CLEAN (Failed to receive data)
|_  0/4 checks are positive: Host is CLEAN or ports are blocked
|_clock-skew: mean: 1h00m00s, deviation: 2h00m00s, median: 0s
| nbstat: NetBIOS name: B2BD6545425E, NetBIOS user: <unknown>, NetBIOS MAC: <unk                                                                                                                                                                             nown> (unknown)
| Names:
|   B2BD6545425E<00>     Flags: <unique><active>
|   B2BD6545425E<03>     Flags: <unique><active>
|   B2BD6545425E<20>     Flags: <unique><active>
|   WORKGROUP<00>        Flags: <group><active>
|   WORKGROUP<1e>        Flags: <group><active>
| Statistics:
|   00:00:00:00:00:00:00:00:00:00:00:00:00:00:00:00:00
|   00:00:00:00:00:00:00:00:00:00:00:00:00:00:00:00:00
|_  00:00:00:00:00:00:00:00:00:00:00:00:00:00

TRACEROUTE
HOP RTT     ADDRESS
1   1.74 ms metasploitable.lab.rtu.lv (192.168.1.11)

NSE: Script Post-scanning.
NSE: Starting runlevel 1 (of 3) scan.
Initiating NSE at 23:21
Completed NSE at 23:21, 0.00s elapsed
NSE: Starting runlevel 2 (of 3) scan.
Initiating NSE at 23:21
Completed NSE at 23:21, 0.00s elapsed
NSE: Starting runlevel 3 (of 3) scan.
Initiating NSE at 23:21
Completed NSE at 23:21, 0.00s elapsed
Read data files from: /usr/share/nmap
OS and Service detection performed. Please report any incorrect results at https                                                                                                                                                                             ://nmap.org/submit/ .
Nmap done: 1 IP address (1 host up) scanned in 162.32 seconds
           Raw packets sent: 1023 (45.806KB) | Rcvd: 1015 (41.354KB)

```
