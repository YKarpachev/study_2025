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

## Цели и задачи

Целью данной работы является приобретение практических навыков
установки операционной системы на виртуальную машину, настройки ми-
нимально необходимых для дальнейшей работы сервисов.

1. создать папку в нужном месте

2. открыть virtual box и выполнить настройку

3. сделать настройку виртуальной машины

4. запустить виртуальную машину и выполнить внутренню настройку

5. установка и перезагрузка

## создаем папку /var/tmp/yokarpachev

![Терминал с папкой](image/1.png){#fig:001 width=70%}

## Отрыть виртуал бокс и изменить дефолтную папку для машин на /var/tmp/yokarpachev

## Сделать настройку машины

![Общии настройки](image/2.png){#fig:002 width=70%}
![это нужно отключить](image/3.png){#fig:003 width=70%}
![память](image/4.png){#fig:004 width=70%}
![диск жесткий](image/5.png){#fig:005 width=70%}

## запустить виртуальную машину и выполнить внутренню настройку

![язык](image/6.png){#fig:002 width=70%}

![Настройки внутренние](image/7.png){#fig:007 width=70%}

## установка и перезагрузка

![Проверка верности установки](image/8.png){#fig:008 width=70%}
