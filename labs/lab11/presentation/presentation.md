---
## Front matter
lang: ru-RU
title: Лабораторная работа
subtitle: Номер 11
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

Получить навыки работы с загрузчиком системы GRUB2.

## Задание

Поработать с загрузчиком системы GRUB2.

## Работа с GRUB2

Для начала увеличим время перед тем как запускается системы, чтобы можно было успеть перейти в GRUB2

![Увеличение интервала GRUB2](image/1101.PNG)

## Работа с GRUB2

Запишем изменения в файле и перезапустим систем

![Запись изменений](image/1102.PNG)

## Работа с GRUB2

После перезапуска быстро жмем Esc и переходим в GRUB2

![Переход в GRUB2](image/1103.PNG)

## Работа с GRUB2

Теперь в GRUB2 сбрасываем пароль root

![Сброс пароля root](image/1104.PNG)

## Выводы

В ходе данной лабораторной работы были получены навыки для работы с загрузчиком системы GRUB2.

