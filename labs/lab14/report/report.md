---
## Front matter
title: "Отчёт о лабораторной работе"
subtitle: "Лабораторная работа №14"
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

Получить навыки создания разделов на диске и файловых систем. Получить навыки монтирования файловых систем.

# Задание

Научиться создавать разделы на диске и файловые системы, монтировать файловые системы.

# Выполнение лабораторной работы

Для начала переходим в меню для добавления жестких дисков (рис. [-@fig:001]).

![Меню для жестких дисков](image/01.PNG){#fig:001 width=70%}

Нажимаем добавить и затем выбираем тип файла VDI (рис. [-@fig:002]).

![Тип файла жесткого диска](image/02.PNG){#fig:002 width=70%}

Указываем имя и размер диска (рис. [-@fig:003]).

![Имя и размер диска](image/03.PNG){#fig:003 width=70%}

Далее создаем второй такой же диск (рис. [-@fig:004]).

![Создание второго диска](image/04.PNG){#fig:004 width=70%}

Внутри виртуальной машины видим, что диски успешно добавлены (рис. [-@fig:005]).

![Проверка наличия виртуальных дисков](image/05.PNG){#fig:005 width=70%}

Далее создаем разметку для диска 1 (рис. [-@fig:006]).

![Создание разметки для диска 1](image/06.PNG){#fig:006 width=70%}

Проверям и видим, что все успешно создано (рис. [-@fig:007]).

![Проверка разметки для диска 1](image/07.PNG){#fig:007 width=70%}

Далее создаем логический раздел для диска 2 (рис. [-@fig:008]).

![Создание логиского раздела для диска 2](image/08.PNG){#fig:008 width=70%}

Проверяем наличие логического раздела (рис. [-@fig:009]).

![Проверка наличия логического раздела](image/09.PNG){#fig:009 width=70%}

Далее создаем раздел для подкачки (рис. [-@fig:010]).

![Создание раздела для подкачки](image/10.PNG){#fig:010 width=70%}

Проверяем наличие разделя для подкачки (рис. [-@fig:011]).

![Проверка наличия раздела для подкачки](image/11.PNG){#fig:011 width=70%}

Потом форматируем диск для подкачки и проверяем наличие места (рис. [-@fig:012]).

![Форматирование диска для подкачки](image/12.PNG){#fig:012 width=70%}

Далее создаем раздел GPT с помощью gdisk (рис. [-@fig:013]).

![Создание раздела GPT](image/13.PNG){#fig:013 width=70%}

Затем форматируем файловую систему XFS и EXT4 (рис. [-@fig:014]).

![Форматирование файловой системы XFS и EXT4](image/14.PNG){#fig:014 width=70%}

А теперь вручную примонтурем созданные разделы, после команды выведем все файловые системы (рис. [-@fig:015]).

![Вывод всех файловые систем](image/15.PNG){#fig:015 width=70%}

После команды раздел успешно отмонтирован (рис. [-@fig:016]).

![Проверка того, что диск отмонтирован](image/16.PNG){#fig:016 width=70%}

Теперь создаем папку для монтирования раздела и выводим айди нужного раздела (рис. [-@fig:017]).

![Создание папки](image/17.PNG){#fig:017 width=70%}

Далее изменим файл и впишем туда данные куда монтировать и какой раздел по айди (рис. [-@fig:018]).

![Внесение данных](image/18.PNG){#fig:018 width=70%}

Монтируем и проверяем (рис. [-@fig:019]).

![Монтировка и проверка](image/19.PNG){#fig:019 width=70%}

# Выводы

В ходе данной лабораторной работы были полученны навыки для создания разделов на диске и файловых систем и монтирования файловых систем.

# Ответы на контрольные вопросы

1. gdisk или parted
2. используется fdisk
3. файл /etc/fstab
4. в /etc/fstab опция noauto
5. mkswap /dev/имя_раздела
6. mount -a
7. создаётся файловая система ext2
8. mkfs.ext4 /dev/имя_раздела
9. blkid
