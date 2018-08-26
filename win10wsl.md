https://docs.microsoft.com/en-us/windows/wsl/about

https://docs.microsoft.com/en-us/windows/wsl/install-win10

Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux

https://docs.microsoft.com/en-us/windows/wsl/troubleshooting#check-your-build-number

```
XPS 15 9560 Signature Edition
Edition       Windows 10 Pro
Version       1803
Installed on  6/19/2018
OS build      171134.165

davidho@LAPTOP-H2R4EKMU:~$
davidho@LAPTOP-H2R4EKMU:~$ date
Sun Aug 26 09:22:10 DST 2018
davidho@LAPTOP-H2R4EKMU:~$ pwd -P
/home/davidho
davidho@LAPTOP-H2R4EKMU:~$ uname -a
Linux LAPTOP-H2R4EKMU 4.4.0-17134-Microsoft #137-Microsoft Thu Jun 14 18:46:00 PST 2018 x86_64 x86_64 x86_64 GNU/Linux
davidho@LAPTOP-H2R4EKMU:~$
davidho@LAPTOP-H2R4EKMU:~$ ls -latr
total 8
drwxr-xr-x 1 root    root     512 Aug 25 13:35 ..
-rw-r--r-- 1 davidho davidho  220 Aug 25 13:35 .bash_logout
-rw-r--r-- 1 davidho davidho  807 Aug 25 13:35 .profile
-rw-r--r-- 1 davidho davidho 3771 Aug 25 13:35 .bashrc
drwxr-xr-x 1 davidho davidho  512 Aug 25 13:35 .
davidho@LAPTOP-H2R4EKMU:~$
davidho@LAPTOP-H2R4EKMU:~$ ls -latr /
total 88
-rwxr-xr-x  1 root root 87944 Dec 31  1969 init
drwxr-xr-x  1 root root   512 Jul 19 06:05 snap
drwxr-xr-x  1 root root   512 Jul 25 11:50 usr
drwxr-xr-x  1 root root   512 Jul 25 11:50 srv
drwxr-xr-x  1 root root   512 Jul 25 11:50 opt
drwxr-xr-x  1 root root   512 Jul 25 11:50 media
drwxr-xr-x  1 root root   512 Jul 25 11:51 lib64
drwxr-xr-x  1 root root   512 Jul 25 11:53 lib
drwxr-xr-x  1 root root   512 Jul 25 11:54 var
drwx------  1 root root   512 Jul 25 11:54 root
drwxr-xr-x  1 root root   512 Jul 25 11:54 sbin
drwxr-xr-x  1 root root   512 Jul 25 11:56 boot
drwxr-xr-x  1 root root   512 Aug 25 13:34 ..
drwxr-xr-x  1 root root   512 Aug 25 13:34 .
drwxr-xr-x  1 root root   512 Aug 25 13:34 bin
drwxr-xr-x  1 root root   512 Aug 25 13:34 mnt
drwxr-xr-x  1 root root   512 Aug 25 13:35 home
drwxr-xr-x  1 root root   512 Aug 25 13:35 etc
dr-xr-xr-x 12 root root     0 Aug 25 13:35 sys
dr-xr-xr-x  9 root root     0 Aug 25 13:35 proc
drwxr-xr-x  1 root root   512 Aug 25 13:35 run
drwxr-xr-x  1 root root   512 Aug 25 13:35 dev
drwxrwxrwt  1 root root   512 Aug 25 13:35 tmp
davidho@LAPTOP-H2R4EKMU:~$
davidho@LAPTOP-H2R4EKMU:~$ cat /etc/lsb-release
DISTRIB_ID=Ubuntu
DISTRIB_RELEASE=18.04
DISTRIB_CODENAME=bionic
DISTRIB_DESCRIPTION="Ubuntu 18.04.1 LTS"
davidho@LAPTOP-H2R4EKMU:~$
davidho@LAPTOP-H2R4EKMU:~$ cat /etc/os-release
NAME="Ubuntu"
VERSION="18.04.1 LTS (Bionic Beaver)"
ID=ubuntu
ID_LIKE=debian
PRETTY_NAME="Ubuntu 18.04.1 LTS"
VERSION_ID="18.04"
HOME_URL="https://www.ubuntu.com/"
SUPPORT_URL="https://help.ubuntu.com/"
BUG_REPORT_URL="https://bugs.launchpad.net/ubuntu/"
PRIVACY_POLICY_URL="https://www.ubuntu.com/legal/terms-and-policies/privacy-policy"
VERSION_CODENAME=bionic
UBUNTU_CODENAME=bionic
davidho@LAPTOP-H2R4EKMU:~$
```
