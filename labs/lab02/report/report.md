---
## Front matter
title: "Отчёт о лабораторной работе"
subtitle: "Лабораторная работа №2"
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

Получить представление о работе с учётными записями пользователей и группами пользователей в операционной системе типа Linux.

# Задание

Поработать с учетными записями

# Выполнение лабораторной работы

Для начала узнаем всю информацию об основной учетной записи и root (рис. [3.1]).

![Информация об основной учетной записи и root](image/201.PNG){#fig:001 width=70%}

Далее изменим параметр в etc/sudoers при помощи visido (используем его по причине удобства и безопасности) (рис. [3.2] - [3.3]).

![Изменение параметра в etc/sudoers](image/202.PNG){#fig:002 width=70%}

![Изменение параметра в etc/sudoers](image/203.PNG){#fig:003 width=70%}

Теперь начнем работать с учетными записями. Для начала создаем Алису, видим что у неё другой id, ставим для неё пароль и тоже самое для Боба (рис. [3.4]).

![Работа с учетными записями](image/204.PNG){#fig:004 width=70%}

Далее изменим пару параметров в etc/login.defs (рис. [3.5]).

![Изменение параметров в etc/login.defs](image/205.PNG){#fig:005 width=70%}

Теперь создадим третью учетную запись Кэрол (рис. [3.6]).

![Создание третьей учетной записи](image/206.PNG){#fig:006 width=70%}

И напоследок поработаем с параметрами со сроком действия и группами (рис. [3.7]).

![Работа с гуппами и параметрами со сроком действия](image/207.PNG){#fig:007 width=70%}

# Выводы

В ходе данной лабораторной работы были получены знания для работы с учетными записями в линукс

# Ответы на контрольные вопросы

1. Команды для получения информации об идентификаторе и группах пользователя:  
id (например, `id alice`)  

2. UID пользователя root: 0.  
Команда для узнать UID: id -u или id alice.  

3. su — переключение пользователя, требует пароль.  
sudo — выполнение команды с правами другого пользователя (обычно администратора), требует пароль.  

4. Параметры sudo определяются в файле /etc/sudoers.  

5. Для безопасного изменения конфигурации sudo: использовать команду visudo.  

6. Пользователь должен быть членом группы sudo или wheel (зависит от дистрибутива).  

7. Файлы/каталоги: /etc/passwd (для параметров учётных записей), /etc/shadow (секреты паролей).  
Примеры настроек: shell по умолчанию, домашний каталог.  

8. Информация о группах хранится в /etc/group.  
Для пользователя alice: строка вида alice:x:1001 (группа основная).  

9. Команды: chage, passwd --status, passwd --expire.  

10. Используйте команду vipw или vigr — для безопасного редактирования /etc/passwd и /etc/group. Они обеспечивают предотвращение повреждения файлов и проверку синтаксиса.
