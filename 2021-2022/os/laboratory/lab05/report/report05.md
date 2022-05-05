---
## Front matter
title: "Отчет"
subtitle: "Лабораторная работа №5"
author: "Павлова Варвара Юрьевна НПМбд-02-21 1032217616"

## Generic otions
lang: ru-RU
toc-title: "Содержание"

## Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

## Pdf output format
toc: true # Table of contents
toc-depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4
documentclass: scrreprt
## I18n polyglossia
polyglossia-lang:
  name: russian
  options:
	- spelling=modern
	- babelshorthands=true
polyglossia-otherlangs:
  name: english
## I18n babel
babel-lang: russian
babel-otherlangs: english
## Fonts
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase,Scale=0.9
## Biblatex
biblatex: true
biblio-style: "gost-numeric"
biblatexoptions:
  - parentracker=true
  - backend=biber
  - hyperref=auto
  - language=auto
  - autolang=other*
  - citestyle=gost-numeric
## Pandoc-crossref LaTeX customization
figureTitle: "Рис."
tableTitle: "Таблица"
listingTitle: "Листинг"
lofTitle: "Список иллюстраций"
lotTitle: "Список таблиц"
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Ознакомление с файловой системой Linux, ее структурой, именами и содержанием каталогов. Приобретение практических навыков по применению команд для работы с файлами и каталогами, обслуживания файловой системы.

# Задание

1. Выполнитевсепримеры,приведённыевпервойчастиописаниялабораторнойработы.
2. Выполните следующие действия, зафиксировав в отчёте по лабораторной работе
используемые при этом команды и результаты их выполнения:
	2.1. Скопируйте файл /usr/include/sys/io.h в домашний каталоги назовите его
	equipment.Если файла io.h нет,то используйтелюбойдругой файл в каталоге
	/usr/include/sys/ вместо него.
	2.2. В домашнем каталоге создайте директорию ~/ski.plases.
	2.3. Переместите файл equipment в каталог ~/ski.plases.
	2.4. Переименуйте файл ~/ski.plases/equipment в ~/ski.plases/equiplist.
	2.5. Создайте в домашнем каталоге файл abc1 и скопируйте его в каталог
	~/ski.plases,назовите его equiplist2.
	2.6. Создайте каталог с именем equipment в каталоге ~/ski.plases.
	2.7. Переместите файлы ~/ski.plases/equiplist и equiplist2 в каталог
	~/ski.plases/equipment.
	2.8. Создайте и переместите каталог ~/newdir в каталог ~/ski.plases и назовите
	его plans.
3. Определите опции команды chmod,необходимые длят ого,чтобы присвоить перечис-
ленным ниже файлам выделенные права доступа, считая, что в начале таких прав
нет:
	3.1. drwxr--r-- ... australia
	3.2. drwx--x--x ... play
	3.3. -r-xr--r-- ... my_os
	3.4. -rw-rw-r-- ... feathers
При необходимости создайте нужные файлы.
4. Проделайте приведённые ниже упражнения, записывая в отчёт по лабораторной
работе используемые при этом команды:
	4.1. Просмотрите содержимое файла /etc/password.
	4.2. Скопируйте файл ~/feathers в файл ~/file.old.
	4.3. Переместите файл ~/file.old в каталог ~/play.
	4.4. Скопируйте каталог ~/play в каталог ~/fun.
	4.5. Переместите каталог ~/fun в каталог ~/play и назовите его games.
	4.6. Лишите владельца файла ~/feathers права на чтение.
	4.7. Что произойдёт,если вы попытаетесь просмотреть файл ~/feathers командой
	cat?
	4.8. Что произойдёт,если вы попытаетесь скопировать файл ~/feathers?
	4.9. Дайте владельцу файла ~/feathers право на чтение.
	4.10. Лишите владельца каталога ~/play права на выполнение.
	4.11. Перейдите в каталог ~/play.Что произошло?
	4.12. Дайте владельцу каталога ~/play право на выполнение.
5. Прочитайте man mount, fsck, mkfs, kill и кратко их охарактеризуйте, приведя примеры.

# Теоретическое введение

Файловые системы в Linux используются не только для работы с файлами на диске, но и для хранения данных в оперативной памяти или доступа к конфигурации ядра во время работы системы. Все они включены в ядро и могут использоваться в качестве корневой файловой системы.

# Выполнение лабораторной работы

1. Выполняю все примеры, приведенные в первой части описания лабораторной работы. (рис. [-@fig:001])

![рис. 1](img/1.png){#fig:001 width = 70%)

2. Выполняю следующие действия (рис. [-@fig:002]):

![рис. 2](img/2.png){#fig:002 width = 70%)

	2.1. Копирую файл /usr/include/sys/io.h в домашний каталог и называю его
	equipment.
	2.2. В домашнем каталоге создаю директорию ~/ski.plases.
	2.3. Перемещаю файл equipment в каталог ~/ski.plases.
	2.4. Переименовываю файл ~/ski.plases/equipment в ~/ski.plases/equiplist.
	2.5. Создаю в домашнем каталоге файл abc1 и копирую его в каталог
	~/ski.plases,называю его equiplist2.
	2.6. Создаю каталог с именем equipment в каталоге ~/ski.plases.
	2.7. Перемещаю файлы ~/ski.plases/equiplist и equiplist2 в каталог
	~/ski.plases/equipment.
	2.8. Создаю и перемещаю каталог ~/newdir в каталог ~/ski.plases и называю
	его plans.
	
3. Определяю опции команды chmod,необходимые для того,чтобы присвоить перечис-
ленным ниже файлам выделенные права доступа. (рис. [-@fig:003])

![рис. 3](img/3.png){#fig:003 width = 70%)

4. Проделываю приведённые ниже упражнения (рис. [-@fig:004]):

![рис. 4](img/4.png){#fig:004 width = 70%)

	4.1. Просматриваю содержимое файла /etc/password.
	4.2. Копирую файл ~/feathers в файл ~/file.old.
	4.3. Перемещаю файл ~/file.old в каталог ~/play.
	4.4. Копирую каталог ~/play в каталог ~/fun.
	4.5. Перемещаю каталог ~/fun в каталог ~/play и называю его games.
	4.6. Лишаю владельца файла ~/feathers права на чтение.
	4.7. При поптыке просмотра файла ~/feathers получаю ошибку, так как владелец файла лишен права на 		чтение.
	4.8. При попытке скопировать файл ~/feathers получаю ошибку по вышеуказанной причине.
	4.9. Даю владельцу файла ~/feathers право на чтение.
	4.10. Лишаю владельца каталога ~/play права на выполнение.
	4.11. При попытке перейти в каталог ~/play получаю ошибку, так как владелец файла лишен права на 		чтение.
	4.12. Даю владельцу каталога ~/play право на выполнение.

5. Читаю man mount (рис. [-@fig:005]), fsck (рис. [-@fig:006]), mkfs (рис. [-@fig:007]), kill (рис. [-@fig:008]). 

![рис. 5](img/5.png){#fig:005 width = 70%)


![рис. 6](img/6.png){#fig:006 width = 70%)


![рис. 7](img/7.png){#fig:007 width = 70%)


![рис. 8](img/8.png){#fig:008 width = 70%)



# Выводы

Выполняя данную лабораторную работу я ознакомилась с файловой системой Linux и научилась с ней взаимодействовать.

# Список литературы{.unnumbered}

::: {#refs}
:::
