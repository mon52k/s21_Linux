## Part 1
![screenshot](Allpart/part1/udu1.png)
- Команда показать версию ubuntu и ее результат.

## Part 2
![screenshot](Allpart/part2/ubu2.1.png)
- Добавление нового пользователя.

![screenshot](Allpart/part2/ubu2.2.png)
- Добавление нового пользователя в команду adm.

![screenshot](Allpart/part2/ubu2.3.png)
- Результат команды `cat /etc/passwd`.

## Part 3

![screenshot](Allpart/part3/ubu3.1.png)
- Изменение имени хоста командой `sudo hostnamectl set-hostname name`.
- Обновление имени хоста командой `exec bash`.
- Вывод нового имени хоста.

![screenshot](Allpart/part3/ubu3.2.png)
- Командой `timedatectl` узнаем текущую временную зону.
- Командой `sudo timedatectl set-timezone Europe/Moscow` меняем текущую временную зону.

![screenshot](Allpart/part3/ubu3.3.png)
- Командой `ifconfig -a` узнаем названия сетевых интерфейсов.
- Или командой `ip link` узнаем названия сетевых интерфейсов.

#### Интерфейс <span style="color: blue;">lo</span> представляет собой виртуальный интерфейс, который используется для взаимодействия процессов на самом компьютере без обращения к физической сети.
#### Он обычно имеет IP-адрес <span style="color: blue;">127.0.0.1</span> (localhost), который указывает на сам компьютер.
#### Интерфейс <span style="color: blue;">lo</span> является неотъемлемой частью конфигурации сети в Linux и других операционных системах.
#### Он обеспечивает стабильное и надежное взаимодействие приложений.
<br>

![screenshot](Allpart/part3/ubu3.4.png)
- Командой `ifconfig` узнаем названия сетевых интерфейсов.
- Или командой `ip addr` узнаем названия сетевых интерфейсов.

#### **Dynamic** - Динамический
#### **DHCP** позволяет динамически (автоматически) назначать IP-адреса и другие сетевые параметры устройствам в сети.
#### **Host** - Хост
#### Хост обозначает устройство (например, компьютер или смартфон), которому присваивается сетевая конфигурация.
#### **Configuration** - Конфигурация
#### DHCP конфигурирует (устанавливает) сетевые параметры устройства, такие как IP-адрес, шлюз, DNS-серверы и другие настройки.
#### **Protocol** - Протокол
#### **DHCP** является сетевым протоколом, обеспечивающим автоматическую настройку IP-адресов и других сетевых параметров в компьютерных сетях.
#### Таким образом, **Dynamic Host Configuration Protocol (DHCP)** представляет собой протокол для автоматической настройки сетевых параметров устройств в компьютерных сетях, что делает процесс управления IP-адресами и другими параметрами более эффективным и удобным для администраторов сети и пользователей.
<br>

![screenshot](Allpart/part3/ubu3.5.png)
- Командой `curl ifconfig.me/ip` узнаем внешний ip-адрес шлюза.
- Командой `ip route` узнаем внутренний IP-адрес шлюза.

![screenshot](Allpart/part3/ubu3.6.png)
- Командой ` sudo nano /etc/netplan/00-installer-config.yaml` открываем файл и заполняем как на скрине.
- Командой `sudo netplan apply` применить настройки.
- Командой `sudo reboot` перезагрузить.

![screenshot](Allpart/part3/ubu3.7.png)
- Командой `ip route show` проверить после перезагрузки.

![screenshot](Allpart/part3/ubu3.8.png)
- Командой `ping 1.1.1.1` проверить после перезагрузки.

## Part 4


![screenshot](Allpart/part4/ubu4.1.png)
![screenshot](Allpart/part4/ubu4.2.png)
![screenshot](Allpart/part4/ubu4.3.png)
- Командой `sudo apt update` обновляем список доступных пакетов с репозиториев.
- Командой `sudo apt upgrade` обновляем.
- Командой `sudo apt update` проверяем после обновления.

## Part 5

![screenshot](Allpart/part5/ubu5.1.png)
- Командой `sudo usermod -aG sudo name` добавляем пользователя в группу sudo.

#### Команда **sudo** ( **substitute user and do**, подменить пользователя и выполнить ) позволяет строго определенным пользователям выполнять указанные программы с административными привилегиями без ввода пароля суперпользователя **root**. Если быть точнее, то команда **sudo** позволяет выполнять программы от имени любого пользователя, но, если идентификатор или имя этого пользователя не указаны, то предполагается выполнение от имени суперпользователя **root**. Таким образом, использование sudo позволяет выполнять привилегированные команды обычным пользователям без необходимости ввода пароля суперпользователя **root**. Список пользователей и перечень их прав по отношению к ресурсам системы может быть настроен оптимальным образом для обеспечения комфортной и безопасной работы. Например, команда **sudo** в **Ubuntu Linux**, используется в режиме, позволяющем выполнять любые задачи администрирования системы без интерактивного входа под учетной записью **root**.
</br>

