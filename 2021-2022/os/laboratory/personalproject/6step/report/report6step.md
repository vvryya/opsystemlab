---
## Front matter
title: "Отчет"
subtitle: "6 этап"
author: "Павлова Варвара Юрьевна НПМбд-02-21"

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

Создание академического сайта.

# Задание

Разместить двуязычный сайт на Github.
- Сделать поддержку английского и русского языков.
- Разместить элементы сайта на обоих языках.
- Разместить контент на обоих языках.
- Сделать пост по прошедшей неделе.
- Добавить пост на тему по выбору (на двух языках).

# Выполнение 6 этапа

1. Вызываю ~/bin/hugo server и перехожу на сайт.(рис. [-@fig:001])

![вызов hugo server](img/1.png){ #fig:001 width=70% }

2. Добавляю английский язык на сайт. (рис. [-@fig:002]) 

![добавление языка](img/2.png){ #fig:002 width=70% }

3. Пишу пост на тему котов сфинксов. (рис. [-@fig:003])

![пост на тему по выбору](img/3.png){ #fig:003 width=70% }

4. Пишу пост о прошедшей неделе. (рис. [-@fig:004])

![пост о 6 неделе](img/4.png){ #fig:004 width=70% }

5. Вызываю в терминале ~/bin/hugo.(рис. [-@fig:005])

![вызов hugo](img/5.png){ #fig:005 width=70% }

7. Перехожу в подкаталог public и выполняю команды *git add .*, *git commit* и *git push*.(рис. [-@fig:006])

![команды с git в public](img/6.png){ #fig:007 width=70% }

8. Перехожу в каталог blog и выполняю команды *git add .*, *git commit* и *git push*.(рис. [-@fig:007])

![команды с git в blog](img/7.png){ #fig:007 width=70% }

9. Захожу на сайт и проверяю изменения.(рис. [-@fig:008])(рис. [-@fig:009])

![добавлен английский](img/8.png){ #fig:008 width=70% }


![новые посты](img/9.png){ #fig:009 width=70% }

# Выводы

Выполняя данный этап я научилась публиковать данные на сайте.


