Домашнє завдання №3: Процеси та ресурси
Студент: Кучерук Євгеній Романович

Завдання 1. Огляд активних процесів (1 бал)

    Виведи список усіх процесів у системі за допомогою ps.

root@ubuntu:~$ ps aux
USER         PID %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND
root           1  0.1  0.6  22060 13296 ?        Ss   10:35   0:02 /sbin/init
root           2  0.0  0.0      0     0 ?        S    10:35   0:00 [kthreadd]
root           3  0.0  0.0      0     0 ?        S    10:35   0:00 [pool_workqueue_release]
root           4  0.0  0.0      0     0 ?        I<   10:35   0:00 [kworker/R-rcu_g]
root           5  0.0  0.0      0     0 ?        I<   10:35   0:00 [kworker/R-rcu_p]
root           6  0.0  0.0      0     0 ?        I<   10:35   0:00 [kworker/R-slub_]
root           7  0.0  0.0      0     0 ?        I<   10:35   0:00 [kworker/R-netns]
root          10  0.0  0.0      0     0 ?        I<   10:35   0:00 [kworker/0:0H-kblockd]
root          12  0.0  0.0      0     0 ?        I<   10:35   0:00 [kworker/R-mm_pe]

    Запусти інтерактивний монітор top (або htop, якщо він встановлений) та знайди процес, який споживає найбільше пам'яті (RAM).
root@ubuntu:~$ top -o %MEM

top - 10:57:13 up 21 min,  0 user,  load average: 0.07, 0.02, 0.00
Tasks: 123 total,   1 running, 122 sleeping,   0 stopped,   0 zombie
%Cpu(s):  0.0 us,  0.0 sy,  0.0 ni,100.0 id,  0.0 wa,  0.0 hi,  0.0 si,  0.0 st 
MiB Mem :   1903.2 total,    874.4 free,    415.2 used,    781.3 buff/cache     
MiB Swap:   1024.0 total,   1024.0 free,      0.0 used.   1488.0 avail Mem 

    PID USER      PR  NI    VIRT    RES    SHR S  %CPU  %MEM     TIME+ COMMAND                                            
   1247 root      39  19   11.2g  96032  43056 S   0.0   4.9   0:02.25 node                                               
    901 root      20   0 1835000  76856  55776 S   0.0   3.9   0:00.24 dockerd                                            
   1277 root      39  19 1177912  53908  40228 S   0.0   2.8   0:01.46 node                                               
    615 root      20   0 1719016  47120  33648 S   0.0   2.4   0:01.13 containerd                                         
    350 root      rt   0  288952  27292   8760 S   0.0   1.4   0:00.09 multipathd                                         
    666 root      20   0  110016  23056  13596 S   0.0   1.2   0:00.14 unattended-upgr                                    
    601 root      20   0  468832  13528  11416 S   0.0   0.7   0:00.15 udisksd                                            
      1 root      20   0   22060  13296   9528 S   0.0   0.7   0:02.37 systemd                     

    Знайди PID процесу вашої поточної оболонки (bash/zsh).

root@ubuntu:~$ echo $$
1683
root@ubuntu:~$ 


Завдання 2. Робота у фоні та керування процесами (1 бали)

    Запусти довгу команду (наприклад, sleep 1000) у фоновому режимі.

root@ubuntu:~$ sleep 1000 &
[1] 1692
root@ubuntu:~$ 

    Перевір список фонових завдань.

root@ubuntu:~$ jobs
[1]+  Running                 sleep 1000 &
root@ubuntu:~$ 

    Поверни цей процес із фону на передній план.

root@ubuntu:~$ fg %1
sleep 1000
^Z
[1]+  Stopped                 sleep 1000
root@ubuntu:~$ 

    Зупини процес та «примусово» заверши його за допомогою kill.

root@ubuntu:~$ kill -9 %1

[1]+  Stopped                 sleep 1000
root@ubuntu:~$ 

    Запусти будь-яку команду за допомогою nohup, щоб вона продовжувала працювати після закриття терміналу.

root@ubuntu:~$ nohup sleep 2000 &
[2] 1697
[1]   Killed                  sleep 1000
root@ubuntu:~$ nohup: ignoring input and appending output to 'nohup.out'


Завдання 3. Пріоритети та обмеження (2 бал)

    Запусти нову команду з підвищеним значенням nice (нижчим пріоритетом).

root@ubuntu:~$ nice -n 10 sleep 500 &
[3] 1701
root@ubuntu:~$ 

    Зміни пріоритет вже запущеного процесу.
    
root@ubuntu:~$ renice -n 15 -p 1701 
1701 (process ID) old priority 10, new priority 15
root@ubuntu:~$ 

    Переглянь поточні обмеження ресурсів вашого користувача за допомогою ulimit.

root@ubuntu:~$ ulimit -a
real-time non-blocking time  (microseconds, -R) unlimited
core file size              (blocks, -c) 0
data seg size               (kbytes, -d) unlimited
scheduling priority                 (-e) 0
file size                   (blocks, -f) unlimited
pending signals                     (-i) 7459
max locked memory           (kbytes, -l) 8192
max memory size             (kbytes, -m) unlimited
open files                          (-n) 1024
pipe size                (512 bytes, -p) 8
POSIX message queues         (bytes, -q) 819200
real-time priority                  (-r) 0
stack size                  (kbytes, -s) 8192
cpu time                   (seconds, -t) unlimited
max user processes                  (-u) 7459
virtual memory              (kbytes, -v) unlimited
file locks                          (-x) unlimited
[3]+  Done                    nice -n 10 sleep 500
root@ubuntu:~$ 


Завдання 4. Моніторинг ресурсів (1 бал)
    Виведи інформацію про використання дискового простору (вільне/зайняте місце).

root@ubuntu:~$ df -h
Filesystem      Size  Used Avail Use% Mounted on
tmpfs           191M  996K  190M   1% /run
/dev/vda1        19G  5.4G   14G  29% /
tmpfs           952M   84K  952M   1% /dev/shm
tmpfs           5.0M     0  5.0M   0% /run/lock
/dev/vda16      881M  117M  703M  15% /boot
/dev/vda15      105M  6.2M   99M   6% /boot/efi
root@ubuntu:~$ 

    Покажи обсяг вільної та використаної оперативної пам'яті в системі у зручному для читання форматі (Мб/Гб).
    
root@ubuntu:~$ free -h
               total        used        free      shared  buff/cache   available
Mem:           1.9Gi       457Mi       803Mi       1.1Mi       810Mi       1.4Gi
Swap:          1.0Gi          0B       1.0Gi
root@ubuntu:~$ 