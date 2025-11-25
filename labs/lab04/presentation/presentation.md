---
## Front matter
lang: ru-RU
title: Лабораторная работа
subtitle: Номер 4
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

Получить навыки работы с репозиториями и менеджерами пакетов.

## Задание

Поработать с менеджером пакетов и репозиториями 

## Работа с пакетами

Для начала откроем любой репозиторий с .repo 

![Файлы с .repo](image/401.PNG)

## Работа с пакетами

![Файл .repo внутри](image/402.PNG)

## Работа с пакетами

Далее выводим список всех пакетов в которых есть слово user и заодно ищем nmap

![Все файлы с в которых есть слово user и поиск nmap](image/403.PNG)

## Работа с пакетами

Теперь получим список всех умеющихся групп пакетов

![Список группа пакетов](image/404.PNG)

## Работа с пакетами

![Список группа пакетов на англ](image/405.PNG)

## Работа с пакетами

Теперь установим группу пакетов RPM Development Tools

![Установка RPM Development Tools](image/406.PNG)

## Работа с пакетами

Теперь выведем всю информацию о взаимодействии с dnf пакетами и попробуем отменить некоторые действия 

![История взаимодействия с dnf пакетами](image/407.PNG)

## Работа с пакетами

Теперь установим lynx и определим некоторую информацию о нем 

![Установка и работа с lynx](image/408.PNG)

## Работа с пакетами

![Установка и работа с lynx](image/409.PNG)

## Работа с пакетами

Выведем список всех файлов

![Список всех файлов lynx](image/410.PNG)

## Работа с пакетами

Теперь выведем информацию об определенных файлах 

![Список определенных файлов lynx](image/411.PNG)

## Работа с пакетами

Далее установим dnsmasq 

![Установка dnsmasq](image/412.PNG)

## Работа с пакетами

Выведем перечень всех файлов dnsmasq 

![Список всех файлов dnsmasq](image/413.PNG)

## Работа с пакетами

Теперь выведем информацию об определенных файлах 

![Список определенных файлов dnsmasq](image/414.PNG)

## Выводы

В ходе данной лабораторной работы были получены знания для работы с менеджером пакетов

