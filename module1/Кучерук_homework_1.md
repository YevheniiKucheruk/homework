Домашнє завдання 1: Основи Linux і робота в терміналі
Студент: Кучерук Євгеній Романович

Завдання 1: Базові команди

1) Покажи вміст домашнього каталогу

ls ~
zhenya@Air-Evgenij ~ % ls
Applications			Templates
Cisco Packet Tracer 8.0.1	VirtualBox VMs
Desktop				Zomboid
Documents			cache
Downloads			def g(x, y):.py
Library				node_modules
Movies				package-lock.json
Music				package.json
My Games			shedule
Parallels			ssh_key
Pictures			ssh_key.pub
Projects			ts-fundamentals-hw-2
Public				Ігри
PycharmProjects

zhenya@Air-Evgenij ~ % ls -la
total 344
drwxr-x---+  72 zhenya  staff   2304 28 чер 08:31 .
drwxr-xr-x    7 root    admin    224 17 чер  2024 ..
-r--------    1 zhenya  staff      8 11 кві  2023 .CFUserTextEncoding
-rw-r--r--@   1 zhenya  staff  28676 25 чер 23:34 .DS_Store
drwxr-xr-x    7 zhenya  staff    224  6 лис  2023 .IdentityService
drwx------+   2 zhenya  staff     64 25 чер 23:34 .Trash
drwxr-xr-x    3 zhenya  staff     96 19 сер  2022 .android
drwxr-xr-x   11 zhenya  staff    352  5 вер  2024 .anydesk
drwxr-xr-x    4 zhenya  staff    128 20 тра  2025 .aws
-rw-------    1 zhenya  staff   1821 14 кві  2025 .bash_history
-rw-r--r--@   1 zhenya  staff    303 28 січ  2025 .bash_profile
drwxr-xr-x@   3 zhenya  staff     96 29 гру  2024 .cache
drwx------    3 zhenya  staff     96 19 сер  2025 .cups
drwxr-xr-x   19 zhenya  staff    608  5 вер  2024 .dotnet
-rw-r--r--    1 zhenya  staff    611 26 січ 23:56 .gitconfig
-rw-r--r--@   1 zhenya  staff     95 22 бер  2024 .gitflow_export
-rw-r--r--@   1 zhenya  staff     13 14 лют  2024 .gitignore_global
-rw-r--r--@   1 zhenya  staff     27 14 лют  2024 .hgignore_global
drwxr-xr-x    4 zhenya  staff    128 22 лис  2022 .idlerc
-rw-------    1 zhenya  staff     20  5 чер 18:03 .lesshst
drwxrwxrwx    4 zhenya  staff    128  5 вер  2024 .local
drwxr-xr-x@   4 zhenya  staff    128 30 січ  2025 .m2
drwxr-xr-x    4 zhenya  staff    128 29 січ  2025 .matplotlib
drwxr-xr-x    3 zhenya  staff     96 18 сер  2022 .mono
-rw-------    1 zhenya  staff     92  6 січ 14:38 .node_repl_history
drwxr-xr-x    7 zhenya  staff    224  5 вер  2024 .npm
drwxr-xr-x    5 zhenya  staff    160  5 вер  2024 .nuget
drwxr-xr-x    8 zhenya  staff    256  5 вер  2024 .nvm
drwxr-xr-x    3 zhenya  staff     96  6 вер  2023 .oracle_jre_usage
-rw-r--r--@   1 zhenya  staff    246 14 гру  2023 .packettracer
drwx------@  56 zhenya  staff   1792 25 чер 17:44 .pgadmin
-rw-------@   1 zhenya  staff    121 20 бер 18:09 .psql_history
drwx------    6 zhenya  staff    192 28 січ 11:35 .ssh
-rw-r--r--@   1 zhenya  staff      0 22 бер  2024 .stCommitMsg
drwxr-xr-x   15 zhenya  staff    480 11 гру  2022 .start_app_logs
drwxr-xr-x    4 zhenya  staff    128 31 лип  2022 .swiftpm
drwxr-xr-x    5 zhenya  staff    160  5 вер  2024 .templateengine
-rw-------    1 zhenya  staff  16324  5 чер 18:04 .viminfo
drwxr-xr-x    6 zhenya  staff    192  7 вер  2023 .vscode
-rw-r--r--    1 zhenya  staff    375 16 жов  2024 .zprofile
-rw-r--r--    1 zhenya  staff    209  7 вер  2023 .zprofile.pysave
-rw-------    1 zhenya  staff  22347 28 чер 08:31 .zsh_history
drwx------    6 zhenya  staff    192 28 чер 08:31 .zsh_sessions
-rw-r--r--    1 zhenya  staff     57 18 жов  2023 .zshrc
-rw-------    1 zhenya  staff    101 20 вер  2023 .zshrc.save
drwx------@   9 zhenya  staff    288  4 кві 08:59 Applications
drwxr-xr-x@  10 zhenya  staff    320  5 вер  2024 Cisco Packet Tracer 8.0.1
drwx------@ 157 zhenya  staff   5024 25 чер 23:56 Desktop
drwx------+  15 zhenya  staff    480 26 січ 18:58 Documents
drwx------@ 693 zhenya  staff  22176 26 чер 18:49 Downloads
drwx------@ 103 zhenya  staff   3296 17 кві 22:21 Library
drwx------   10 zhenya  staff    320  5 вер  2024 Movies
drwx------+   5 zhenya  staff    160  5 вер  2024 Music
drwxr-xr-x    5 zhenya  staff    160  5 вер  2024 My Games
drwx------    2 zhenya  staff     64 26 січ 22:41 Parallels
drwx------+   7 zhenya  staff    224 24 лис  2022 Pictures
drwxr-xr-x    8 zhenya  staff    256  5 вер  2024 Projects
drwxr-xr-x+   5 zhenya  staff    160  4 гру  2022 Public
drwxr-xr-x    3 zhenya  staff     96 17 жов  2024 PycharmProjects
drwxr-xr-x    2 zhenya  staff     64 26 лис  2024 Templates
drwxr-xr-x    3 zhenya  staff     96 19 вер  2023 VirtualBox VMs
drwxr-xr-x   18 zhenya  staff    576  8 січ 08:19 Zomboid
drwxr-xr-x    6 zhenya  staff    192  4 гру  2022 cache
-rw-r--r--    1 zhenya  staff   2448 24 тра  2023 def g(x, y):.py
drwxr-xr-x   13 zhenya  staff    416 29 січ 22:59 node_modules
-rw-r--r--    1 zhenya  staff   2754 10 бер  2024 package-lock.json
-rw-r--r--    1 zhenya  staff     65 10 бер  2024 package.json
-rw-r--r--@   1 zhenya  staff  18617 18 тра  2024 shedule
-rw-------@   1 zhenya  staff    432 16 жов  2024 ssh_key
-rw-r--r--    1 zhenya  staff    114 16 жов  2024 ssh_key.pub
drwxr-xr-x   12 zhenya  staff    384 29 січ 23:04 ts-fundamentals-hw-2
drwxr-xr-x    3 zhenya  staff     96 26 лис  2024 Ігри


