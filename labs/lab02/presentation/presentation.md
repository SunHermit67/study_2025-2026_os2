---
## Front matter
lang: ru-RU
title: Лабораторная работа
subtitle: Номер 2
author:
  - Приходько Иван Иванович
institute:
  - Российский университет дружбы народов, Москва, Россия
date: 27 ноября 2025

## i18n babel
babel-lang: russian
babel-otherlangs: english

## Formatting pdf
toc: false
toc-title: Содержание
slide_level: 2
aspectratio: 169
section-titles: true
theme: metropolis
header-includes:
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
 
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
---

# Информация

## Докладчик

:::::::::::::: {.columns align=center}
::: {.column width="70%"}

  * Приходько Иван Иванович
  * Студент
  * Российский университет дружбы народов

:::
::: {.column width="30%"}


:::
::::::::::::::


## Цель работы

Получить представление о работе с учётными записями пользователей и группами пользователей в операционной системе типа Linux.

## Задание

Поработать с учетными записями

## Работа с учетными записями

Для начала узнаем всю информацию об основной учетной записи и root

![Информация об основной учетной записи и root](image/201.PNG)

## Работа с учетными записями

Далее изменим параметр в etc/sudoers при помощи visido (используем его по причине удобства и безопасности)

![Изменение параметра в etc/sudoers](image/202.PNG)

## Работа с учетными записями

![Изменение параметра в etc/sudoers](image/203.PNG)

## Работа с учетными записями

Теперь начнем работать с учетными записями. Для начала создаем Алису, видим что у неё другой id, ставим для неё пароль и тоже самое для Боба 

![Работа с учетными записями](image/204.PNG)

## Работа с учетными записями

Далее изменим пару параметров в etc/login.defs 

![Изменение параметров в etc/login.defs](image/205.PNG)

## Работа с учетными записями

Теперь создадим третью учетную запись Кэрол 

![Создание третьей учетной записи](image/206.PNG)

## Работа с учетными записями

И напоследок поработаем с параметрами со сроком действия и группами 

![Работа с гуппами и параметрами со сроком действия](image/207.PNG)

## Выводы

В ходе данной лабораторной работы были получены знания для работы с учетными записями в линукс

