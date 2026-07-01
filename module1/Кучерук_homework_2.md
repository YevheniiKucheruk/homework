Домашнє завдання №2. Файлова система і права доступу
Студент: Кучерук Євгеній Романович

Завдання 1: Ієрархія каталогів Linux (1 бал)
    Перейди в кореневий каталог / і покажи вміст;

root@ubuntu:~$ cd /
root@ubuntu:/$ ls -la
total 1048664
drwxr-xr-x  22 root root       4096 Jun 20 08:53 .
drwxr-xr-x  22 root root       4096 Jun 20 08:53 ..
lrwxrwxrwx   1 root root          7 Apr 22  2024 bin -> usr/bin
drwxr-xr-x   2 root root       4096 Feb 26  2024 bin.usr-is-merged
drwxr-xr-x   5 root root       4096 Jun 20 08:52 boot
drwxr-xr-x  17 root root       3820 Jul  1 13:53 dev
drwxr-xr-x 118 root root       4096 Jul  1 13:53 etc
drwxr-xr-x   3 root root       4096 Jun 17 06:25 home
lrwxrwxrwx   1 root root          7 Apr 22  2024 lib -> usr/lib
drwxr-xr-x   2 root root       4096 Apr  8  2024 lib.usr-is-merged
lrwxrwxrwx   1 root root          9 Apr 22  2024 lib64 -> usr/lib64
drwx------   2 root root      16384 May 18 13:00 lost+found
drwxr-xr-x   2 root root       4096 May 18 12:57 media
drwxr-xr-x   2 root root       4096 May 18 12:57 mnt
drwxr-xr-x   5 root root       4096 Jul  1 13:53 opt
dr-xr-xr-x 184 root root          0 Jul  1 13:53 proc
drwx------   4 root root       4096 Jun 20 08:54 root
drwxr-xr-x  37 root root       1000 Jul  1 14:06 run
lrwxrwxrwx   1 root root          8 Apr 22  2024 sbin -> usr/sbin
drwxr-xr-x   2 root root       4096 Mar 31  2024 sbin.usr-is-merged
drwxr-xr-x   2 root root       4096 Jun 17 06:25 snap
drwxr-xr-x   2 root root       4096 May 18 12:57 srv
-rw-------   1 root root 1073741824 Jul  1 13:53 swapfile
dr-xr-xr-x  13 root root          0 Jul  1 13:53 sys
drwxrwxrwt  14 root root       4096 Jul  1 14:11 tmp
drwxr-xr-x  12 root root       4096 May 18 12:57 usr
drwxr-xr-x  12 root root       4096 Jun 20 08:52 var
root@ubuntu:/$ 

    Перейди в /etc і покажи вміст;

