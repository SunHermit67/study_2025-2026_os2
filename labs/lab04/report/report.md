---
## Front matter
title: "Отчёт о лабораторной работе"
subtitle: "Лабораторная работа №4"
author: "Приходько Иван Иванович"

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
mainfont: IBM Plex Serif
romanfont: IBM Plex Serif
sansfont: IBM Plex Sans
monofont: IBM Plex Mono
mathfont: STIX Two Math
mainfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
romanfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
sansfontoptions: Ligatures=Common,Ligatures=TeX,Scale=MatchLowercase,Scale=0.94
monofontoptions: Scale=MatchLowercase,Scale=0.94,FakeStretch=0.9
mathfontoptions:
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

Получить навыки работы с репозиториями и менеджерами пакетов.

# Задание

Поработать с менеджером пакетов и репозиториями 

# Выполнение лабораторной работы

Для начала откроем любой репозиторий с .repo (рис. [3.1]-[3.2]).

![Файлы с .repo](image/401.PNG){#fig:001 width=70%}

![Файл .repo внутри](image/402.PNG){#fig:002 width=70%}

Далее выводим список всех пакетов в которых есть слово user и заодно ищем nmap (рис. [3.3]).

![Все файлы с в которых есть слово user и поиск nmap](image/403.PNG){#fig:003 width=70%}

Теперь получим список всех умеющихся групп пакетов (рис. [3.4]-[3.5]).

![Список группа пакетов](image/404.PNG){#fig:004 width=70%}

![Список группа пакетов на англ](image/405.PNG){#fig:005 width=70%}

Теперь установим группу пакетов RPM Development Tools (рис. [3.6]).

![Установка RPM Development Tools](image/406.PNG){#fig:006 width=70%}

Теперь выведем всю информацию о взаимодействии с dnf пакетами и попробуем отменить некоторые действия (рис. [3.7]).

![История взаимодействия с dnf пакетами](image/407.PNG){#fig:007 width=70%}

Теперь установим lynx и определим некоторую информацию о нем (рис. [3.8]-[3.9]).

![Установка и работа с lynx](image/408.PNG){#fig:008 width=70%}

![Установка и работа с lynx](image/409.PNG){#fig:009 width=70%}

Выведем список всех файлов (рис. [3.10]).

![Список всех файлов lynx](image/410.PNG){#fig:010 width=70%}

Теперь выведем информацию об определенных файлах (рис. [3.11]).

![Список определенных файлов lynx](image/411.PNG){#fig:011 width=70%}

Далее установим dnsmasq (рис. [3.12]).

![Установка dnsmasq](image/412.PNG){#fig:012 width=70%}

Выведем перечень всех файлов dnsmasq (рис. [3.13]).

![Список всех файлов dnsmasq](image/413.PNG){#fig:013 width=70%}

Теперь выведем информацию об определенных файлах (рис. [3.14]).

![Список определенных файлов dnsmasq](image/414.PNG){#fig:014 width=70%}

# Выводы

В ходе данной лабораторной работы были получены знания для работы с менеджером пакетов

# Ответы на контрольные вопросы

1. rpm -qf /usr/sbin/useradd

2. getent group dnf  
groups dnf

3. dnf install <имя_пакета> или yum install <имя_пакета>

4. rpm -K <файл.rpm> или rpm -qp --scripts <файл.rpm> 

5. rpm -qd или rpm -q --info

6. rpm -qf <файл>
