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

Взломать пароль с помощью Burp Suit

# Выполнение лабораторной работы

## запускаем две команды одна для mysql, другая для apache2, а также сам Burp Suit

![Запуск команд](image/1.png){#fig:001 width=70%}

## настраиваем окружение

![рокси для браузера](image/2.png){#fig:002 width=70%}

![перехват в преложении](image/3.png){#fig:003 width=70%}

![возможность перехвата в браузере](image/4.png){#fig:004 width=70%}

## перехватываем нужный запрос

![запрос с неверными данными](image/6.png){#fig:006 width=70%}


## готовим атаку

![гатовим аттаку](image/7.png){#fig:007 width=70%}

## запускаем атаку

![пройденная аттаку](image/8.png){#fig:008 width=70%}

## находим запрос который отличается

![отличный запрос](image/9.png){#fig:009 width=70%}

## ретланслируем

![ретрансляция верного пароля](image/10.png){#fig:0010 width=70%}

## Выводы

я научился использовать burp suit для взлома паролей

