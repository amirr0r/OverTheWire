# [Bandit](http://overthewire.org/wargames/bandit)

The Bandit wargame is aimed at absolute beginners.

## Summary
- [x] [Level 0](#level-0)
- [x] [Level 0 → Level 1](#level-0--level-1)
- [x] [Level 1 → Level 2](#level-1--level-2)
- [x] [Level 2 → Level 3](#level-2--level-3)
- [x] [Level 3 → Level 4](#level-3--level-4)
- [x] [Level 4 → Level 5](#level-4--level-5)
- [x] [Level 5 → Level 6](#level-5--level-6)
- [x] [Level 6 → Level 7](#level-6--level-7)
- [x] [Level 7 → Level 8](#level-7--level-8)
- [x] [Level 8 → Level 9](#level-8--level-9)
- [ ] [Level 9 → Level 10](#level-9--level-10)
- [ ] [Level 10 → Level 11](#level-10--level-11)
- [ ] [Level 11 → Level 12](#level-11--level-12)
- [ ] [Level 12 → Level 13](#level-12--level-13)
- [ ] [Level 13 → Level 14](#level-13--level-14)
- [ ] [Level 14 → Level 15](#level-14--level-15)
- [ ] [Level 15 → Level 16](#level-15--level-16)
- [ ] [Level 16 → Level 17](#level-16--level-17)
- [ ] [Level 17 → Level 18](#level-17--level-18)
- [ ] [Level 18 → Level 19](#level-18--level-19)
- [ ] [Level 19 → Level 20](#level-19--level-20)
- [ ] [Level 20 → Level 21](#level-20--level-21)
- [ ] [Level 21 → Level 22](#level-21--level-22)
- [ ] [Level 22 → Level 23](#level-22--level-23)
- [ ] [Level 23 → Level 24](#level-23--level-24)
- [ ] [Level 24 → Level 25](#level-24--level-25)
- [ ] [Level 25 → Level 26](#level-25--level-26)
- [ ] [Level 26 → Level 27](#level-26--level-27)
- [ ] [Level 27 → Level 28](#level-27--level-28)
- [ ] [Level 28 → Level 29](#level-28--level-29)
- [ ] [Level 29 → Level 30](#level-29--level-30)
- [ ] [Level 30 → Level 31](#level-30--level-31)
- [ ] [Level 31 → Level 32](#level-31--level-32)

## Wargames
Checkout this : [SSH from your Browser](https://shellngn.com/)
```bash
$ tldr ssh

  ssh

  Secure Shell is a protocol used to securely log onto remote systems.
  It can be used for logging or executing commands on a remote server.

  - Connect to a remote server:
    ssh username@remote_host

  - Connect to a remote server with a specific identity (private key):
    ssh -i path/to/key_file username@remote_host

  - Connect to a remote server using a specific port:
    ssh username@remote_host -p 2222

  - Run a command on a remote server:
    ssh remote_host command -with -flags

  - SSH tunneling: Dynamic port forwarding (SOCKS proxy on localhost:9999):
    ssh -D 9999 -C username@remote_host

  - SSH tunneling: Forward a specific port (localhost:9999 to slashdot.org:80) along with disabling pseudo-[t]ty allocation and executio[n] of remote commands:
    ssh -L 9999:slashdot.org:80 -N -T username@remote_host

  - SSH jumping: Connect through a jumphost to a remote server (Multiple jump hops may be specified separated by comma characters):
    ssh -J username@jump_host username@remote_host

  - Agent forwarding: Forward the authentication information to the remote machine (see man ssh_config for available options):
    ssh -A username@remote_host
```

### [Level 0](http://overthewire.org/wargames/bandit/bandit0.html)
```bash
$ ssh bandit0@bandit.labs.overthewire.org -p 2220
```
---
### [Level 0 → Level 1](http://overthewire.org/wargames/bandit/bandit1.html)
```bash
# bandit0@bandit.labs.overthewire.org's password:
bandit0@bandit:~$ ls
readme
bandit0@bandit:~$ cat readme
boJ9jbbUNNfktd78OOpsqOltutMc3MY1
```
---
### [Level 1 → Level 2](http://overthewire.org/wargames/bandit/bandit2.html)
```bash
bandit1@bandit:~$ ls      
-
bandit1@bandit:~$ ls -la
total 24
-rw-r-----  1 bandit2 bandit1   33 Dec 28  2017 -
drwxr-xr-x  2 root    root    4096 Dec 28  2017 .
drwxr-xr-x 34 root    root    4096 Jul 15 20:51 ..
-rw-r--r--  1 root    root     220 Sep  1  2015 .bash_logout
-rw-r--r--  1 root    root    3771 Sep  1  2015 .bashrc
-rw-r--r--  1 root    root     655 Jun 24  2016 .profile
bandit1@bandit:~$ cat -
^C
bandit1@bandit:~$ # too long, let's try with vim
bandit1@bandit:~$ vim -
Vim: Reading from stdin...
^C^C^C^C^C
bandit1@bandit:~$ # too long, let's try another way
bandit1@bandit:~$ cat ./-
CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9
```
---
### [Level 2 → Level 3](http://overthewire.org/wargames/bandit/bandit3.html)
```
bandit2@bandit:~$ ls
spaces in this filename
bandit2@bandit:~$ cat "spaces in this filename" 
UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK
bandit2@bandit:~$
```
---
### [Level 3 → Level 4](http://overthewire.org/wargames/bandit/bandit4.html)
```bash
bandit3@bandit:~$ ls
inhere
bandit3@bandit:~$ cd inhere/
bandit3@bandit:~/inhere$ ls
bandit3@bandit:~/inhere$ ls -a
.  ..  .hidden
bandit3@bandit:~/inhere$ cat .hidden 
pIwrPrtPN36QITSp3EQaw936yaFoFgAB
bandit3@bandit:~/inhere$ 
```
---
### [Level 4 → Level 5](http://overthewire.org/wargames/bandit/bandit5.html)
```
bandit4@bandit:~$ ls
inhere
bandit4@bandit:~$ cd inhere/
bandit4@bandit:~/inhere$ ls
-file00  -file01  -file02  -file03  -file04  -file05  -file06  -file07  -file08  -file09
bandit4@bandit:~/inhere$ cat ./*
ykC6q�+���z�C|���M�     �rkA����A����L�
                                       ��]�SN?�r+�l��2��iń:5���mp6�W{�
                                                                             /�
                                                                               �����%�R�O��,-�
                                                                                                ����t���T��W��Lv�<d���3q�
                                                                                                                         &�=�[_��`ɝ�m�=�`�V�zs�9��_o˔�M@�Z������� ���VƊ\%��+��!G kT�8��Õxj�ys�Ƶ�ʑjꮥOkoReBOKuIDDepwhWk7jZC0RTdopnAYKh
����&��ڛ���[̹2��~!\ �����   R��
                              P���к1�=?G0���D���Ui,�Wbandit4@bandit:~/inhere$ # ...
bandit4@bandit:~/inhere$ cat ./"-file07"
koReBOKuIDDepwhWk7jZC0RTdopnAYKh
bandit4@bandit:~/inhere$ 
```
---
### [Level 5 → Level 6](http://overthewire.org/wargames/bandit/bandit6.html)
```bash
bandit5@bandit:~$ ls
inhere
bandit5@bandit:~$ cd inhere/
bandit5@bandit:~/inhere$ ls
maybehere00  maybehere02  maybehere04  maybehere06  maybehere08  maybehere10  maybehere12  maybehere14  maybehere16  maybehere18
maybehere01  maybehere03  maybehere05  maybehere07  maybehere09  maybehere11  maybehere13  maybehere15  maybehere17  maybehere19
bandit5@bandit:~/inhere$ # lol, we know the filesize is 1033 bytes. Let's try with the find command
bandit5@bandit:~/inhere$ man find
bandit5@bandit:~/inhere$ find . -size 1033c
./maybehere07/.file2
bandit5@bandit:~/inhere$ cat ./maybehere07/.file2
DXjZPULLxYr17uwoI01bNLQbtFemEgo7
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        bandit5@bandit:~/inhere$
```
---
### [Level 6 → Level 7](http://overthewire.org/wargames/bandit/bandit7.html)
Check [How can I exclude all *"permission denied"* messages from **"find"** ?](https://stackoverflow.com/questions/762348/how-can-i-exclude-all-permission-denied-messages-from-find)
```bash
bandit6@bandit:~$ find / -user bandit7 -group bandit6 -size 33c
find: '/etc/ssl/private': Permission denied
find: '/etc/polkit-1/localauthority': Permission denied
find: '/run/lxcfs': Permission denied
find: '/run/user/11007': Permission denied
find: '/run/user/11002': Permission denied
#...
bandit6@bandit:~$ find / -user bandit7 -group bandit6 -size 33c 2>/dev/null
/var/lib/dpkg/info/bandit7.password
bandit6@bandit:~$ cat /var/lib/dpkg/info/bandit7.password
HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs
bandit6@bandit:~$ 
```
---
### [Level 7 → Level 8](http://overthewire.org/wargames/bandit/bandit8.html)
```bash
bandit7@bandit:~$ ls
data.txt
bandit7@bandit:~$ cat data.txt | grep "millionth"
millionth       cvX2JJa4CFALtqS87jk27qwqGhBM9plV
```
---
### [Level 8 → Level 9](http://overthewire.org/wargames/bandit/bandit9.html)
Thanks to [tldr uniq](https://tldr.ostera.io/uniq)
```bash
bandit8@bandit:~$ sort data.txt | uniq -u
UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR
bandit8@bandit:~$ 
```
---
### [Level 9 → Level 10](http://overthewire.org/wargames/bandit/bandit10.html)
```bash

```
---
### [Level 10 → Level 11](http://overthewire.org/wargames/bandit/bandit11.html)
```bash

```
---
### [Level 11 → Level 12](http://overthewire.org/wargames/bandit/bandit12.html)
```bash

```
---
### [Level 12 → Level 13](http://overthewire.org/wargames/bandit/bandit13.html)
```bash

```
---
### [Level 13 → Level 14](http://overthewire.org/wargames/bandit/bandit14.html)
```bash

```
---
### [Level 14 → Level 15](http://overthewire.org/wargames/bandit/bandit15.html)
```bash

```
---
### [Level 15 → Level 16](http://overthewire.org/wargames/bandit/bandit16.html)
```bash

```
---
### [Level 16 → Level 17](http://overthewire.org/wargames/bandit/bandit17.html)
```bash

```
---
### [Level 17 → Level 18](http://overthewire.org/wargames/bandit/bandit18.html)
```bash

```
---
### [Level 18 → Level 19](http://overthewire.org/wargames/bandit/bandit19.html)
```bash

```
---
### [Level 19 → Level 20](http://overthewire.org/wargames/bandit/bandit20.html)
```bash

```
---
### [Level 20 → Level 21](http://overthewire.org/wargames/bandit/bandit21.html)
```bash

```
---
### [Level 21 → Level 22](http://overthewire.org/wargames/bandit/bandit22.html)
```bash

```
---
### [Level 22 → Level 23](http://overthewire.org/wargames/bandit/bandit23.html)
```bash

```
---
### [Level 23 → Level 24](http://overthewire.org/wargames/bandit/bandit24.html)
```bash

```
---
### [Level 24 → Level 25](http://overthewire.org/wargames/bandit/bandit25.html)
```bash

```
---
### [Level 25 → Level 26](http://overthewire.org/wargames/bandit/bandit26.html)
```bash

```
---
### [Level 26 → Level 27](http://overthewire.org/wargames/bandit/bandit27.html)
```bash

```
---
### [Level 27 → Level 28](http://overthewire.org/wargames/bandit/bandit28.html)
```bash

```
---
### [Level 28 → Level 29](http://overthewire.org/wargames/bandit/bandit29.html)
```bash

```
---
### [Level 29 → Level 30](http://overthewire.org/wargames/bandit/bandit30.html)
```bash

```
---
### [Level 30 → Level 31](http://overthewire.org/wargames/bandit/bandit31.html)
```bash

```
---
### [Level 31 → Level 32](http://overthewire.org/wargames/bandit/bandit32.html)
```bash

```
---