root@ubuntu:/etc$ cd /etc
root@ubuntu:/etc$ ls -la
total 1004
drwxr-xr-x 118 root root       4096 Jul  1 13:53 .
drwxr-xr-x  22 root root       4096 Jun 20 08:53 ..
-rw-------   1 root root          0 May 18 12:57 .pwd.lock
-rw-r--r--   1 root root        862 May 18 12:57 .resolv.conf.systemd-resolved.bak
-rw-r--r--   1 root root        208 May 18 12:57 .updated
drwxr-xr-x   4 root root       4096 May 18 12:59 ModemManager
drwxr-xr-x   3 root root       4096 Jun 20 08:52 NetworkManager
drwxr-xr-x   2 root root       4096 May 18 12:59 PackageKit
drwxr-xr-x   4 root root       4096 May 18 12:57 X11
-rw-r--r--   1 root root       3444 Jul  5  2023 adduser.conf
drwxr-xr-x   2 root root       4096 Jun 20 08:53 alternatives
drwxr-xr-x   3 root root       4096 Jun 20 08:53 apache2
drwxr-xr-x   2 root root       4096 Jun 20 08:53 apparmor
drwxr-xr-x   9 root root      12288 Jun 20 08:53 apparmor.d
drwxr-xr-x   3 root root       4096 May 18 12:59 apport
drwxr-xr-x   8 root root       4096 May 18 13:01 apt
-rw-r--r--   1 root root       2319 Mar 31  2024 bash.bashrc
-rw-r--r--   1 root root         45 Jan 24  2020 bash_completion
drwxr-xr-x   2 root root       4096 May 18 12:59 bash_completion.d
-rw-r--r--   1 root root        367 Aug  2  2022 bindresvport.blacklist
drwxr-xr-x   2 root root       4096 Apr 19  2024 binfmt.d
drwxr-xr-x   2 root root       4096 May 18 12:59 byobu
drwxr-xr-x   3 root root       4096 May 18 12:57 ca-certificates
-rw-r--r--   1 root root       6862 Jun 20 08:52 ca-certificates.conf
-rw-r--r--   1 root root       6288 May 18 12:57 ca-certificates.conf.dpkg-old
drwxr-xr-x   5 root root       4096 Jun 20 08:52 cloud
drwxr-xr-x   3 root root       4096 Jun 20 08:53 cni
drwxr-xr-x   2 root root       4096 May 18 12:59 console-setup
drwxr-xr-x   3 root root       4096 Jun 20 08:53 containerd
drwxr-xr-x   5 root root       4096 Jun 20 08:53 containers
drwx------   2 root root       4096 Apr 19  2024 credstore
drwx------   2 root root       4096 Apr 19  2024 credstore.encrypted
-rw-r--r--   1 root root         57 Jun 20 08:53 crictl.yaml
drwxr-xr-x   2 root root       4096 Jun 20 08:53 cron.d
drwxr-xr-x   2 root root       4096 May 18 12:59 cron.daily
drwxr-xr-x   2 root root       4096 May 18 12:57 cron.hourly
drwxr-xr-x   2 root root       4096 May 18 12:57 cron.monthly
drwxr-xr-x   2 root root       4096 May 18 12:59 cron.weekly
drwxr-xr-x   2 root root       4096 May 18 12:57 cron.yearly
-rw-r--r--   1 root root       1188 Jun 20 08:54 crontab
drwxr-xr-x   2 root root       4096 May 18 12:59 cryptsetup-initramfs
-rw-r--r--   1 root root         54 May 18 12:58 crypttab
drwxr-xr-x   4 root root       4096 May 18 12:57 dbus-1
-rw-r--r--   1 root root       2967 Apr 12  2024 debconf.conf
-rw-r--r--   1 root root         11 Apr 22  2024 debian_version
drwxr-xr-x   3 root root       4096 Jun 20 08:53 default
-rw-r--r--   1 root root       1706 Jul  5  2023 deluser.conf
drwxr-xr-x   2 root root       4096 May 18 12:58 depmod.d
drwxr-xr-x   3 root root       4096 May 18 12:57 dhcp
-rw-r--r--   1 root root       1429 Mar 31  2024 dhcpcd.conf
drwxr-xr-x   3 root root       4096 Jun 20 08:53 dkms
drwxr-xr-x   2 root root       4096 Jun 20 08:53 dnsmasq.d
drwxr-xr-x   2 root root       4096 Jun 20 08:53 docker
drwxr-xr-x   4 root root       4096 Jun 20 08:53 dpkg
-rw-r--r--   1 root root        685 Apr  8  2024 e2scrub.conf
-rw-r--r--   1 root root         34 May 18 12:59 ec2_version
-rw-r--r--   1 root root        106 May 18 12:57 environment
-rw-r--r--   1 root root       1853 Oct 17  2022 ethertypes
drwxr-xr-x   4 root root       4096 May 18 12:59 fonts
-rw-r--r--   1 root root        146 May 18 13:00 fstab
-rw-r--r--   1 root root        694 Apr  8  2024 fuse.conf
drwxr-xr-x   4 root root       4096 Jun 20 08:52 fwupd
-rw-r--r--   1 root root       2584 Jan 31  2024 gai.conf
drwxr-xr-x   2 root root       4096 Jun 20 08:51 gnutls
-rw-r--r--   1 root root       3986 Feb  9 21:03 gprofng.rc
drwxr-xr-x   2 root root       4096 May 18 12:59 groff
-rw-r--r--   1 root root        843 Jun 20 08:53 group
-rw-r--r--   1 root root        829 Jun 17 06:25 group-
drwxr-xr-x   2 root root       4096 Jun 20 08:52 grub.d
-rw-r-----   1 root shadow      711 Jun 20 08:53 gshadow
-rw-r-----   1 root shadow      700 Jun 17 06:25 gshadow-
drwxr-xr-x   3 root root       4096 May 18 12:57 gss
-rw-r--r--   1 root root       4436 Oct  6  2022 hdparm.conf
-rw-r--r--   1 root root         92 Apr 22  2024 host.conf
-rw-r--r--   1 root root          7 Jun 20 08:52 hostname
-rw-r--r--   1 root root        255 Jun 20 08:52 hosts
-rw-r--r--   1 root root        411 May 18 12:59 hosts.allow
-rw-r--r--   1 root root        711 May 18 12:59 hosts.deny
drwxr-xr-x   2 root root       4096 Jun 20 08:53 init
drwxr-xr-x   2 root root       4096 Jun 20 08:53 init.d
drwxr-xr-x   5 root root       4096 May 18 12:59 initramfs-tools
-rw-r--r--   1 root root       1875 Mar 31  2024 inputrc
drwxr-xr-x   4 root root       4096 May 18 12:58 iproute2
drwxr-xr-x   2 root root       4096 May 18 12:59 iscsi
-rw-r--r--   1 root root         26 Feb  6 07:23 issue
-rw-r--r--   1 root root         19 Feb  6 07:23 issue.net
drwxr-xr-x   7 root root       4096 Jun 20 08:53 kernel
drwxr-xr-x   2 root root       4096 Jul  1 13:53 killercoda
drwxrwxr-x   2 root landscape  4096 Aug 21  2025 landscape
-rw-r--r--   1 root root      25915 Jun 20 08:53 ld.so.cache
-rw-r--r--   1 root root         34 Aug  2  2022 ld.so.conf
drwxr-xr-x   2 root root       4096 Jun 20 08:53 ld.so.conf.d
drwxr-xr-x   2 root root       4096 May 18 12:59 ldap
-rw-r--r--   1 root root        267 Apr 22  2024 legal
-rw-r--r--   1 root root        191 Mar 31  2024 libaudit.conf
drwxr-xr-x   3 root root       4096 May 18 12:59 libblockdev
drwxr-xr-x   2 root root       4096 May 18 12:59 libibverbs.d
drwxr-xr-x   2 root root       4096 May 18 12:59 libnl-3
drwxr-xr-x   4 root root       4096 Jun 20 08:53 lighttpd
-rw-r--r--   1 root root       2996 Mar 30  2024 locale.alias
-rw-r--r--   1 root root         13 May 18 12:59 locale.conf
-rw-r--r--   1 root root       9563 May 18 12:59 locale.gen
lrwxrwxrwx   1 root root         27 May 18 12:57 localtime -> /usr/share/zoneinfo/Etc/UTC
drwxr-xr-x   4 root root       4096 May 18 12:59 logcheck
-rw-r--r--   1 root root      12345 Feb 22  2024 login.defs
-rw-r--r--   1 root root        586 Apr  8  2024 logrotate.conf
drwxr-xr-x   2 root root       4096 Jun 20 08:52 logrotate.d
-rw-r--r--   1 root root        104 Feb  6 07:22 lsb-release
drwxr-xr-x   3 root root       4096 May 18 12:59 lvm
-r--r--r--   1 root root         33 Jun 17 06:25 machine-id
-rw-r--r--   1 root root        111 Mar 31  2024 magic
-rw-r--r--   1 root root        111 Mar 31  2024 magic.mime
-rw-r--r--   1 root root       5230 Apr  8  2024 manpath.config
drwxr-xr-x   2 root root       4096 May 18 12:59 mdadm
-rw-r--r--   1 root root      75113 Jul 12  2023 mime.types
-rw-r--r--   1 root root        744 Apr  8  2024 mke2fs.conf
drwxr-xr-x   2 root root       4096 Jun 20 08:53 modprobe.d
-rw-r--r--   1 root root        212 May 18 12:57 modules
drwxr-xr-x   2 root root       4096 Jun 20 08:53 modules-load.d
lrwxrwxrwx   1 root root         19 May 18 12:57 mtab -> ../proc/self/mounts
drwx------   2 root root       4096 Jun 17 06:25 multipath
-rw-r--r--   1 root root         41 Jul 22  2025 multipath.conf
-rw-r--r--   1 root root      11424 May 23  2023 nanorc
drwxr-xr-x   6 root root       4096 May 18 12:59 needrestart
-rw-r--r--   1 root root        767 Mar 31  2024 netconfig
drwxr-xr-x   2 root root       4096 Jun 17 06:25 netplan
drwxr-xr-x   6 root root       4096 Jun 20 08:53 network
drwxr-xr-x   8 root root       4096 May 18 12:57 networkd-dispatcher
-rw-r--r--   1 root root         91 Apr 22  2024 networks
drwxr-xr-x   2 root root       4096 May 18 12:57 newt
-rwxr-xr-x   1 root root        243 Oct 19  2023 nftables.conf
-rw-r--r--   1 root root        526 May 18 12:57 nsswitch.conf
drwxr-xr-x   2 root root       4096 May 18 12:57 opt
lrwxrwxrwx   1 root root         21 Feb  6 07:23 os-release -> ../usr/lib/os-release
-rw-r--r--   1 root root       6920 Jul  3  2024 overlayroot.conf
-rw-r--r--   1 root root        112 May 18 13:00 overlayroot.local.conf
-rw-r--r--   1 root root        552 Oct 13  2022 pam.conf
drwxr-xr-x   2 root root       4096 Jun 20 08:52 pam.d
-rw-r--r--   1 root root       1776 Jun 20 08:52 passwd
-rw-r--r--   1 root root       1716 Jun 17 06:25 passwd-
drwxr-xr-x   3 root root       4096 May 18 12:58 perl
drwxr-xr-x   3 root root       4096 Jun 20 08:53 php
drwxr-xr-x   4 root root       4096 May 18 12:58 pki
drwxr-xr-x   2 root root       4096 Feb 25  2025 plymouth
drwxr-xr-x   3 root root       4096 May 18 12:58 pm
drwxr-xr-x   3 root root       4096 May 18 12:59 polkit-1
drwxr-xr-x   2 root root       4096 Mar 26 12:25 pollinate
-rw-r--r--   1 root root        582 Apr 22  2024 profile
drwxr-xr-x   2 root root       4096 Jun 20 08:52 profile.d
-rw-r--r--   1 root root       3144 Oct 17  2022 protocols
drwxr-xr-x   2 root root       4096 May 18 12:58 python3
drwxr-xr-x   2 root root       4096 May 18 12:58 python3.12
drwxr-xr-x   2 root root       4096 Jun 20 08:53 rc0.d
drwxr-xr-x   2 root root       4096 Jun 20 08:53 rc1.d
drwxr-xr-x   2 root root       4096 Jun 20 08:53 rc2.d
drwxr-xr-x   2 root root       4096 Jun 20 08:53 rc3.d
drwxr-xr-x   2 root root       4096 Jun 20 08:53 rc4.d
drwxr-xr-x   2 root root       4096 Jun 20 08:53 rc5.d
drwxr-xr-x   2 root root       4096 Jun 20 08:53 rc6.d
drwxr-xr-x   2 root root       4096 May 18 12:59 rcS.d
lrwxrwxrwx   1 root root         32 Jul  1 13:53 resolv.conf -> /run/systemd/resolve/resolv.conf
lrwxrwxrwx   1 root root         13 Apr  8  2024 rmt -> /usr/sbin/rmt
-rw-r--r--   1 root root        911 Oct 17  2022 rpc
-rw-r--r--   1 root root       1213 Mar 22  2024 rsyslog.conf
drwxr-xr-x   2 root root       4096 Jun 20 08:52 rsyslog.d
-rw-r--r--   1 root root       3663 Jun 20  2016 screenrc
drwxr-xr-x   4 root root       4096 May 18 12:58 security
drwxr-xr-x   2 root root       4096 May 18 12:57 selinux
drwxr-xr-x   2 root root       4096 May 18 12:59 sensors.d
-rw-r--r--   1 root root      10593 Mar 31  2024 sensors3.conf
-rw-r--r--   1 root root      12813 Mar 27  2021 services
drwxr-xr-x   2 root root       4096 May 18 12:59 sgml
-rw-r-----   1 root shadow     1008 Jun 20 08:52 shadow
-rw-r-----   1 root shadow      986 Jun 17 06:25 shadow-
-rw-r--r--   1 root root        148 May 18 12:59 shells
drwxr-xr-x   2 root root       4096 May 18 12:57 skel
drwxr-xr-x   6 root root       4096 May 18 12:59 sos
drwxr-xr-x   4 root root       4096 Jun 17 06:25 ssh
drwxr-xr-x   4 root root       4096 Jun 20 08:52 ssl
-rw-r--r--   1 root root         20 Jun 17 06:25 subgid
-rw-r--r--   1 root root          0 May 18 12:57 subgid-
-rw-r--r--   1 root root         20 Jun 17 06:25 subuid
-rw-r--r--   1 root root          0 May 18 12:57 subuid-
-rw-r--r--   1 root root       4343 Apr  8  2024 sudo.conf
-rw-r--r--   1 root root       9804 Apr  8  2024 sudo_logsrvd.conf
-r--r-----   1 root root       1800 Jan 29  2024 sudoers
drwxr-x---   2 root root       4096 Jun 17 06:25 sudoers.d
drwxr-xr-x   2 root root       4096 May 18 12:57 supercat
-rw-r--r--   1 root root       2244 Jun 20 08:54 sysctl.conf
drwxr-xr-x   2 root root       4096 Jun 20 08:53 sysctl.d
drwxr-xr-x   2 root root       4096 May 18 12:59 sysstat
drwxr-xr-x   6 root root       4096 Jul  1 13:53 systemd
drwxr-xr-x   2 root root       4096 May 18 12:57 terminfo
-rw-r--r--   1 root root          8 May 18 12:58 timezone
drwxr-xr-x   2 root root       4096 May 18 12:59 tmpfiles.d
drwxr-xr-x   2 root root       4096 May 18 12:58 ubuntu-advantage
-rw-r--r--   1 root root       1260 Jan 27  2023 ucf.conf
drwxr-xr-x   4 root root       4096 Jun 20 08:52 udev
drwxr-xr-x   2 root root       4096 May 18 12:59 udisks2
drwxr-xr-x   3 root root       4096 May 18 12:59 ufw
drwxr-xr-x   3 root root       4096 May 18 12:59 update-manager
drwxr-xr-x   2 root root       4096 Jun 20 08:52 update-motd.d
drwxr-xr-x   2 root root       4096 Apr  2  2025 update-notifier
-rw-r--r--   1 root root       1523 Apr  8  2024 usb_modeswitch.conf
drwxr-xr-x   2 root root       4096 Dec 16  2023 usb_modeswitch.d
lrwxrwxrwx   1 root root         16 May 18 12:57 vconsole.conf -> default/keyboard
drwxr-xr-x   2 root root       4096 Jun 20 08:52 vim
drwxr-xr-x   4 root root       4096 May 18 12:59 vmware-tools
lrwxrwxrwx   1 root root         23 Feb 26  2024 vtrgb -> /etc/alternatives/vtrgb
-rw-r--r--   1 root root       4942 Jun 19  2024 wgetrc
-rw-r--r--   1 root root        681 Apr  8  2024 xattr.conf
drwxr-xr-x   4 root root       4096 May 18 12:57 xdg
drwxr-xr-x   2 root root       4096 May 18 12:59 xml
-rw-r--r--   1 root root        460 Jan 20  2023 zsh_command_not_found
root@ubuntu:/etc$ 

    Перейди у каталог /home і покажи список користувачів;

