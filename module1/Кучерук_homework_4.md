Домашнє завдання №4. Пакети, сервіси та журнали
Студент: Кучерук Євгеній Романович

Завдання 1. Менеджери пакетів (2 бали)

    Онови список пакетів у вашій системі.

root@ubuntu:~$ apt update
Hit:1 http://security.ubuntu.com/ubuntu noble-security InRelease
Hit:2 http://archive.ubuntu.com/ubuntu noble InRelease
Get:3 http://archive.ubuntu.com/ubuntu noble-updates InRelease [126 kB]
Hit:4 http://archive.ubuntu.com/ubuntu noble-backports InRelease
Get:5 http://archive.ubuntu.com/ubuntu noble-updates/main amd64 Packages [1074 kB]
Get:6 http://archive.ubuntu.com/ubuntu noble-updates/main Translation-en [266 kB]
Fetched 1467 kB in 1s (1131 kB/s)                              
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
21 packages can be upgraded. Run 'apt list --upgradable' to see them.
root@ubuntu:~$ 

    Встанови утиліту tree (або htop, якщо її немає).

root@ubuntu:~$ apt install -y tree
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
The following package was automatically installed and is no longer required:
  squashfs-tools
Use 'apt autoremove' to remove it.
The following NEW packages will be installed:
  tree
0 upgraded, 1 newly installed, 0 to remove and 21 not upgraded.
Need to get 47.4 kB of archives.
After this operation, 111 kB of additional disk space will be used.
Get:1 http://archive.ubuntu.com/ubuntu noble-updates/universe amd64 tree amd64 2.1.1-2ubuntu3.24.04.2 [47.4 kB]
Fetched 47.4 kB in 0s (581 kB/s)
Selecting previously unselected package tree.
(Reading database ... 114086 files and directories currently installed.)
Preparing to unpack .../tree_2.1.1-2ubuntu3.24.04.2_amd64.deb ...
Unpacking tree (2.1.1-2ubuntu3.24.04.2) ...
Setting up tree (2.1.1-2ubuntu3.24.04.2) ...
Processing triggers for man-db (2.12.0-4build2) ...
Scanning processes...                                                                                                     
Scanning linux images...                                                                                                  

Running kernel seems to be up-to-date.

No services need to be restarted.

No containers need to be restarted.

No user sessions are running outdated binaries.

No VM guests are running outdated hypervisor (qemu) binaries on this host.
root@ubuntu:~$ 


    Перевір, чи встановлено пакет, і виведіть його версію.

root@ubuntu:~$ tree --version
tree v2.1.1 (c) 1996 - 2023 by Steve Baker, Thomas Moore, Francesc Rocher, Florian Sesser, Kyosuke Tokoro
root@ubuntu:~$ 

    Видали встановлений пакет.

root@ubuntu:~$ apt remove -y tree
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
The following package was automatically installed and is no longer required:
  squashfs-tools
Use 'apt autoremove' to remove it.
The following packages will be REMOVED:
  tree
0 upgraded, 0 newly installed, 1 to remove and 21 not upgraded.
After this operation, 111 kB disk space will be freed.
(Reading database ... 114093 files and directories currently installed.)
Removing tree (2.1.1-2ubuntu3.24.04.2) ...
Processing triggers for man-db (2.12.0-4build2) ...
root@ubuntu:~$ 


Завдання 2. Керування сервісами через systemctl (2 бали)

    Перевір статус сервісу ssh (або cron, або nginx, якщо є).

