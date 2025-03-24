---
## Front matter
title: "Проект Этап 3"
subtitle: "Отчет"
author: "Карпачев Ярослав"

## Generic otions
lang: ru-RU
toc-title: "Содержание"

## Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

## Pdf output format
toc: true # Table of contents
toc-depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4
documentclass: scrreprt
## I18n polyglossia
polyglossia-lang:
  name: russian
  options:
	- spelling=modern
	- babelshorthands=true
polyglossia-otherlangs:
  name: english
## I18n babel
babel-lang: russian
babel-otherlangs: english
## Fonts
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase,Scale=0.9
## Biblatex
biblatex: true
biblio-style: "gost-numeric"
biblatexoptions:
  - parentracker=true
  - backend=biber
  - hyperref=auto
  - language=auto
  - autolang=other*
  - citestyle=gost-numeric
## Pandoc-crossref LaTeX customization
figureTitle: "Рис."
tableTitle: "Таблица"
listingTitle: "Листинг"
lofTitle: "Список иллюстраций"
lotTitle: "Список таблиц"
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

С помощью Hydra взломать пароль (в данном случае DVWA который мы получили при установки приложения)

# Задание

1. Получить лист с паролями
2. Создать команду
3. Проверить пароль

# Выполнение лабораторной работы

1. Анзипаем встроенный список с паролями для брут форса - rockyou.txt

![Распаковка паролей](image/1.png){#fig:000 width=70%}

2. Для того чтобы получить точку доступа скачиваем любой cooky анализатор и используем его на форме

![Куки с данными](image/3.png){#fig:000 width=70%}

3. С помощью данных параметров запускаем команду и ждем ее завершения

![Главная команда](image/2.png){#fig:001 width=70%}


4. Проверяем что все пароль действительно правильный

![Проверка пароля](image/4.png){#fig:004 width=70%}


# Выводы

Я понял как брутфорсить HTML формы