2) Перейди у каталог Downloads і покажи його вміст

zhenya@Air-Evgenij ~ % cd Downloads
zhenya@Air-Evgenij Downloads % ls

безіменна папка
Мистецтво життєвого балансу.pdf
Скановано_20260119-1232 (1).pdf
Скановано_20260119-1232 (2).pdf
Скановано_20260119-1232 (3).pdf
Скановано_20260119-1232.pdf
підліткова програма 2026(1).pdf
Потенційні партнери для підтримки літнього служіння.xlsx
Військово-обліковий документ.pdf
відеозапис.mov

3) Створи порожній файл (без touch)
zhenya@Air-Evgenij HW % cd ../../..
zhenya@Air-Evgenij ~ % cd Desktop/University/HW
zhenya@Air-Evgenij HW % > homework.txt

^C
zhenya@Air-Evgenij HW % 

4) Переглянь вміст файлу
^C
zhenya@Air-Evgenij HW % cat homework.txt

zhenya@Air-Evgenij HW % 

5) Перейди у домашній каталог абсолютним шляхом
zhenya@Air-Evgenij ~ % cd /users/zhenya
zhenya@Air-Evgenij zhenya % ls
Applications			Templates
Cisco Packet Tracer 8.0.1	VirtualBox VMs
Desktop				Zomboid
Documents			cache
Downloads			def g(x, y):.py
Library				node_modules
Movies				package-lock.json
Music				package.json
My Games			shedule
Parallels			ssh_key
Pictures			ssh_key.pub
Projects			ts-fundamentals-hw-2
Public				Ігри
PycharmProjects
zhenya@Air-Evgenij zhenya % 

6) Перейди у домашній каталог відносним шляхом

zhenya@Air-Evgenij ~ % cd desktop/university/hw
zhenya@Air-Evgenij hw % cd ~
zhenya@Air-Evgenij ~ % ls


Applications			Templates
Cisco Packet Tracer 8.0.1	VirtualBox VMs
Desktop				Zomboid
Documents			cache
Downloads			def g(x, y):.py
Library				node_modules
Movies				package-lock.json
Music				package.json
My Games			shedule
Parallels			ssh_key
Pictures			ssh_key.pub
Projects			ts-fundamentals-hw-2
Public				Ігри
PycharmProjects


Завдання 2: Робота з документацією

zhenya@Air-Evgenij ~ % man ls

