---
## Front matter
title: "Отчёт о лабораторной работе"
subtitle: "Лабораторная работа №7"
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

Получить навыки работы с журналами мониторинга различных событий в системе.

# Задание

Поработать с журналом мониторинга событий в системе

# Выполнение лабораторной работы

Для начала запустим жирнал событий в другом терминале и попробуем вывести пару сообщений (рис. [3.1]).

![Вывод сообщений в журнале действий](image/701.PNG){#fig:001 width=70%}

Изменим файл httpd.conf (рис. [3.2]).

![Изменение файла httpd.conf](image/702.PNG){#fig:002 width=70%}

Выведем еще пару сообщений в терминале (рис. [3.3]).

![Вывод сообщений через файл](image/703.PNG){#fig:003 width=70%}

Теперь выведем сообщение через другой способ (рис. [3.4]).

![Вывод сообщений черезиной способ](image/704.PNG){#fig:004 width=70%}

Теперь откроем содержимое терминала (рис. [3.5]-[3.7]).

![Открытие сордержимого терминала](image/705.PNG){#fig:005 width=70%}

![Открытие сордержимого терминала](image/706.PNG){#fig:006 width=70%}

![Открытие сордержимого терминала](image/707.PNG){#fig:007 width=70%}

Теперь создадим и настроим каталог для записи журнала (рис. [3.8]).

![Сорздание инастройка каталога для записи журнала](image/708.PNG){#fig:008 width=70%}

# Выводы

В ходе данной лабораторной работы были получены навыки работы с журналами мониторинга различных событий в системе.

# Ответы на контрольные вопросы

1. /etc/rsyslog.conf или /etc/rsyslog.d/  

2. /etc/rsyslog.conf или файлы в /etc/rsyslog.d/, связанные с auth или authpriv  

3. Зависит от настроек, обычно — несколько секунд или минут, сразу после триггера ротации.  

4. *.info /var/log/messages.info  

5. tail -f /var/log/messages или journalctl -f  

6. journalctl _PID=1 --since "09:00" --until "15:00"  

7. journalctl --boot или journalctl -b  

8. Использовать systemctl restart systemd-journald после настройки /etc/systemd/journald.conf.
