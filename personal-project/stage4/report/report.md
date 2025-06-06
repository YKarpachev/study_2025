---
## Front matter
title: "Проект Этап 5"
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

Найти уязвимости с помощью nikto

# Задание

0. приготовить mysql, apache2
1. найти точку входа на DVWA (айпи адрес + порт или полный URL)
2. запустить провеку на уровне защиты low
3. запустить проверку на уровне защиты imposible

# Выполнение лабораторной работы

1. запускаем две команды одна для mysql, другая для apache2

![Запуск команд](image/1.png){#fig:001 width=70%}

2. Запускаем проверку на уровне защиты low, full url path

![Запуск команды на уровне защиты low](image/2.png){#fig:002 width=70%}

3. Запускаем проверку на уровне защиты imposible, ip + port

![Запуск команды на уровне защиты impossible](image/3.png){#fig:003 width=70%}

# Выводы

Я научился находить уязвимости с помощью утилиты nikto
