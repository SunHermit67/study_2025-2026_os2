---
## Front matter
title: "Отчёт о лабораторной работе"
subtitle: "Лабораторная работа №5"
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

Получить навыки управления системными службами операционной системы посредством systemd.

# Задание

Научится управлять системными службами операционной системы посредством systemd

# Выполнение лабораторной работы

Для начаал установим systemd (рис. [3.1]).

![Установка systemd](image/501.PNG){#fig:001 width=70%}

Далее активируем systemd и перезагруем машину (рис. [3.2]).

![Активация systemd](image/502.PNG){#fig:002 width=70%}

Далее добавим службу Very Secure FTP в автозапуск и сразу же удалим оттуда (рис. [3.3]).

![Добавление службы Very Secure FTP в автозапуск](image/503.PNG){#fig:003 width=70%}

Теперь установим iptables (рис. [3.4]).

![Установка iptables](image/504.PNG){#fig:004 width=70%}

Он конфликтует с firewall, поэтому отключим его, далее попробуем замаскировать сеть и провзаимодействоввать с ней (рис. [3.5]).

![Маскировка сетей](image/505.PNG){#fig:005 width=70%}

Отключим iptables и включим firewall, а потом выведем список всех сетей которые можно изолировать (рис. [3.6]).

![Список сетей которые можно изолировать](image/506.PNG){#fig:006 width=70%}

Теперь поработаем с целями (рис. [3.7]).

![Работа с целями](image/507.PNG){#fig:007 width=70%}

После этого система запустилась в текстовом режиме, попробуем вернуть снова в графический (рис. [3.8]).

![Вовзращение в графический режим](image/508.PNG){#fig:008 width=70%}

# Выводы

В ходе данной лабораторной работы были получены знания для управления системными службами операционной системы посредством systemd.

# Ответы на контрольные вопросы

1. Юнит — единица systemd (сервис, таймер). Примеры: nginx.service, backup.timer.  

2. systemctl disable <цель> или systemctl is-enabled <цель>.  

3. systemctl list-units --type=service.  

4. systemctl add-wants <unit> <target>.  

5. systemctl rescue.  

6. Цель не может быть изолирована из-за зависимостей или активных юнитов.  

7. systemctl list-dependencies <служба>.