LS(1)                       General Commands Manual                      LS(1)

NAME
     ls – list directory contents

SYNOPSIS
     ls [-@ABCFGHILOPRSTUWabcdefghiklmnopqrstuvwxy1%,] [--color=when]
        [-D format] [file ...]

DESCRIPTION
     For each operand that names a file of a type other than directory, ls
     displays its name as well as any requested, associated information.  For
     each operand that names a file of type directory, ls displays the names
     of files contained within that directory, as well as any requested,
     associated information.

     If no operands are given, the contents of the current directory are
     displayed.  If more than one operand is given, non-directory operands are
     displayed first; directory and non-directory operands are sorted
     separately and in lexicographical order.

     The following options are available:

:

zhenya@Air-Evgenij ~ % help cd 
zsh: command not found: help

zhenya@Air-Evgenij ~ % man cat 

CAT(1)                      General Commands Manual                     CAT(1)

NAME
     cat – concatenate and print files

SYNOPSIS
     cat [-belnstuv] [file ...]

DESCRIPTION
     The cat utility reads files sequentially, writing them to the standard
     output.  The file operands are processed in command-line order.  If file
     is a single dash (‘-’) or absent, cat reads from the standard input.  If
     file is a UNIX domain socket, cat connects to it and then reads it until
     EOF.  This complements the UNIX domain binding capability available in
     inetd(8).

     The options are as follows:

     -b      Number the non-blank output lines, starting at 1.

     -e      Display non-printing characters (see the -v option), and display
             a dollar sign (‘$’) at the end of each line.

:

zhenya@Air-Evgenij ~ % man man 

MAN(1)                      General Commands Manual                     MAN(1)

NAME
     man, apropos, whatis – display online manual documentation pages

SYNOPSIS
     man [-adho] [-t | -w] [-M manpath] [-P pager] [-S mansect]
         [-m arch[:machine]] [-p [eprtv]] [mansect] page ...

     man -f [-d] [-M manpath] [-P pager] [-S mansect] keyword ...
     whatis [-d] [-s mansect] keyword ...

     man -k [-d] [-M manpath] [-P pager] [-S mansect] keyword ...
     apropos [-d] [-s mansect] keyword ...

DESCRIPTION
     The man utility finds and displays online manual documentation pages.  If
     mansect is provided, man restricts the search to the specific section of
     the manual.

     The sections of the manual are:
           1.   General Commands Manual
           2.   System Calls Manual


zhenya@Air-Evgenij ~ % cp --help  
cp: illegal option -- -
usage: cp [-R [-H | -L | -P]] [-fi | -n] [-aclpSsvXx] source_file target_file
       cp [-R [-H | -L | -P]] [-fi | -n] [-aclpSsvXx] source_file ... target_directory
zhenya@Air-Evgenij ~ % 

zhenya@Air-Evgenij ~ % mv --help
mv: illegal option -- -
usage: mv [-f | -i | -n] [-hv] source target
       mv [-f | -i | -n] [-v] source ... directory
zhenya@Air-Evgenij ~ % 

В системі macOS в терміналі не працюють прапорці --help чи -help. Замість цього треба використовувати man для перегляду документації.

Питання:
Який ключ ls показує приховані файли?
- a 

Який ключ у cat нумерує рядки?
-n

Чим відрізняються man і -help?

man - це утиліта, що надає детальний опис команди.

- help - це ключ, що надає короткий опис команди.

Завдання 3: Міні-сценарій (2 бали)
    zhenya@Air-Evgenij ~ % cd /tmp          
    zhenya@Air-Evgenij /tmp % > text_exmple1.txt

^C
    zhenya@Air-Evgenij /tmp % ls                
