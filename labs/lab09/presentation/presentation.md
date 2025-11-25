---
## Front matter
lang: ru-RU
title: Лабораторная работа
subtitle: Номер 9
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

Получить навыки работы с контекстом безопасности и политиками SELinux.

## Задание

Поработать с контекстом безопасности и политиками SELinux.

## Работа с SELinux

Для начала посмотрим статус SELinux

![Статус SELinux](image/901.PNG)

## Работа с SELinux

Теперь в файле отключим SELinux

![ОТключение SELinux](image/903.PNG)

## Работа с SELinux

![Отключение SELinux](image/902.PNG)

## Работа с SELinux

Теперь вернем SELinux в enforcing

![Включение SELinux](image/904.PNG)

## Работа с SELinux

После перезапусками системы SELinux снова включен

![Перезапуск системы](image/905.PNG)

## Работа с SELinux

Теперь поработаем с контекстом безопасности файла

![Работа с контекстом безопасности файла](image/906.PNG)

## Работа с SELinux

Далее добавим пару строк в httpd.conf

![Изменение httpd.conf](image/907.PNG)

## Работа с SELinux

![Изменение httpd.conf](image/908.PNG)

## Работа с SELinux

Теперь запустим httpd

![Запуск httpd](image/909.PNG)

## Работа с SELinux

Поработаем немного с httpd и выведем список переключатей SELinux

![Работа с httpd и список переключатей SELinux](image/910.PNG)

## Работа с SELinux

Теперь поработаем с переключателями SELinux 

![Работа с переключателями SELinux](image/911.PNG)

## Выводы

В ходе данной работы были получены навыки для работы с контекстом безопасности и политиками SELinux.