root@ubuntu:/etc$ cd ..
root@ubuntu:/$ cd /home
root@ubuntu:/home$ ls -la
total 12
drwxr-xr-x  3 root   root   4096 Jun 17 06:25 .
drwxr-xr-x 22 root   root   4096 Jun 20 08:53 ..
drwxr-x---  3 ubuntu ubuntu 4096 Jun 17 06:25 ubuntu
root@ubuntu:/home$ 

Завдання 2. Файли, каталоги та посилання (2 бали)

    Створи новий каталог у домашньому каталозі

root@ubuntu:/home$ mkdir ~/lab2
root@ubuntu:/home$ cd ~
root@ubuntu:~$ ls
filesystem  lab2
root@ubuntu:~$ cd lab2
root@ubuntu:~/lab2$ 

    Створи всередині файл

root@ubuntu:~/lab2$ touch file.txt
root@ubuntu:~/lab2$ ls
file.txt
root@ubuntu:~/lab2$ 

    Скопіюй файл у нове ім’я

root@ubuntu:~/lab2$ cp file.txt file_copy.txt
root@ubuntu:~/lab2$ ls
file.txt  file_copy.txt
root@ubuntu:~/lab2$ 

    Перейменуй копію

root@ubuntu:~/lab2$ mv file_copy.txt file_renamed.txt
root@ubuntu:~/lab2$ ls
file.txt  file_renamed.txt
root@ubuntu:~/lab2$ 

    Створи жорстке посилання

