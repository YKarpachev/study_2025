---
## Front matter
lang: ru-RU
title: Структура научной презентации
subtitle: Простейший шаблон
author:
  - Карпачев Я. О.
institute:
  - Российский университет дружбы народов, Москва, Россия

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
 - '\makeatletter'
 - '\beamer@ignorenonframefalse'
 - '\makeatother'
---

# Информация

## Докладчик

:::::::::::::: {.columns align=center}
::: {.column width="70%"}

  * Карпачев Я. О.
  * студент
  * Российский университет дружбы народов

:::
::: {.column width="30%"}

:::
::::::::::::::

# Вводная часть

## Цель работы

Найти уязвимости с помощью nikto

## Задачи

0. приготовить mysql, apache2
1. найти точку входа на DVWA (айпи адрес + порт или полный URL)
2. запустить провеку на уровне защиты low
3. запустить проверку на уровне защиты imposible

## Запускаем две команды одна для mysql, другая для apache2

![Запуск команд](image/1.png){#fig:001 width=70%}

## Запускаем проверку на уровне защиты low, full url path

![Запуск команды на уровне защиты low](image/2.png){#fig:002 width=70%}

## Запускаем проверку на уровне защиты imposible, ip + port

![Запуск команды на уровне защиты impossible](image/3.png){#fig:003 width=70%}


# Выводы

Я научился находить уязвимости с помощью утилиты nikto
