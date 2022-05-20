---
## Front matter
title: "Отчет"
subtitle: "4 этап"
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

1. Зарегистрироваться на соответствующих ресурсах и разместить на них ссылки на сайте:

   - eLibrary : https://elibrary.ru/;
   - Google Scholar : https://scholar.google.com/;
   - ORCID : https://orcid.org/;
   - Mendeley : https://www.mendeley.com/;
   - ResearchGate : https://www.researchgate.net/;
   - Academia.edu : https://www.academia.edu/;
   - arXiv : https://arxiv.org/;
   - github : https://github.com/.

2. Сделать пост по прошедшей неделе.
3. Добавить пост на тему по выбору:

   - Оформление отчёта.
   - Создание презентаций.
   - Работа с библиографией.

# Выполнение 3 этапа

1. Вызываю ~/bin/hugo server и перехожу на сайт.(рис. [-@fig:001])

![вызов hugo server](img/1.png){ #fig:001 width=70% }

2. Регистрируюсь на указанный в задании ресурсах и оставляю на них ссылку на сайте. (рис. [-@fig:002]) 

![указание ссылок](img/2.png){ #fig:002 width=70% }

3. Пишу пост на тему оформления отчета. (рис. [-@fig:003])

![пост на тему по выбору](img/3.png){ #fig:003 width=70% }

4. Пишу пост о прошедшей неделе. (рис. [-@fig:004])

![пост о 4 неделе](img/4.png){ #fig:004 width=70% }

5. Вызываю в терминале ~/bin/hugo.(рис. [-@fig:005])

![вызов hugo](img/5.png){ #fig:005 width=70% }

7. Перехожу в подкаталог public и выполняю команды *git add .*, *git commit* и *git push*.(рис. [-@fig:006])

![команды с git в public](img/6.png){ #fig:007 width=70% }

8. Перехожу в каталог blog и выполняю команды *git add .*, *git commit* и *git push*.(рис. [-@fig:007])

![команды с git в blog](img/7.png){ #fig:007 width=70% }

9. Захожу на сайт и проверяю изменения.(рис. [-@fig:008])(рис. [-@fig:009])

![ссылки на ресурсы](img/8.png){ #fig:008 width=70% }


![новые посты](img/9.png){ #fig:009 width=70% }

# Выводы

Выполняя данный этап я научилась публиковать данные на сайте.