root@ubuntu:~/lab2$ ln ~/lab2/file.txt ~/lab2/hardlink.txt
root@ubuntu:~/lab2$ ls
file.txt  file_renamed.txt  hardlink.txt
root@ubuntu:~/lab2$ 

    Створи символічне посилання

root@ubuntu:~/lab2$ ln -s ~/lab2/file.txt ~/lab2/symlink.txt
root@ubuntu:~/lab2$ ls
file.txt  file_renamed.txt  hardlink.txt  symlink.txt
root@ubuntu:~/lab2$ 

    Знайди файл по імені
root@ubuntu:~/lab2$ find ~ -name "file.txt"
/root/lab2/file.txt
root@ubuntu:~/lab2$ 

Завдання 3. Права доступу (1 бал)

    Переглянь права файлу, який ти створив

root@ubuntu:~/lab2$ ls -l file.txt
-rw-r--r-- 2 root root 0 Jul  1 14:16 file.txt
root@ubuntu:~/lab2$ 

    Надай файлу права тільки на читання

root@ubuntu:~/lab2$ chmod 444 file.txt
root@ubuntu:~/lab2$ ls -l file.txt
-r--r--r-- 2 root root 0 Jul  1 14:16 file.txt
root@ubuntu:~/lab2$ 

    Надай власнику право на запис

root@ubuntu:~/lab2$ chmod u+w file.txt
root@ubuntu:~/lab2$ ls -l file.txt
-rw-r--r-- 2 root root 0 Jul  1 14:16 file.txt
root@ubuntu:~/lab2$ 

    Переглянь значення umask

root@ubuntu:~/lab2$ umask
0022
root@ubuntu:~/lab2$ 

    Встанови нове значення, наприклад 022

root@ubuntu:~/lab2$ umask 022

Завдання 4. Користувачі (1 бал)

    Створи нового користувача

root@ubuntu:~/lab2$ sudo useradd -m -s /bin/bash student

    Додай його до sudo-групи

root@ubuntu:~/lab2$ sudo usermod -aG sudo student 

    Перевір, що користувач існує

root@ubuntu:~/lab2$ grep student /etc/passwd
student:x:1001:1001::/home/student:/bin/bash
root@ubuntu:~/lab2$ 
