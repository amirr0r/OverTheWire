# [Bandit](http://overthewire.org/wargames/bandit)

The Bandit wargame is aimed at absolute beginners.

## Summary
- [ ] [Level 0](#level-0)
- [ ] [Level 0 → Level 1](#level-0--level-1)
- [ ] [Level 1 → Level 2](#level-1--level-2)
- [ ] [Level 2 → Level 3](#level-2--level-3)
- [ ] [Level 3 → Level 4](#level-3--level-4)
- [ ] [Level 4 → Level 5](#level-4--level-5)
- [ ] [Level 5 → Level 6](#level-5--level-6)
- [ ] [Level 6 → Level 7](#level-6--level-7)
- [ ] [Level 7 → Level 8](#level-7--level-8)
- [ ] [Level 8 → Level 9](#level-8--level-9)
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
---
### [Level 0 → Level 1](http://overthewire.org/wargames/bandit/bandit1.html)
---
### [Level 1 → Level 2](http://overthewire.org/wargames/bandit/bandit2.html)
---
### [Level 2 → Level 3](http://overthewire.org/wargames/bandit/bandit3.html)
---
### [Level 3 → Level 4](http://overthewire.org/wargames/bandit/bandit4.html)
---
### [Level 4 → Level 5](http://overthewire.org/wargames/bandit/bandit5.html)
---
### [Level 5 → Level 6](http://overthewire.org/wargames/bandit/bandit6.html)
---
### [Level 6 → Level 7](http://overthewire.org/wargames/bandit/bandit7.html)
---
### [Level 7 → Level 8](http://overthewire.org/wargames/bandit/bandit8.html)
---
### [Level 8 → Level 9](http://overthewire.org/wargames/bandit/bandit9.html)
---
### [Level 9 → Level 10](http://overthewire.org/wargames/bandit/bandit10.html)
---
### [Level 10 → Level 11](http://overthewire.org/wargames/bandit/bandit11.html)
---
### [Level 11 → Level 12](http://overthewire.org/wargames/bandit/bandit12.html)
---
### [Level 12 → Level 13](http://overthewire.org/wargames/bandit/bandit13.html)
---
### [Level 13 → Level 14](http://overthewire.org/wargames/bandit/bandit14.html)
---
### [Level 14 → Level 15](http://overthewire.org/wargames/bandit/bandit15.html)
---
### [Level 15 → Level 16](http://overthewire.org/wargames/bandit/bandit16.html)
---
### [Level 16 → Level 17](http://overthewire.org/wargames/bandit/bandit17.html)
---
### [Level 17 → Level 18](http://overthewire.org/wargames/bandit/bandit18.html)
---
### [Level 18 → Level 19](http://overthewire.org/wargames/bandit/bandit19.html)
---
### [Level 19 → Level 20](http://overthewire.org/wargames/bandit/bandit20.html)
---
### [Level 20 → Level 21](http://overthewire.org/wargames/bandit/bandit21.html)
---
### [Level 21 → Level 22](http://overthewire.org/wargames/bandit/bandit22.html)
---
### [Level 22 → Level 23](http://overthewire.org/wargames/bandit/bandit23.html)
---
### [Level 23 → Level 24](http://overthewire.org/wargames/bandit/bandit24.html)
---
### [Level 24 → Level 25](http://overthewire.org/wargames/bandit/bandit25.html)
---
### [Level 25 → Level 26](http://overthewire.org/wargames/bandit/bandit26.html)
---
### [Level 26 → Level 27](http://overthewire.org/wargames/bandit/bandit27.html)
---
### [Level 27 → Level 28](http://overthewire.org/wargames/bandit/bandit28.html)
---
### [Level 28 → Level 29](http://overthewire.org/wargames/bandit/bandit29.html)
---
### [Level 29 → Level 30](http://overthewire.org/wargames/bandit/bandit30.html)
---
### [Level 30 → Level 31](http://overthewire.org/wargames/bandit/bandit31.html)
---
### [Level 31 → Level 32](http://overthewire.org/wargames/bandit/bandit32.html)
---
