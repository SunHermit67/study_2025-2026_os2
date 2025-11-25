---
## Front matter
lang: ru-RU
title: Лабораторная работа
subtitle: Номер 7
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

Получить навыки работы с журналами мониторинга различных событий в системе.

## Задание

Поработать с журналом мониторинга событий в системе

## Работа с журналом действий

Для начала запустим жирнал событий в другом терминале и попробуем вывести пару сообщений 

![Вывод сообщений в журнале действий](image/701.PNG)

## Работа с журналом действий

Изменим файл httpd.conf

![Изменение файла httpd.conf](image/702.PNG)

## Работа с журналом действий

Выведем еще пару сообщений в терминале 

![Вывод сообщений через файл](image/703.PNG)

## Работа с журналом действий

Теперь выведем сообщение через другой способ 

![Вывод сообщений черезиной способ](image/704.PNG)

## Работа с журналом действий

Теперь откроем содержимое терминала

![Открытие сордержимого терминала](image/705.PNG)

## Работа с журналом действий

![Открытие сордержимого терминала](image/706.PNG)

## Работа с журналом действий

![Открытие сордержимого терминала](image/707.PNG)

## Работа с журналом действий

Теперь создадим и настроим каталог для записи журнала

![Сорздание инастройка каталога для записи журнала](image/708.PNG)

## Выводы

В ходе данной лабораторной работы были получены навыки работы с журналами мониторинга различных событий в системе.
