---
## Front matter
lang: ru-RU
title: Лабораторная работа
subtitle: Номер 3
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

Получение навыков настройки базовых и специальных прав доступа для групп пользователей в операционной системе типа Linux.

## Задание

Получить базовые навыми для работы с правами доступа для пользователей

## Работа с правами доступа

Для начала создадим две папке, чтобы одна группа пользователей могла пользоваться только первой, а другоая группа только второй

![Создание папок](image/301.PNG)

## Работа с правами доступа

Теперь создадим несколько файлов от имени разных пользователей 

![Создание файлов от имени разных пользователей](image/302.PNG)

## Работа с правами доступа

Теперь посмотрим на свойства этих файлов и попробуем провзаимодействовать с ними

![Работа с файлами](image/303.PNG)

## Работа с правами доступа

![Свойства файлов](image/304.PNG)

## Работа с правами доступа

И под конец поработаем с двумя ранее создаными файлами, которые были внутри папок, которым мы выдали определенные свойста, из-за чего с один из файлов мы не смогли провзаимодействовать

![Последняя работа с файлами](image/305.PNG)

## Выводы

В ходе данной лабораторной работы были получены знания для работы с правами доступа для разных пользователей.