![screenshot](Allpart/part5/ubu5.2.png)
- Командой `hostname` смотрим имя хоста.
- Командой `su name` переходим на пользователя созданого в **Allpart/part 2**.
- Командой `sudo hostnamectl set-hostname name` меняем имя.
- Командой `hostname` смотрим имя хоста.

## Part 6

![screenshot](Allpart/part6/ubu6.1.png)
- Командой `timedatectl show` смотрим время.

## Part 7

![screenshot](Allpart/part7/ubu7.1.png)
- Сохранить `Ctrl + O`, затем нажмите Enter для сохранения, и `Ctrl + X` для выхода.

![screenshot](Allpart/part7/ubu7.2.png)
- `:wq` и нажмите Enter для сохранения и выхода.

![screenshot](Allpart/part7/ubu7.3.1.png)
Чтобы сохранить изменения и выйти, нажмите `Ctrl + K - X` , 

![screenshot](Allpart/part7/ubu7.3.png)
- Чтобы выйти без сохранения изменений `Ctrl + X`.

![screenshot](Allpart/part7/ubu7.4.png)
- Чтобы выйти без сохранения изменений `:q!`.

![screenshot](Allpart/part7/ubu7.5.png)
- Чтобы выйти без записи `Ctrl + С`, с запросом на подтверждение утраты сделанных изменений, буде таковые имелись;

![screenshot](Allpart/part7/ubu7.6.png)
- Результат не изменился.

![screenshot](Allpart/part7/ubu7.7.png)
![screenshot](Allpart/part7/ubu7.8.png)
- `Option R` сначало слово поиска потом слово замены.

![screenshot](Allpart/part7/ubu7.9.png)
- Команда `:%s/twitchis/21 School 21/g` для замены.

![screenshot](Allpart/part7/ubu7.9.1.png)
![screenshot](Allpart/part7/ubu7.9.2.png)
`Ctrl+K-F` замена; для замены надо в опциях (запрашиваются после ввода образца) указать R Поиск/замена понимает регулярные выражения

## Part 8

![screenshot](Allpart/part8/ubu8.1.png)
- Команда `sudo apt install ssh` для установки SSH.

![screenshot](Allpart/part8/ubu8.2.png)
- Добавление автостарта для ssh.

![screenshot](Allpart/part8/ubu8.3.png)
- Переписал порт с 22 на 2022.
![screenshot](Allpart/part8/ubu8.4.png)
- Команда ps с ключами -axfv



![screenshot](Allpart/part8/ubu8.5.png)
-a: Выбрать все процессы, кроме лидеров сеансов и процессов, не связанных с терминалом.\

![screenshot](Allpart/part8/ubu8.5.1.png)
-x: Заставляет ps отображать список всех процессов, которыми вы владеете (тот же EUID, что и у ps), или перечислять все процессы при использовании вместе с опцией a.\

![screenshot](Allpart/part8/ubu8.5.3.png)
-f: Выводить полноформатный список\

![screenshot](Allpart/part8/ubu8.5.2.png)
-v: Выводить информацию о версии

![screenshot](Allpart/part8/ubu8.6.png)
- Вывод команды `netstat -tan` должен содержать `tcp 0 0 0.0.0.0:2022 0.0.0.0:* LISTEN`

-a показывает состояние всех сокетов\
-n показывает ip адрес, а не сетевое имя\
-t показывает только tcp соединения.

Значения столбцов:

Proto - протокол, используемый сокетом;\
Recv-Q - количество байтов, не скопированных пользовательской программой, подключенной к этому сокету\
Local Address - локальный адрес (имя локального хоста) и номер порта сокета\
Foreign Address - удаленный адрес (имя удаленного хоста) и номер порта сокета\
State - состояние сокета\
0.0.0.0 в этом контексте означает "все IP-адреса на локальной машине"

## Part 9



![screenshot](Allpart/part9/ubu9.png)
- Запустил утилиту Top.

![screenshot](Allpart/part9/ubu9.1.png)
- Запустил утилиту Htop.

- По выводу команды top определи и напиши в отчёте:
    - uptime 00:50:31 min
    - количество авторизованных пользователей 1
    - общую загрузку системы 0,07 0,02 0,00
    - общее количество процессов 94 total
    - загрузку cpu 0,0 us 0,0 sy 0,0 ni 0,0 si 0,0 st
    - загрузку памяти 146,3 used
    - pid процесса занимающего больше всего памяти 1473
    - pid процесса, занимающего больше всего процессорного времени 1473
htop отсортированному по PID, PERCENT_CPU, PERCENT_MEM, TIME 




![screenshot](Allpart/part9/ubu9.2.png)
- Сортировка PID.

![screenshot](Allpart/part9/ubu9.2.1.png)
- Сортировка PERCENT_CPU.

![screenshot](Allpart/part9/ubu9.2.2.png)
- Сортировка PERCENT_MEM.

![screenshot](Allpart/part9/ubu9.2.3.png)
- Сортировка TIME.


![screenshot](Allpart/part9/ubu9.2.4.png)

- отфильтрованному для процесса sshd.

![screenshot](Allpart/part9/ubu9.2.5.png)
- с процессом syslog, найденным, используя поиск.

![screenshot](Allpart/part9/ubu9.2.6.png)
- с добавленным выводом hostname, clock и uptime.

## Part 10

![screenshot](Allpart/part10/ubu10.1.png)
- название жесткого диска: **/dev/sda**
- его размер и количество секторов: **26843545600 bytes, 52428800 sectors**

![screenshot](Allpart/part10/ubu10.2.png)
- размер swap: **2 GiB (swapon --show)**

## Part 11

![screenshot](Allpart/part11/ubu11.1.png)
`df /` для корневого раздела

- В отчёте напиши для корневого раздела (/):
    - размер раздела: **11758760**
    - размер занятого пространства: **4769196**
    - размер свободного пространства: **6370456**
    - процент использования: **43%**

- Стандартно в выводе df используются килобайты, но можно добавить флаг -h чтобы налядно видеть единицы измерения.

![screenshot](sAllpart/part11/ubu11.2.png)
- `df /` для корневого раздела
df -Th / для корневого раздела (флаг -h для единиц измерения, -T для вывода типа файловой системы)

-- В отчёте напиши для корневого раздела (/):
    - размер раздела: **12G**
- размер занятого пространства: **4,6G**
- размер свободного пространства: **6,1G**
- процент использования: **43%**
- тип файловой системы для раздела: **ext4**

## Part 12

![screenshot](Allpart/part12/ubu12.1.png)
- Вывод `du`.

![screenshot](Allpart/part12/ubu12.2.png)
- `du -sb` (-b в байтах -s показывает только суммарные данные).

![screenshot](Allpart/part12/ubu12.3.png)
- `du -sb /var/log/*`.

## Part 13
![screenshot](Allpart/part13/ubu13.1.png)
* Установи утилиту ncdu

`sudo apt install ncdu`

* Выведи размер папок /home, /var, /var/log

![screenshot](Allpart/part13/ubu13.2.1.png)\
/home

![screenshot](Allpart/part13/ubu13.2.2.png)\
/var

![screenshot](Allpart/part13/ubu13.2.3.png)\
/var/log

## Part 14

* Открой для просмотра:
##### 1. /var/log/dmesg
![screenshot](Allpart/part14/ubu14.1.png)
- `nano -v /var/log/dmesg`
##### 2. /var/log/syslog
![screenshot](Allpart/part14/ubu14.2.png)
- `nano -v /var/log/syslog`
##### 3. /var/log/auth.log
![screenshot](Allpart/part14/ubu14.3.png)  
- `nano -v /var/log/auth.log`

 Напиши в отчёте время последней успешной авторизации: 
 ![screenshot](Allpart/part14/ubu14.4.png)
* FEB 16 12:24:37 `cat /var/log/auth.log | grep "session"`
* имя пользователя: twitchis 
* и метод входа в систему: TTY: tty1 
* Перезапусти службу SSHd\
![screenshot](Allpart/part14/ubu14.5.png)
`sudo systemctl restart ssh`

* Вставь в отчёт скрин с сообщением о рестарте службы (искать в логах).

![screenshot](Allpart/part14/ubu14.6.png)
- Логи о перезапуске службы

## **Part 15**

- Для использования планировщика заданий `CRON` необходимо его установить при помощи команды
    
    ![screenshot](Allpart/part15/ubu15.1.png)
> sudo apt install cron

- Для работы в фоновом режиме необходимо использовать команду
   ![screenshot](Allpart/part15/ubu15.2.png)

> sudo systemctl enable cron
> 

![screenshot](Allpart/part15/ubu15.3.png)

- Для редактирования `crontab -e` , далее выбрать редактор
- Назначаем команду для запуска каждые 2 минуты `/2 * * * * uptime`

![screenshot](Allpart/part15/ubu15.4.png)

- Для проверки автозапуска команд в `/var/log/syslog`
- Проверяем текущие задачи cron
    
![screenshot](Allpart/part15/ubu15.5.png)
    
> crontab -l

- Для удаления задач cron пишем
    
   ![screenshot](Allpart/part15/ubu15.6.png)

> crontab -r

Готово