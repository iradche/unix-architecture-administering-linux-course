## День 1
* Введение (краткая история Unix и Linux, диаграмма эволюции Unix https://en.wikipedia.org/wiki/Unix#/media/File:Unix_history-simple.svg)
* Unix консоль как интерфейс к системе
* Демонстрация работы в консоли: ls -alF and ps
* Красота Linux консоли: zsh и oh-my-zsh
* Понятие пакета и пакетного менеджера
* Домашнее задание: написать сервер, показывающий динамическую веб-страницу (на любом ЯП)
* Анатомия Unix-системы: кернелспейс и юзерспейс
* Кольца (rings) процессора
* Очень краткая история операционных систем
* Дебаты Торвальдс-Танненбаум
* История дистрибутивов Linux
* Анатомия Unix-системы еще раз: все является файлом
* Файловые системы: стандарт файловой иерархии FHS
* Файлы /etc/fstab, /etc/mtab, проблемы /etc/mtab
* Файловые системы: superblock, inodes, blocks
* Файловые системы: hardlinks, symlinks
* Файловые системы: ext2, ext3, ext4, понятие журналирования, разные степени журналирования, понятние барьеров
* ext\*: место, зарезервированное для пользователя root
* Файловые системы: утилита blktrace
* Файловые системы: ZFS, алгоритм CoW, ARC, снэпшоты
* Утилита smartctl, SMART long tests

## День 2
* Файловые системы: снэпшоты как часть Disaster Recovery Plan
* Файловые системы: BTRFS
* Файловые системы: псевдо-файловые системы /dev, /proc, /sys
* Файловые системы: утилиты разметки fdisk, cfdisk, parted, работа с дисками в Advanced Format
* Файловые системы: утилита file
* Пользователи: файл /etc/passwd и его поля
* Пользователи: суперпользователи (понятие UID, соответствие UID и имен, UID 0) и обычные пользователи
* Пользователи: модель безопасности Unix
* Модель безопасности Unix: подсистема PAM
* Модель безопасности Unix: su и sudo
* Модель безопасности Unix применительно к файловым системам: традиционные права
* Права на файлы и флаги: биты rwx
* Права на файлы и флаги: биты SUID и SGID
* Права на файлы и флаги: sticky bit
* Модель безопасности Unix применительно к файловым системам: расширенные атрибуты, SELinux и другие MAC/RBAC фреймворки (GRSecurity, Tomoyo)
* Модель безопасности Unix применительно к файловым системам: POSIX ACLs
* AppArmor и его проблемы
* Модель памяти: использованная память, swap и RSS
* Модель памяти: zram
* Модель памяти: KSM и UKSM
* Модель памяти применительно к файловым системам: block cache
* Процессы и межпроцессное взаимодействие: порядок запуска программы из бинарного файла на диске
* Процессы и межпроцессное взаимодействие: динамическая линковка и динамический линкер/загрузчик
* Процессы и межпроцессное взаимодействие: magic numbers
* Процессы и межпроцессное взаимодействие: стандартные файловые дескрипторы
* Процессы и файлы: файловые дескрипторы, стандартный API для чтения/записи
* Процессы и файлы: системный вызов ioctl и асинхронная обработка
* Процессы и межпроцессное взаимодействие: процесс-родитель и процесс-потомок, вызовы fork() и exec(), еще раз про алгоритм CoW
* Процессы и межпроцессное взаимодействие: пайпы
* Процессы и межпроцессное взаимодействие: сигналы и обработчики сигналов, утилита kill, сигнал SIGKILL и его особенности
* Процессы и межпроцессное взаимодействие: стандартные сигналы
* Процессы и межпроцессное взаимодействие: многопоточность, отображения потоков 1:1 и N:M
* Процессы и межпроцессное взаимодействие: лимиты (и /proc/XXXX/limits), утилита ulimit, файл /etc/security/limits.conf
* Процессы и межпроцессное взаимодействие: разделяемая память, семафоры, UNIX-сокеты
* Домашняя работа: система Vagrant

## День 3
* Процессы и межпроцессное взаимодействие: понятие niceness, утилиты nice и ionice
* Процесс загрузки Linux: BIOS и UEFI
* Процесс загрузки Linux: BIOS различных производителей и устройств
* Процесс загрузки Linux: MBR, формат записей MBR и GPT
* Процесс загрузки Linux: записи в таблице разделов
* Процесс загрузки Linux: загрузчики syslinux, LILO и GRUB
* Процесс загрузки Linux: загрузчик GRUB1 и его конфигурация, загрузчик GRUB2 и его конфигурация
* Процесс загрузки Linux: реальный и защищенный режимы
* Процесс загрузки Linux: статические файлы в /dev, подсистемы devfs и udev
* Процесс загрузки Linux: идентификаторы PCI и USB устройств, автоматическое определение и конфигурирование аппаратных устройств
* Процесс загрузки Linux: процесс init и файл /etc/inittab
* Процесс загрузки Linux: BSD initscripts и SysV initscripts, runlevels
* Процесс загрузки Linux: файлы initrd и initramfs
* Процесс загрузки Linux: внутреннее устройство файла initrd, модули ядра, фреймворк dracut
* Процесс загрузки Linux: параллельная загрузка, утилита bootchart, файл bootlog, параллельные инитскрипты
* Процесс загрузки Linux/Unix: фреймворки upstart, OpenRC, SMF
* Различные супервизоры: daemontools, runit, god, bluepill, eye, forever, supervisord
* Процесс загрузки Linux: systemd
* Процесс загрузки Linux: cgroups и namespaces, взаимоотношение cgroups, namespaces и systemd
* Логирование: syslog
* Логирование: ELK, Graylog, Splunk
* Сетевое взаимодействие: основы конфигурации сети
* Сетевое взаимодействие: TCP и UDP
* Сетевое взаимодействие: Network Manager
* Сетевое взаимодействие: утилита ethtool
* Сетевое взаимодействие: MAC-адрес
* Сетевое взаимодействие: утилита ifconfig
* Сетевое взаимодействие: утилита ip
* Сетевое взаимодействие: подсистема DNS и разрешение имен
* Сетевое взаимодействие: маршрутизация
* Сетевое взаимодействие: GRE и VXLAN туннели
* Сетевое взаимодействие: виртуальные частные сети IPsec
* Сетевое взаимодействие: виртуальные частные сети OpenVPN (второго и третьего уровня)
* Сетевое взаимодействие: утилиты tcpdump и Wireshark
* Сетевое взаимодействие: NFS
* Сетевое взаимодействие: Samba
* Сетевое взаимодействие: LDAP

## День 4
* Сетевое взаимодействие: подсистема netfilter и утилита iptables
* Сетевое взаимодействие: механизм port knocking
* Сетевое взаимодействие: модуль ipset
* Сетевое взаимодействие: механизм NAT (SNAT, DNAT) и masquerading
* Сетевое взаимодействие: таблица трекинга соединений
* Сетевое взаимодействие: сервис FTP
* Сетевое взаимодействие: сервис SSH, подсистемы scp и SFTP
* Сетевое взаимодействие: утилита ssh-agent
* Сетевое взаимодействие: протокол HTTP
* Сетевое взаимодействие: веб-серверы Apache и nginx, их отличия
* Сетевое взаимодействие: утилиты rsync and rsyncd
* Сетевое взаимодействие: утилита netcat
* Сетевое взаимодействие: протокол HTTPS, сертификаты, обмен ключами
* Сетевое взаимодействие: проксирование HTTP и HTTPS трафика, Squid
* Сетевое взаимодействие: IPsec и система racoon, конфигурация racoon
* Сетевое взаимодействие: IPsec и система OpenSWAN, конфигурация OpenSWAN
* Сетевое взаимодействие: IPsec и система StrongSWAN, конфигурация StrongSWAN
* Понятие скриптинга (разница между статическими и динамическими языками)
* Скриптинг на bash: интерактивный и неинтерактивный режим, конфигурационные файлы и порядок их применения
* Скриптинг на bash: переменные и экспорт переменных
* Скриптинг на bash: встроенные команды bash
* Скриптинг на bash: globs
* Скриптинг на bash: управляющие структуры (if, case, for)
* Скриптинг на bash: команда test и встроенная команда test
* Скриптинг на bash: "магические" переменные ($? и так далее)
* Скриптинг на bash: отладка
* Перенаправление ввода/вывода: >, >> and <
* Команды Unix: wc, cat, cut, sort
* Команды Unix: awk и sed 
* Команды Unix: find
* Команды Unix: xargs
* Понятие о системах контроля версий (SVN и Git)

## День 5
* Понятие наблюдаемости (observability)
* Средства observability в Linux: матрица Брэндана Грегга
* Средства трассировки: strace
* Средства трассировки: ltrace
* Средства трассировки: системный вызов ptrace()
* Отладчик gdb и отладочные символы
* Средства трассировки: Poor Man's Profiler
* Файлы core и команда отладчика gdb "backtrace"
* Наблюдаемость: утилита top
* Наблюдаемость: утилита atop
* Наблюдаемость: утилита mpstat
* Наблюдаемость: утилита iostat
* Наблюдаемость: утилита pidstat
* Наблюдаемость: утилита iotop
* Наблюдаемость: cat /proc/interrupts
* Наблюдаемость: система Munin
* Наблюдаемость: система Zabbix и time-series базы данных
* Наблюдаемость: стек Graphite
* Наблюдаемость: система netdata
* Наблюдаемость: утилита и подсистема perf
* Наблюдаемость: подсистема DTrace
* Наблюдаемость: подсистема BPF и утилиты BPF
* Наблюдаемость: flamegraphs
* Наблюдаемость: система kaldur
* Наблюдаемость: flamegraphs и динамические языки
* Домашняя работа: рассмотрение готового кода
* Домашняя работа: совместное написание кода
* Понятие пакетных менеджеров
* Пакетные менеджеры RPM и dpkg
* Системы Docker и Nix
* Домашняя работа: создание пакета под Debian с использованием FPM
* Домашняя работа: создание пакета под Debian с использованием checkinstall
* Домашняя работа: создание репозитория Debian
* Домашняя работа: стресс-тестирование с использованием ab
* Домашняя работа: стресс-тестирование с использованием siege
* Домашняя работа: написание файла-описателя сервиса для upstart
* Домашняя работа: написание файла-описателя сервиса для systemd