root@ubuntu:~$ systemctl status cron
● cron.service - Regular background program processing daemon
     Loaded: loaded (/usr/lib/systemd/system/cron.service; enabled; preset: enabled)
     Active: active (running) since Thu 2026-07-02 10:43:44 UTC; 1h 6min ago
       Docs: man:cron(8)
   Main PID: 737 (cron)
      Tasks: 8 (limit: 2237)
     Memory: 6.6M (peak: 10.2M)
        CPU: 255ms
     CGroup: /system.slice/cron.service
             ├─ 737 /usr/sbin/cron -f -P
             ├─ 849 "dhcpcd: enp1s0 [ip4] [ip6]"
             ├─ 850 "dhcpcd: [privileged proxy] enp1s0 [ip4] [ip6]"
             ├─ 851 "dhcpcd: [network proxy] enp1s0 [ip4] [ip6]"
             ├─ 852 "dhcpcd: [control proxy] enp1s0 [ip4] [ip6]"
             ├─1122 "dhcpcd: [BPF ARP] enp1s0 172.30.1.2"
             ├─1123 "dhcpcd: [DHCP6 proxy] fe80::fc85:3a54:a334:4301"
             └─1157 "dhcpcd: [BOOTP proxy] 172.30.1.2"

Jul 02 11:25:01 ubuntu CRON[1786]: pam_unix(cron:session): session opened for user root(uid=0) by root(uid=0)
Jul 02 11:25:01 ubuntu CRON[1787]: (root) CMD (command -v debian-sa1 > /dev/null && debian-sa1 1 1)
Jul 02 11:25:01 ubuntu CRON[1786]: pam_unix(cron:session): session closed for user root
Jul 02 11:35:01 ubuntu CRON[1796]: pam_unix(cron:session): session opened for user root(uid=0) by root(uid=0)
Jul 02 11:35:01 ubuntu CRON[1797]: (root) CMD (command -v debian-sa1 > /dev/null && debian-sa1 1 1)
Jul 02 11:35:01 ubuntu CRON[1796]: pam_unix(cron:session): session closed for user root
Jul 02 11:39:01 ubuntu CRON[1800]: pam_unix(cron:session): session opened for user root(uid=0) by root(uid=0)
Jul 02 11:39:01 ubuntu CRON[1800]: pam_unix(cron:session): session closed for user root
Jul 02 11:45:01 ubuntu CRON[1837]: pam_unix(cron:session): session opened for user root(uid=0) by root(uid=0)
Jul 02 11:45:01 ubuntu CRON[1837]: pam_unix(cron:session): session closed for user root
root@ubuntu:~$ 

    Зупини сервіс та переконайтеся, що він не активний.

root@ubuntu:~$ systemctl stop cron
root@ubuntu:~$ systemctl status cron
○ cron.service - Regular background program processing daemon
     Loaded: loaded (/usr/lib/systemd/system/cron.service; enabled; preset: enabled)
     Active: inactive (dead) since Thu 2026-07-02 11:51:13 UTC; 4s ago
   Duration: 1h 7min 29.405s
       Docs: man:cron(8)
    Process: 737 ExecStart=/usr/sbin/cron -f -P $EXTRA_OPTS (code=killed, signal=TERM)
   Main PID: 737 (code=killed, signal=TERM)
      Tasks: 7 (limit: 2237)
     Memory: 6.2M (peak: 10.2M)
        CPU: 255ms
     CGroup: /system.slice/cron.service
             ├─ 849 "dhcpcd: enp1s0 [ip4] [ip6]"
             ├─ 850 "dhcpcd: [privileged proxy] enp1s0 [ip4] [ip6]"
             ├─ 851 "dhcpcd: [network proxy] enp1s0 [ip4] [ip6]"
             ├─ 852 "dhcpcd: [control proxy] enp1s0 [ip4] [ip6]"
             ├─1122 "dhcpcd: [BPF ARP] enp1s0 172.30.1.2"
             ├─1123 "dhcpcd: [DHCP6 proxy] fe80::fc85:3a54:a334:4301"
             └─1157 "dhcpcd: [BOOTP proxy] 172.30.1.2"