CrashUpload-OJm1z			zeb_def_ipc_54751
aws-toolkit-vscode			zeb_def_ipc_54828
com.apple.launchd.B1LmEjUdDn		zeb_def_ipc_54851
com.apple.launchd.JthVByvKGX		zeb_def_ipc_55000
dumps					zeb_def_ipc_55277
powerlog				zeb_def_ipc_55365
steam.pipe				zeb_def_ipc_55741
steam_chrome_shmem_uid501_spid87648	zeb_def_ipc_55866
text_exmple.txt				zeb_def_ipc_56037
text_exmple1.txt			zeb_def_ipc_56162
zeb_def_ipc_10019			zeb_def_ipc_56296
zeb_def_ipc_10131			zeb_def_ipc_5646
zeb_def_ipc_10223			zeb_def_ipc_56493
zeb_def_ipc_10240			zeb_def_ipc_56700
zeb_def_ipc_10452			zeb_def_ipc_57121
zeb_def_ipc_10565			zeb_def_ipc_57264
zeb_def_ipc_11163			zeb_def_ipc_57299
zeb_def_ipc_11194			zeb_def_ipc_57346
zeb_def_ipc_11546			zeb_def_ipc_57502
zeb_def_ipc_1160			zeb_def_ipc_57649
zeb_def_ipc_11665			zeb_def_ipc_57821
zeb_def_ipc_11818			zeb_def_ipc_57935
zeb_def_ipc_1203			zeb_def_ipc_58021
zeb_def_ipc_12170			zeb_def_ipc_58034
zeb_def_ipc_12225			zeb_def_ipc_58082
zeb_def_ipc_12341			zeb_def_ipc_58164
zeb_def_ipc_12344			zeb_def_ipc_58265
zeb_def_ipc_12528			zeb_def_ipc_58396
zeb_def_ipc_12672			zeb_def_ipc_58446
zeb_def_ipc_12727			zeb_def_ipc_58513
zeb_def_ipc_12869			zeb_def_ipc_58529
zeb_def_ipc_12922			zeb_def_ipc_58953
zeb_def_ipc_12932			zeb_def_ipc_59068
zeb_def_ipc_12938			zeb_def_ipc_59221
zeb_def_ipc_13000			zeb_def_ipc_59251
zeb_def_ipc_13118			zeb_def_ipc_59772
zeb_def_ipc_1345			zeb_def_ipc_59821
zeb_def_ipc_13547			zeb_def_ipc_59867
zeb_def_ipc_13649			zeb_def_ipc_60107
zeb_def_ipc_1393			zeb_def_ipc_60379
zeb_def_ipc_14161			zeb_def_ipc_60385
zeb_def_ipc_14233			zeb_def_ipc_60730
zeb_def_ipc_14541			zeb_def_ipc_60781
zeb_def_ipc_14590			zeb_def_ipc_60824
zeb_def_ipc_14741			zeb_def_ipc_60843
zeb_def_ipc_14955			zeb_def_ipc_6099
zeb_def_ipc_14960			zeb_def_ipc_61050
zeb_def_ipc_14967			zeb_def_ipc_61384
zeb_def_ipc_15102			zeb_def_ipc_61906
zeb_def_ipc_15238			zeb_def_ipc_61980
zeb_def_ipc_15626			zeb_def_ipc_62072
zeb_def_ipc_15740			zeb_def_ipc_62087
zeb_def_ipc_15904			zeb_def_ipc_62102
zeb_def_ipc_15908			zeb_def_ipc_6224
zeb_def_ipc_15935			zeb_def_ipc_62336
zeb_def_ipc_15948			zeb_def_ipc_62406
zeb_def_ipc_1600			zeb_def_ipc_62569
zeb_def_ipc_16013			zeb_def_ipc_6257
zeb_def_ipc_16064			zeb_def_ipc_62753
zeb_def_ipc_16174			zeb_def_ipc_62771
zeb_def_ipc_16374			zeb_def_ipc_62851
zeb_def_ipc_16379			zeb_def_ipc_62867
zeb_def_ipc_16435			zeb_def_ipc_62935
zeb_def_ipc_16531			zeb_def_ipc_63079
zeb_def_ipc_16567			zeb_def_ipc_63190
zeb_def_ipc_16571			zeb_def_ipc_63232
zeb_def_ipc_16857			zeb_def_ipc_63331
zeb_def_ipc_1686			zeb_def_ipc_63380
zeb_def_ipc_16880			zeb_def_ipc_63381
zeb_def_ipc_1709			zeb_def_ipc_63448
zeb_def_ipc_17093			zeb_def_ipc_63520
zeb_def_ipc_17145			zeb_def_ipc_63796
zeb_def_ipc_17557			zeb_def_ipc_63811
zeb_def_ipc_17558			zeb_def_ipc_64033
zeb_def_ipc_17643			zeb_def_ipc_64293
zeb_def_ipc_17669			zeb_def_ipc_64472
zeb_def_ipc_17787			zeb_def_ipc_64610
zeb_def_ipc_17797			zeb_def_ipc_64763
zeb_def_ipc_18085			zeb_def_ipc_64980
zeb_def_ipc_18893			zeb_def_ipc_6510
zeb_def_ipc_18994			zeb_def_ipc_65205
zeb_def_ipc_18995			zeb_def_ipc_6532
zeb_def_ipc_19007			zeb_def_ipc_65548
zeb_def_ipc_1903			zeb_def_ipc_65682
zeb_def_ipc_19049			zeb_def_ipc_65688
zeb_def_ipc_19109			zeb_def_ipc_65838
zeb_def_ipc_19268			zeb_def_ipc_65886
zeb_def_ipc_19363			zeb_def_ipc_65913
zeb_def_ipc_19599			zeb_def_ipc_661
zeb_def_ipc_19890			zeb_def_ipc_6619
zeb_def_ipc_19989			zeb_def_ipc_66222
zeb_def_ipc_20021			zeb_def_ipc_66410
zeb_def_ipc_20852			zeb_def_ipc_66433
zeb_def_ipc_20956			zeb_def_ipc_66729
zeb_def_ipc_20970			zeb_def_ipc_66761
zeb_def_ipc_21123			zeb_def_ipc_66798
zeb_def_ipc_21180			zeb_def_ipc_66855
zeb_def_ipc_21188			zeb_def_ipc_67075
zeb_def_ipc_21211			zeb_def_ipc_67831
zeb_def_ipc_21219			zeb_def_ipc_68003
zeb_def_ipc_21246			zeb_def_ipc_68274
zeb_def_ipc_21606			zeb_def_ipc_68329
zeb_def_ipc_21685			zeb_def_ipc_68480
zeb_def_ipc_22008			zeb_def_ipc_68648
zeb_def_ipc_2202			zeb_def_ipc_68728
zeb_def_ipc_22065			zeb_def_ipc_68789
zeb_def_ipc_22126			zeb_def_ipc_69031
zeb_def_ipc_22141			zeb_def_ipc_69189
zeb_def_ipc_22345			zeb_def_ipc_69274
zeb_def_ipc_22507			zeb_def_ipc_69385
zeb_def_ipc_22649			zeb_def_ipc_69431
zeb_def_ipc_22748			zeb_def_ipc_69450
zeb_def_ipc_23211			zeb_def_ipc_69714
zeb_def_ipc_23381			zeb_def_ipc_69806
zeb_def_ipc_23405			zeb_def_ipc_70093
zeb_def_ipc_23484			zeb_def_ipc_70406
zeb_def_ipc_23666			zeb_def_ipc_70505
zeb_def_ipc_24141			zeb_def_ipc_70596
zeb_def_ipc_24206			zeb_def_ipc_7070
zeb_def_ipc_24216			zeb_def_ipc_70743
zeb_def_ipc_24445			zeb_def_ipc_70769
zeb_def_ipc_24515			zeb_def_ipc_70886
zeb_def_ipc_24679			zeb_def_ipc_70904
zeb_def_ipc_24701			zeb_def_ipc_71009
zeb_def_ipc_24770			zeb_def_ipc_71033
zeb_def_ipc_24783			zeb_def_ipc_71063
zeb_def_ipc_24833			zeb_def_ipc_71100
zeb_def_ipc_24862			zeb_def_ipc_71160
zeb_def_ipc_24918			zeb_def_ipc_7128
zeb_def_ipc_24966			zeb_def_ipc_71423
zeb_def_ipc_25256			zeb_def_ipc_71534
zeb_def_ipc_25342			zeb_def_ipc_71584
zeb_def_ipc_25371			zeb_def_ipc_71635
zeb_def_ipc_25405			zeb_def_ipc_71869
zeb_def_ipc_25634			zeb_def_ipc_71987
zeb_def_ipc_25671			zeb_def_ipc_72188
zeb_def_ipc_2568			zeb_def_ipc_7234
zeb_def_ipc_25827			zeb_def_ipc_72515
zeb_def_ipc_26172			zeb_def_ipc_72567
zeb_def_ipc_26196			zeb_def_ipc_72762
zeb_def_ipc_26568			zeb_def_ipc_73071
zeb_def_ipc_26668			zeb_def_ipc_73168
zeb_def_ipc_26830			zeb_def_ipc_73211
zeb_def_ipc_27123			zeb_def_ipc_73656
zeb_def_ipc_27217			zeb_def_ipc_7367
zeb_def_ipc_27403			zeb_def_ipc_7370
zeb_def_ipc_2744			zeb_def_ipc_73806
zeb_def_ipc_27577			zeb_def_ipc_73836
zeb_def_ipc_27918			zeb_def_ipc_74003
zeb_def_ipc_28092			zeb_def_ipc_74195
zeb_def_ipc_28254			zeb_def_ipc_74205
zeb_def_ipc_283				zeb_def_ipc_74207
zeb_def_ipc_2833			zeb_def_ipc_74267
zeb_def_ipc_28478			zeb_def_ipc_74339
zeb_def_ipc_28557			zeb_def_ipc_74371
zeb_def_ipc_28641			zeb_def_ipc_74583
zeb_def_ipc_28752			zeb_def_ipc_74800
zeb_def_ipc_2879			zeb_def_ipc_74940
zeb_def_ipc_28938			zeb_def_ipc_74963
zeb_def_ipc_29255			zeb_def_ipc_75127
zeb_def_ipc_29362			zeb_def_ipc_75229
zeb_def_ipc_29461			zeb_def_ipc_75451
zeb_def_ipc_29598			zeb_def_ipc_75534
zeb_def_ipc_29639			zeb_def_ipc_75753
zeb_def_ipc_29659			zeb_def_ipc_75976
zeb_def_ipc_29883			zeb_def_ipc_75984
zeb_def_ipc_29896			zeb_def_ipc_76039
zeb_def_ipc_29971			zeb_def_ipc_76234
zeb_def_ipc_29980			zeb_def_ipc_7646
zeb_def_ipc_30224			zeb_def_ipc_76485
zeb_def_ipc_30231			zeb_def_ipc_7659
zeb_def_ipc_30254			zeb_def_ipc_76659
zeb_def_ipc_3032			zeb_def_ipc_76748
zeb_def_ipc_30347			zeb_def_ipc_76772
zeb_def_ipc_3035			zeb_def_ipc_76777
zeb_def_ipc_30783			zeb_def_ipc_76823
zeb_def_ipc_30901			zeb_def_ipc_76989
zeb_def_ipc_31112			zeb_def_ipc_77320
zeb_def_ipc_31544			zeb_def_ipc_77402
zeb_def_ipc_3163			zeb_def_ipc_77421
zeb_def_ipc_31643			zeb_def_ipc_77687
zeb_def_ipc_31737			zeb_def_ipc_77822
zeb_def_ipc_31843			zeb_def_ipc_7798
zeb_def_ipc_31982			zeb_def_ipc_78087
zeb_def_ipc_32017			zeb_def_ipc_781
zeb_def_ipc_32161			zeb_def_ipc_78467
zeb_def_ipc_32315			zeb_def_ipc_7849
zeb_def_ipc_32320			zeb_def_ipc_78614
zeb_def_ipc_32335			zeb_def_ipc_78845
zeb_def_ipc_32658			zeb_def_ipc_78892
zeb_def_ipc_32738			zeb_def_ipc_78901
zeb_def_ipc_32749			zeb_def_ipc_79037
zeb_def_ipc_32883			zeb_def_ipc_79126
zeb_def_ipc_32982			zeb_def_ipc_79193
zeb_def_ipc_33004			zeb_def_ipc_7922
zeb_def_ipc_33013			zeb_def_ipc_79641
zeb_def_ipc_33223			zeb_def_ipc_79682
zeb_def_ipc_33276			zeb_def_ipc_79752
zeb_def_ipc_33336			zeb_def_ipc_7989
zeb_def_ipc_33370			zeb_def_ipc_7998
zeb_def_ipc_33378			zeb_def_ipc_80137
zeb_def_ipc_33691			zeb_def_ipc_80237
zeb_def_ipc_33713			zeb_def_ipc_80264
zeb_def_ipc_33832			zeb_def_ipc_80295
zeb_def_ipc_34009			zeb_def_ipc_80444
zeb_def_ipc_34331			zeb_def_ipc_80865
zeb_def_ipc_35086			zeb_def_ipc_80955
zeb_def_ipc_35113			zeb_def_ipc_80969
zeb_def_ipc_35227			zeb_def_ipc_81006
zeb_def_ipc_35363			zeb_def_ipc_81070
zeb_def_ipc_3581			zeb_def_ipc_81131
zeb_def_ipc_35863			zeb_def_ipc_81189
zeb_def_ipc_35905			zeb_def_ipc_8123
zeb_def_ipc_3610			zeb_def_ipc_81260
zeb_def_ipc_3611			zeb_def_ipc_8136
zeb_def_ipc_36138			zeb_def_ipc_81556
zeb_def_ipc_36187			zeb_def_ipc_81789
zeb_def_ipc_36551			zeb_def_ipc_81839
zeb_def_ipc_36804			zeb_def_ipc_8191
zeb_def_ipc_36809			zeb_def_ipc_820
zeb_def_ipc_36877			zeb_def_ipc_82217
zeb_def_ipc_36891			zeb_def_ipc_8233
zeb_def_ipc_3690			zeb_def_ipc_82482
zeb_def_ipc_36938			zeb_def_ipc_82484
zeb_def_ipc_37314			zeb_def_ipc_82632
zeb_def_ipc_37330			zeb_def_ipc_82689
zeb_def_ipc_37423			zeb_def_ipc_82743
zeb_def_ipc_37529			zeb_def_ipc_82744
zeb_def_ipc_37667			zeb_def_ipc_82989
zeb_def_ipc_37672			zeb_def_ipc_83025
zeb_def_ipc_37882			zeb_def_ipc_831
zeb_def_ipc_37979			zeb_def_ipc_83174
zeb_def_ipc_38035			zeb_def_ipc_83183
zeb_def_ipc_38036			zeb_def_ipc_83480
zeb_def_ipc_38090			zeb_def_ipc_83570
zeb_def_ipc_38209			zeb_def_ipc_83614
zeb_def_ipc_38255			zeb_def_ipc_83792
zeb_def_ipc_3837			zeb_def_ipc_83797
zeb_def_ipc_38413			zeb_def_ipc_83815
zeb_def_ipc_38442			zeb_def_ipc_84038
zeb_def_ipc_39020			zeb_def_ipc_84081
zeb_def_ipc_39282			zeb_def_ipc_84324
zeb_def_ipc_39330			zeb_def_ipc_84599
zeb_def_ipc_39347			zeb_def_ipc_84699
zeb_def_ipc_3956			zeb_def_ipc_85047
zeb_def_ipc_3958			zeb_def_ipc_85106
zeb_def_ipc_39600			zeb_def_ipc_85194
zeb_def_ipc_39633			zeb_def_ipc_85299
zeb_def_ipc_39637			zeb_def_ipc_85368
zeb_def_ipc_40068			zeb_def_ipc_85580
zeb_def_ipc_40170			zeb_def_ipc_85772
zeb_def_ipc_40300			zeb_def_ipc_8599
zeb_def_ipc_40342			zeb_def_ipc_86009
zeb_def_ipc_40465			zeb_def_ipc_86095
zeb_def_ipc_40861			zeb_def_ipc_86176
zeb_def_ipc_40883			zeb_def_ipc_86218
zeb_def_ipc_41118			zeb_def_ipc_86241
zeb_def_ipc_41131			zeb_def_ipc_86424
zeb_def_ipc_41217			zeb_def_ipc_8680
zeb_def_ipc_41355			zeb_def_ipc_8700
zeb_def_ipc_41411			zeb_def_ipc_87068
zeb_def_ipc_41461			zeb_def_ipc_87080
zeb_def_ipc_41513			zeb_def_ipc_87127
zeb_def_ipc_41638			zeb_def_ipc_87183
zeb_def_ipc_41682			zeb_def_ipc_87200
zeb_def_ipc_41695			zeb_def_ipc_87202
zeb_def_ipc_41718			zeb_def_ipc_87340
zeb_def_ipc_41763			zeb_def_ipc_87655
zeb_def_ipc_41788			zeb_def_ipc_87673
zeb_def_ipc_41953			zeb_def_ipc_87884
zeb_def_ipc_41971			zeb_def_ipc_87890
zeb_def_ipc_42002			zeb_def_ipc_88452
zeb_def_ipc_42287			zeb_def_ipc_88536
zeb_def_ipc_43091			zeb_def_ipc_8855
zeb_def_ipc_43200			zeb_def_ipc_88564
zeb_def_ipc_43859			zeb_def_ipc_88627
zeb_def_ipc_4403			zeb_def_ipc_89040
zeb_def_ipc_44090			zeb_def_ipc_89062
zeb_def_ipc_44288			zeb_def_ipc_89115
zeb_def_ipc_4429			zeb_def_ipc_89209
zeb_def_ipc_44314			zeb_def_ipc_89214
zeb_def_ipc_4450			zeb_def_ipc_89808
zeb_def_ipc_44640			zeb_def_ipc_89819
zeb_def_ipc_44663			zeb_def_ipc_90371
zeb_def_ipc_44718			zeb_def_ipc_90487
zeb_def_ipc_44868			zeb_def_ipc_90488
zeb_def_ipc_44885			zeb_def_ipc_90532
zeb_def_ipc_45087			zeb_def_ipc_90621
zeb_def_ipc_45100			zeb_def_ipc_90672
zeb_def_ipc_45246			zeb_def_ipc_90808
zeb_def_ipc_45263			zeb_def_ipc_90958
zeb_def_ipc_45312			zeb_def_ipc_91207
zeb_def_ipc_45384			zeb_def_ipc_91242
zeb_def_ipc_45390			zeb_def_ipc_91411
zeb_def_ipc_45473			zeb_def_ipc_91517
zeb_def_ipc_45898			zeb_def_ipc_91566
zeb_def_ipc_46232			zeb_def_ipc_91580
zeb_def_ipc_46353			zeb_def_ipc_91624
zeb_def_ipc_46512			zeb_def_ipc_91667
zeb_def_ipc_4662			zeb_def_ipc_92015
zeb_def_ipc_46699			zeb_def_ipc_92164
zeb_def_ipc_46727			zeb_def_ipc_92241
zeb_def_ipc_4688			zeb_def_ipc_92310
zeb_def_ipc_46923			zeb_def_ipc_9239
zeb_def_ipc_46930			zeb_def_ipc_92394
zeb_def_ipc_47039			zeb_def_ipc_92523
zeb_def_ipc_47055			zeb_def_ipc_92604
zeb_def_ipc_47131			zeb_def_ipc_92718
zeb_def_ipc_47175			zeb_def_ipc_9273
zeb_def_ipc_4769			zeb_def_ipc_92912
zeb_def_ipc_47745			zeb_def_ipc_92939
zeb_def_ipc_47764			zeb_def_ipc_93123
zeb_def_ipc_47916			zeb_def_ipc_93234
zeb_def_ipc_4792			zeb_def_ipc_93336
zeb_def_ipc_47961			zeb_def_ipc_93370
zeb_def_ipc_48358			zeb_def_ipc_93480
zeb_def_ipc_48536			zeb_def_ipc_93571
zeb_def_ipc_48580			zeb_def_ipc_93733
zeb_def_ipc_48845			zeb_def_ipc_93881
zeb_def_ipc_4886			zeb_def_ipc_94151
zeb_def_ipc_48883			zeb_def_ipc_9430
zeb_def_ipc_48932			zeb_def_ipc_94329
zeb_def_ipc_49065			zeb_def_ipc_94687
zeb_def_ipc_49120			zeb_def_ipc_94800
zeb_def_ipc_49219			zeb_def_ipc_94805
zeb_def_ipc_49287			zeb_def_ipc_95282
zeb_def_ipc_49289			zeb_def_ipc_95298
zeb_def_ipc_49399			zeb_def_ipc_95389
zeb_def_ipc_49439			zeb_def_ipc_95400
zeb_def_ipc_49520			zeb_def_ipc_95416
zeb_def_ipc_49531			zeb_def_ipc_9555
zeb_def_ipc_4963			zeb_def_ipc_95821
zeb_def_ipc_49708			zeb_def_ipc_95947
zeb_def_ipc_49778			zeb_def_ipc_96037
zeb_def_ipc_49912			zeb_def_ipc_96082
zeb_def_ipc_49938			zeb_def_ipc_96109
zeb_def_ipc_50031			zeb_def_ipc_96233
zeb_def_ipc_50081			zeb_def_ipc_96366
zeb_def_ipc_50086			zeb_def_ipc_9642
zeb_def_ipc_50250			zeb_def_ipc_9671
zeb_def_ipc_50284			zeb_def_ipc_96988
zeb_def_ipc_50344			zeb_def_ipc_9708
zeb_def_ipc_50940			zeb_def_ipc_97253
zeb_def_ipc_51343			zeb_def_ipc_97279
zeb_def_ipc_51385			zeb_def_ipc_97286
zeb_def_ipc_52556			zeb_def_ipc_9746
zeb_def_ipc_52603			zeb_def_ipc_97569
zeb_def_ipc_52651			zeb_def_ipc_97585
zeb_def_ipc_52667			zeb_def_ipc_97639
zeb_def_ipc_52688			zeb_def_ipc_9780
zeb_def_ipc_52701			zeb_def_ipc_97997
zeb_def_ipc_52808			zeb_def_ipc_98181
zeb_def_ipc_52822			zeb_def_ipc_98214
zeb_def_ipc_52886			zeb_def_ipc_98402
zeb_def_ipc_52969			zeb_def_ipc_98702
zeb_def_ipc_52978			zeb_def_ipc_98724
zeb_def_ipc_53094			zeb_def_ipc_98913
zeb_def_ipc_53470			zeb_def_ipc_99162
zeb_def_ipc_53550			zeb_def_ipc_99217
zeb_def_ipc_53645			zeb_def_ipc_99240
zeb_def_ipc_54073			zeb_def_ipc_99335
zeb_def_ipc_54106			zeb_def_ipc_99502
zeb_def_ipc_5415			zeb_def_ipc_99518
zeb_def_ipc_54296			zeb_def_ipc_99534
zeb_def_ipc_54298			zeb_def_ipc_99598
zeb_def_ipc_54365			zeb_def_ipc_99621
zeb_def_ipc_54397			zeb_def_ipc_99670
zeb_def_ipc_54417			zeb_def_ipc_9970
zeb_def_ipc_54451			zeb_def_ipc_99701
zeb_def_ipc_54566			zeb_def_ipc_99764
zeb_def_ipc_54568			zeb_def_ipc_99886


    zhenya@Air-Evgenij /tmp % cd /var/log
    zhenya@Air-Evgenij log % cd ..
    zhenya@Air-Evgenij /var % cd -
/var/log
    zhenya@Air-Evgenij log % man pwd

PWD(1)                      General Commands Manual                     PWD(1)

NAME
     pwd – return working directory name

SYNOPSIS
     pwd [-L | -P]

DESCRIPTION
     The pwd utility writes the absolute pathname of the current working
     directory to the standard output.

     Some shells may provide a builtin pwd command which is similar or
     identical to this utility.  Consult the builtin(1) manual page.

     The options are as follows:

     -L      Display the logical current working directory.

     -P      Display the physical current working directory (all symbolic
             links resolved).

     If no options are specified, the -L option is assumed.
:
