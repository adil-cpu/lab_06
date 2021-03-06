# Презентация к лабораторной работе №6
# Анализ файловой системы Linux. Команды для работы с файлами и каталогами

----

## Российский Университет Дружбы Народов

### Факульткт Физико-Математических и Естественных Наук

*Дисциплина: Операционные системы*

Студент: Мухамедияр Адиль

Группа: НКНбд-01-20

Москва, 2021г.

----

### Цель работы

Ознакомление с файловой системой Linux, её структурой, именами и содержанием каталогов. Приобретение практических навыков по применению команд для работы с файлами и каталогами, по управлению процессами (и работами), по проверке использования диска и обслуживанию файловой системы.

----

### Ход работы:
1. Выполнил все примеры, приведённые в первой части описания лабораторной работы.

![1_1.png](https://raw.githubusercontent.com/adil-cpu/lab_06/main/img_06/1_1.PNG)

![1_2.png](https://raw.githubusercontent.com/adil-cpu/lab_06/main/img_06/1_2.PNG)

2.	Выполнил следующие действия:

* Скопировал файл /usr/include/sys/io.txt в домашний каталог и назвал его equipment.
* В домашнем каталоге создал директорию ~/ski.plases.
* Переместил файл equipment в каталог ~/ski.plases.
* Переименовал файл ~/ski.plases/equipment в ~/ski.plases/equiplist.
*  домашнем каталоге создал файл abc1 и скопировал его в каталог ~/ski.plases, назвал его equiplist2.
* Создал каталог с именем equipment в каталоге ~/ski.plases.
* Переместил файлы ~/ski.plases/equiplist и equiplist2 в каталог ~/ski.plases/equipment.
* Создал и переместил каталог ~/newdir в каталог ~/ski.plases, назвав его plans.
 
[![2.png](https://raw.githubusercontent.com/adil-cpu/lab_06/main/img_06/2.PNG)

 3.	Определил опции команды chmod, необходимые для того, чтобы присвоить перечисленным ниже файлам выделенные права доступа, считая, что в начале таких прав нет:

* drwxr--r-- ... australia
* drwx--x--x ... play
* -r-xr--r-- ... my_os
* -rw-rw-r-- ... feathers

![3.png](https://raw.githubusercontent.com/adil-cpu/lab_06/main/img_06/3.PNG)

 4.	Проделал приведённые ниже упражнения, записывая в отчёт по лабораторной работе используемые при этом команды:

* Просмотрел содержимое файла /etc/password.

![4_1.png](https://raw.githubusercontent.com/adil-cpu/lab_06/main/img_06/4_1.PNG)

* Скопировал файл ~/feathers в файл ~/file.old.
* Переместил файл ~/file.old в каталог ~/play.
* Скопировал каталог ~/play в каталог ~/fun.
* Переместил каталог ~/fun в каталог ~/play и назвала его games.

 ![4_2.png](https://raw.githubusercontent.com/adil-cpu/lab_06/main/img_06/4_2.PNG)

* Лишил владельца файла ~/feathers права на чтение.
* Не олучилось просмотреть файл ~/feathers командой cat.
* Не получилось скопировать файл ~/feathers.
* Дал владельцу файла ~/feathers право на чтение.

![4_3.png](https://raw.githubusercontent.com/adil-cpu/lab_06/main/img_06/4_3.PNG)

* Лишил владельца каталога ~/play права на выполнение.
* НЕ получилось перейти в каталог ~/play.
* Дал владельцу каталога ~/play право на выполнение

![4_4.png](https://raw.githubusercontent.com/adil-cpu/lab_06/main/img_06/4_4.PNG)

5.	
![5_1.png](https://raw.githubusercontent.com/adil-cpu/lab_06/main/img_06/5_1.PNG)

* mount - нужна для просмотра смонтированных файловых систем, а также для монтирования любых локальных или удаленных файловых систем. Например, при вызове команды «mount /dev/cdrom /mnt/cdrom» устройство /dev/cdrom монтируется в каталог /mnt/cdrom, если он существует. Начиная от момента монтирования и пока пользователь не отмонтирует файловую систему (или туда не будет смонтировано что-то иное) в каталоге /mnt/cdrom будет содержаться дерево каталогов устройства /dev/cdrom; те файлы, и подкаталоги, которые раньше находились в /mnt/cdrom, сохранятся, но будут недоступны до размонтирования устройства /dev/cdrom. Для размонтирования достаточно указать точку монтирования или имя устройства, команда «umount /dev/cdrom». При запуске команды mount без параметров выводится список смонтированных файловых систем.

![5_2.png](https://raw.githubusercontent.com/adil-cpu/lab_06/main/img_06/5_2.PNG)

* fsck - проверяет и устраняет ошибки в файловой системе. Например, fsck -fy -t ext4 /dev/sda1. Опция -f (force) используется для принудительного выполнения проверки. Опция -y (yes) позволяет программе автоматически отвечать "да" на все вопросы в ходе работы.

![5_3.png](https://raw.githubusercontent.com/adil-cpu/lab_06/main/img_06/5_3.PNG)

* mkfs - действие заключается в создании указанной файловой системы на выбранном диске или разделе. Например, команда «mkfs-text2 /dev/hda1» создает файловую систему ext2 на разделе hda1.

![5_4.png](https://raw.githubusercontent.com/adil-cpu/lab_06/main/img_06/5_4.PNG)

* kill - завершает некорректно работающее приложение. Например, чтобы послать сигнал SIGKILL (он имеет номер 9) процессу 2811, необходимо вызвать команду «kill -9 2811».

![5_5.png](https://raw.githubusercontent.com/adil-cpu/lab_06/main/img_06/5_5.PNG)

----

### Вывод

Ознакомился с файловой системой Linux, её структурой, именами и содержанием каталогов. Приобрел практические навыки по применению команд для работы с файлами и каталогами, по управлению процессами (и работами), по про- верке использования диска и обслуживанию файловой системы.

----