Jul 02 11:51:13 ubuntu systemd[1]: Stopping cron.service - Regular background program processing daemon...
Jul 02 11:51:13 ubuntu systemd[1]: cron.service: Deactivated successfully.
Jul 02 11:51:13 ubuntu systemd[1]: cron.service: Unit process 849 (dhcpcd) remains running after unit stopped.
Jul 02 11:51:13 ubuntu systemd[1]: cron.service: Unit process 850 (dhcpcd) remains running after unit stopped.
Jul 02 11:51:13 ubuntu systemd[1]: cron.service: Unit process 851 (dhcpcd) remains running after unit stopped.
Jul 02 11:51:13 ubuntu systemd[1]: cron.service: Unit process 852 (dhcpcd) remains running after unit stopped.
Jul 02 11:51:13 ubuntu systemd[1]: cron.service: Unit process 1122 (dhcpcd) remains running after unit stopped.
Jul 02 11:51:13 ubuntu systemd[1]: cron.service: Unit process 1123 (dhcpcd) remains running after unit stopped.
Jul 02 11:51:13 ubuntu systemd[1]: cron.service: Unit process 1157 (dhcpcd) remains running after unit stopped.
Jul 02 11:51:13 ubuntu systemd[1]: Stopped cron.service - Regular background program processing daemon.
root@ubuntu:~$ 

    Запусти сервіс знову.

root@ubuntu:~$ systemctl start cron
root@ubuntu:~$ systemctl status cron
● cron.service - Regular background program processing daemon
     Loaded: loaded (/usr/lib/systemd/system/cron.service; enabled; preset: enabled)
     Active: active (running) since Thu 2026-07-02 11:51:42 UTC; 7s ago
       Docs: man:cron(8)
   Main PID: 2356 (cron)
      Tasks: 8 (limit: 2237)
     Memory: 6.6M (peak: 10.2M)
        CPU: 5ms
     CGroup: /system.slice/cron.service
             ├─ 849 "dhcpcd: enp1s0 [ip4] [ip6]"
             ├─ 850 "dhcpcd: [privileged proxy] enp1s0 [ip4] [ip6]"
             ├─ 851 "dhcpcd: [network proxy] enp1s0 [ip4] [ip6]"
             ├─ 852 "dhcpcd: [control proxy] enp1s0 [ip4] [ip6]"
             ├─1122 "dhcpcd: [BPF ARP] enp1s0 172.30.1.2"
             ├─1123 "dhcpcd: [DHCP6 proxy] fe80::fc85:3a54:a334:4301"
             ├─1157 "dhcpcd: [BOOTP proxy] 172.30.1.2"
             └─2356 /usr/sbin/cron -f -P

Jul 02 11:51:42 ubuntu systemd[1]: Started cron.service - Regular background program processing daemon.
Jul 02 11:51:42 ubuntu (cron)[2356]: cron.service: Referenced but unset environment variable evaluates to an empty string>
Jul 02 11:51:42 ubuntu cron[2356]: (CRON) INFO (pidfile fd = 3)
Jul 02 11:51:42 ubuntu cron[2356]: (CRON) INFO (Skipping @reboot jobs -- not system startup)
lines 1-22/22 (END)

    Додай сервіс в автозавантаження (щоб він запускався разом із системою).

root@ubuntu:~$ systemctl enable cron
Synchronizing state of cron.service with SysV service script with /usr/lib/systemd/systemd-sysv-install.
Executing: /usr/lib/systemd/systemd-sysv-install enable cron
root@ubuntu:~$ 


Завдання 3. Робота з логами (2 бали)

    Перейди в директорію /var/log і виведіть останні 10 рядків файлу syslog (або messages).

root@ubuntu:~$ cd /var/log
root@ubuntu:/var/log$ tail -n 10 syslog
2026-07-02T11:51:42.523607+00:00 ubuntu cron[2356]: (CRON) INFO (Skipping @reboot jobs -- not system startup)
2026-07-02T11:52:23.982316+00:00 ubuntu systemd[1]: Reloading requested from client PID 2364 ('systemctl') (unit ssh.service)...
2026-07-02T11:52:23.983698+00:00 ubuntu systemd[1]: Reloading...
2026-07-02T11:52:24.290548+00:00 ubuntu systemd[1]: Reloading finished in 307 ms.
2026-07-02T11:52:24.341464+00:00 ubuntu systemd[1]: Reloading requested from client PID 2407 ('systemctl') (unit ssh.service)...
2026-07-02T11:52:24.341550+00:00 ubuntu systemd[1]: Reloading...
2026-07-02T11:52:24.660596+00:00 ubuntu systemd[1]: Reloading finished in 318 ms.
2026-07-02T11:52:24.705037+00:00 ubuntu systemd[1]: Reloading requested from client PID 2360 ('systemctl') (unit ssh.service)...
2026-07-02T11:52:24.705506+00:00 ubuntu systemd[1]: Reloading...
2026-07-02T11:52:25.055439+00:00 ubuntu systemd[1]: Reloading finished in 349 ms.
root@ubuntu:/var/log$ 

    Використовуй journalctl, щоб переглянути тільки помилки (рівень priority "err") у вашій системі.

root@ubuntu:/var/log$ journalctl -p err --no-pager -n 20
Jun 17 06:25:54 vm2 systemd[1]: Failed to start cloud-final.service - Cloud-init: Final Stage.
-- Boot 3ebec48c9cdc4214ae35cb64cac099bc --
Jun 20 08:51:38 vm2 systemd[1]: apt-daily.timer: Unit to trigger vanished.
Jun 20 08:51:38 vm2 systemd[1]: apt-daily-upgrade.timer: Unit to trigger vanished.
Jun 20 08:51:38 vm2 sudo[1391]:     root : unable to resolve host vm2: Name or service not known
Jun 20 08:51:38 vm2 sudo[1393]:     root : unable to resolve host vm2: Name or service not known
-- Boot 420ac0a9612b4b9fa9c0dfc3246d8ef9 --
Jul 02 10:43:43 ubuntu systemd[1]: Failed to start rsyslog.service - System Logging Service.
Jul 02 10:43:45 ubuntu dhcpcd[837]: dhcpcd is not running
root@ubuntu:/var/log$ 

    Знайди у журналах запис про запуск або зупинку сервісу, з яким ви працювали у Завданні 2.
root@ubuntu:/var/log$ journalctl -p err --no-pager -n 20
Jun 17 06:25:54 vm2 systemd[1]: Failed to start cloud-final.service - Cloud-init: Final Stage.
-- Boot 3ebec48c9cdc4214ae35cb64cac099bc --
Jun 20 08:51:38 vm2 systemd[1]: apt-daily.timer: Unit to trigger vanished.
Jun 20 08:51:38 vm2 systemd[1]: apt-daily-upgrade.timer: Unit to trigger vanished.
Jun 20 08:51:38 vm2 sudo[1391]:     root : unable to resolve host vm2: Name or service not known
Jun 20 08:51:38 vm2 sudo[1393]:     root : unable to resolve host vm2: Name or service not known
-- Boot 420ac0a9612b4b9fa9c0dfc3246d8ef9 --
Jul 02 10:43:43 ubuntu systemd[1]: Failed to start rsyslog.service - System Logging Service.
Jul 02 10:43:45 ubuntu dhcpcd[837]: dhcpcd is not running
root@ubuntu:/var/log$ journalctl -u cron --no-pager -n 20
Jul 02 11:51:42 ubuntu systemd[1]: cron.service: This usually indicates unclean termination of a previous run, or service implementation deficiencies.
Jul 02 11:51:42 ubuntu systemd[1]: cron.service: Found left-over process 850 (dhcpcd) in control group while starting unit. Ignoring.
Jul 02 11:51:42 ubuntu systemd[1]: cron.service: This usually indicates unclean termination of a previous run, or service implementation deficiencies.
Jul 02 11:51:42 ubuntu systemd[1]: cron.service: Found left-over process 851 (dhcpcd) in control group while starting unit. Ignoring.
Jul 02 11:51:42 ubuntu systemd[1]: cron.service: This usually indicates unclean termination of a previous run, or service implementation deficiencies.
Jul 02 11:51:42 ubuntu systemd[1]: cron.service: Found left-over process 852 (dhcpcd) in control group while starting unit. Ignoring.
Jul 02 11:51:42 ubuntu systemd[1]: cron.service: This usually indicates unclean termination of a previous run, or service implementation deficiencies.
Jul 02 11:51:42 ubuntu systemd[1]: cron.service: Found left-over process 1122 (dhcpcd) in control group while starting unit. Ignoring.
Jul 02 11:51:42 ubuntu systemd[1]: cron.service: This usually indicates unclean termination of a previous run, or service implementation deficiencies.
Jul 02 11:51:42 ubuntu systemd[1]: cron.service: Found left-over process 1123 (dhcpcd) in control group while starting unit. Ignoring.
Jul 02 11:51:42 ubuntu systemd[1]: cron.service: This usually indicates unclean termination of a previous run, or service implementation deficiencies.
Jul 02 11:51:42 ubuntu systemd[1]: cron.service: Found left-over process 1157 (dhcpcd) in control group while starting unit. Ignoring.
Jul 02 11:51:42 ubuntu systemd[1]: cron.service: This usually indicates unclean termination of a previous run, or service implementation deficiencies.
Jul 02 11:51:42 ubuntu systemd[1]: Started cron.service - Regular background program processing daemon.
Jul 02 11:51:42 ubuntu (cron)[2356]: cron.service: Referenced but unset environment variable evaluates to an empty string: EXTRA_OPTS
Jul 02 11:51:42 ubuntu cron[2356]: (CRON) INFO (pidfile fd = 3)
Jul 02 11:51:42 ubuntu cron[2356]: (CRON) INFO (Skipping @reboot jobs -- not system startup)
Jul 02 11:55:01 ubuntu CRON[2493]: pam_unix(cron:session): session opened for user root(uid=0) by root(uid=0)
Jul 02 11:55:01 ubuntu CRON[2494]: (root) CMD (command -v debian-sa1 > /dev/null && debian-sa1 1 1)
Jul 02 11:55:01 ubuntu CRON[2493]: pam_unix(cron:session): session closed for user root
root@ubuntu:/var/log$ 


Завдання 4. Створення власного сервісу (4 бали)

    Створи простий bash-скрипт у своєму домашньому каталозі, який щосекунди записує поточну дату в текстовий файл.

root@ubuntu:~$ cat << 'EOF' > /root/date_logger.sh
#!/bin/bash
while true; do
    date >> /root/date_log.txt
    sleep 1
done
EOF
root@ubuntu:~$ chmod +x /root/date_logger.sh

    Створи файл конфігурації сервісу /etc/systemd/system/myscript.service.

root@ubuntu:~$ cat << 'EOF' > /etc/systemd/system/myscript.service
[Unit]
Description=My Custom Date Logger Service
After=network.target

[Service]
ExecStart=/bin/bash /root/date_logger.sh
Restart=always
User=root

[Install]
WantedBy=multi-user.target
EOF
root@ubuntu:~$ 

    Налаштуй його так, щоб він запускав ваш скрипт.

root@ubuntu:~/filesystem/etc/systemd/system$ systemctl daemon-reload
root@ubuntu:~/filesystem/etc/systemd/system$ systemctl start myscript

    Запусти сервіс, перевірте його статус та переконайтеся, що дані записуються у файл.
root@ubuntu:~/filesystem/etc/systemd/system$ systemctl status myscript
● myscript.service - My Custom Date Logger Service
     Loaded: loaded (/etc/systemd/system/myscript.service; disabled; preset: enabled)
     Active: active (running) since Thu 2026-07-02 12:09:13 UTC; 16s ago
   Main PID: 1953 (bash)
      Tasks: 2 (limit: 2237)
     Memory: 584.0K (peak: 1.1M)
        CPU: 48ms
     CGroup: /system.slice/myscript.service
             ├─1953 /bin/bash /root/date_logger.sh
             └─1987 sleep 1

Jul 02 12:09:13 ubuntu systemd[1]: Started myscript.service - My Custom Date Logger Service.
root@ubuntu:~/filesystem/etc/systemd/system$ 

root@ubuntu:~/filesystem/etc/systemd/system$ tail -n 5 /root/date_log.txt
Thu Jul  2 12:10:01 UTC 2026
Thu Jul  2 12:10:02 UTC 2026
Thu Jul  2 12:10:03 UTC 2026
Thu Jul  2 12:10:04 UTC 2026
Thu Jul  2 12:10:05 UTC 2026
root@ubuntu:~/filesystem/etc/systemd/system$ 