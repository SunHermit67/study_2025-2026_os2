---
## Front matter
title: "Отчёт о лабораторной работе"
subtitle: "Лабораторная работа №6"
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

Получить навыки управления процессами операционной системы.

# Задание

Научится работать с процессами операционной системы.

# Выполнение лабораторной работы

Для начала запустим пару процессов и поработаем с их id (рис. [3.1]).

![Работа с процессами](image/601.PNG){#fig:001 width=70%}

Выведем список всех процессов (рис. [3.2]).

![Список всех процессов](image/602.PNG){#fig:002 width=70%}

Запустим еще несколько процессов и посмотрим их подробную информацию (рис. [3.3]).

![Подробная информация о процессах](image/603.PNG){#fig:003 width=70%}

Попробуем поменять приоритеты (рис. [3.4]).

![Изменение приоритетов](image/604.PNG){#fig:004 width=70%}

Выведем дерево всех процессов (рис. [3.5]).

![Дерево процессов](image/606.PNG){#fig:005 width=70%}

Теперь поставим приоритеты -5 и -15 для разных задач (рис. [3.6]).

![Приоритеты](image/607.PNG){#fig:006 width=70%}

Остановим все процессы что запустили (рис. [3.7]).

![Остановка процессов](image/610.PNG){#fig:007 width=70%}

# Выводы

В ходе данной лабораторной работы были получены знания для работы с процессами

# Ответы на контрольные вопросы

1. jobs  

2. kill %<номер задания>  

3. Ctrl + Z  

4. Использовать kill по PID, если есть доступ к нему, или через системные средства удалённого управления.  

5. pstree  

6. renice -n -<приоритет> -p 1234  

7. pkill dd или killall dd  

8. pkill mycommand или killall mycommand  

9. В top — нажать k, ввести PID, затем указать приоритет.  

10. nice -n <значение> <команда> с высоким приоритетом (например, `nice -n -10 команда`).
