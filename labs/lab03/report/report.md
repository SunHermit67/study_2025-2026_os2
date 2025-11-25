---
## Front matter
title: "Отчёт о лабораторной работе"
subtitle: "Лабораторная работа №3"
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

Получение навыков настройки базовых и специальных прав доступа для групп пользователей в операционной системе типа Linux.

# Задание

Получить базовые навыми для работы с правами доступа для пользователей

# Выполнение лабораторной работы

Для начала создадим две папке, чтобы одна группа пользователей могла пользоваться только первой, а другоая группа только второй (рис. [3.1]).

![Создание папок](image/301.PNG){#fig:001 width=70%}

Теперь создадим несколько файлов от имени разных пользователей (рис. [3.2]).

![Создание файлов от имени разных пользователей](image/302.PNG){#fig:002 width=70%}

Теперь посмотрим на свойства этих файлов и попробуем провзаимодействовать с ними (рис. [3.3] - [3.4]).

![Работа с файлами](image/303.PNG){#fig:003 width=70%}

![Свойства файлов](image/304.PNG){#fig:004 width=70%}

И под конец поработаем с двумя ранее создаными файлами, которые были внутри папок, которым мы выдали определенные свойста, из-за чего с один из файлов мы не смогли провзаимодействовать (рис. [3.5]).

![Последняя работа с файлами](image/305.PNG){#fig:005 width=70%}

# Выводы

В ходе данной лабораторной работы были получены знания для работы с правами доступа для разных пользователей.

# Ответы на контрольные вопросы

1. chown <пользователь>:<группа> <файл>  

2. find / -user <имя_пользователя>  

3. chmod 770 /data  

4. chmod +x <файл>  

5. chmod g+s <каталог> или chmod o-g <каталог> 

6. Использовать umask, чтобы ограничить права при создании файлов. umask 027 — владельцы и группа получат rwxr-x--- права.  

7. setfacl -m g:<группа>:r-- <файл или каталог> Чтобы установить для всех файлов в каталоге: setfacl -R -m g:<группа>:r-- .  

8. chmod g+s <каталог>  

9. umask 077 — новые файлы имеют права 600 (для файлов) или 700 (для каталогов).
