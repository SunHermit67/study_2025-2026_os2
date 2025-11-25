---
## Front matter
lang: ru-RU
title: Лабораторная работа
subtitle: Номер 13
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

Получить навыки настройки пакетного фильтра в Linux.

## Задание

Поработать с пакетным фильтром в Linux.

## Работа со службами

Для начала посмотрим все доступные службы в текущей зоне

![Все доступные службы в текущей зоне](image/1301.PNG)

## Работа со службами

Выведем немного подругому доступные службы

![Все доступные службы в текущей зоне](image/1302.PNG)

## Работа со VNC

Добавим VNC в конфигурацию брэндмауэр и проверим добавился ли он

![Добавление VNC в конфигурацию брэндмауэр](image/1303.PNG)

## Работа со VNC

Только после перезагрузки он появился

![Проверка VNC](image/1304.PNG)

## Работа со VNC

Проверим добавился ли VNC после перманентного добавления

![Проверка VNC на перманентрое добавление](image/1305.PNG)

## Работа с firewall

Теперь попробуем запустить графическое меню firewall

![Запуск графическиго меню firewall](image/1306.PNG)

## Работа с firewall

Через графичесике меню добавляем серивисы, что просят в задании

![Добавление сервисов](image/1307.PNG)

## Работа с firewall

Проверим добавились ли они

![Проверка сервисов](image/1308.PNG)

## Работа с firewall

После перезагрузки компьютера проверим, были добавлены изменения после самостоятельной работы

![Проверка сервисов после самостоятельной работы](image/1309.PNG)

## Выводы

В ходе данной лабораторной работы были получены навыки для настройки пакетного фильтра в Linux.


