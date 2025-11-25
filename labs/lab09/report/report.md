---
## Front matter
title: "Отчёт о лабораторной работе"
subtitle: "Лабораторная работа №9"
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

Получить навыки работы с контекстом безопасности и политиками SELinux.

# Задание

Поработать с контекстом безопасности и политиками SELinux.

# Выполнение лабораторной работы

Для начала посмотрим статус SELinux (рис. [3.1]).

![Статус SELinux](image/901.PNG){#fig:001 width=70%}

Теперь в файле отключим SELinux (рис. [3.2]-[3.3]).

![ОТключение SELinux](image/903.PNG){#fig:002 width=70%}

![Отключение SELinux](image/902.PNG){#fig:003 width=70%}

Теперь вернем SELinux в enforcing (рис. [3.4]).

![Включение SELinux](image/904.PNG){#fig:004 width=70%}

После перезапусками системы SELinux снова включен (рис. [3.5]).

![Перезапуск системы](image/905.PNG){#fig:005 width=70%}

Теперь поработаем с контекстом безопасности файла (рис. [3.6]).

![Работа с контекстом безопасности файла](image/906.PNG){#fig:006 width=70%}

Далее добавим пару строк в httpd.conf (рис. [3.7]-[3.8]).

![Изменение httpd.conf](image/907.PNG){#fig:007 width=70%}

![Изменение httpd.conf](image/908.PNG){#fig:008 width=70%}

Теперь запустим httpd (рис. [3.9]).

![Запуск httpd](image/909.PNG){#fig:009 width=70%}

Поработаем немного с httpd и выведем список переключатей SELinux (рис. [3.10]).

![Работа с httpd и список переключатей SELinux](image/910.PNG){#fig:010 width=70%}

Теперь поработаем с переключателями SELinux (рис. [3.11]).

![Работа с переключателями SELinux](image/911.PNG){#fig:011 width=70%}

# Выводы

В ходе данной работы были получены навыки для работы с контекстом безопасности и политиками SELinux.

# Ответы на контрольные вопросы

1. setenforce 1  

2. sestatus -v или semanage boolean -l  

3. setroubleshoot (или sealert`) — пакет называется `setroubleshoot  

4. chcon -t httpd_sys_content_t /web и restorecon -Rv /web  

5. Изменить или удалить файл /etc/selinux/config  

6. /var/log/audit/audit.log  

7. seinfo -t ftp или semanage fcontext -l  

8. Проверить журнал /var/log/audit/audit.log или использовать sealert для диагностики
