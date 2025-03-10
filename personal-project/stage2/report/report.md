---
## Front matter
title: "Лабораторная 2"
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

Установите DVWA на виртуальную машину
Github DVWA - https://github.com/digininja/DVWA

# Задание

1. Зайти на гитхаб приложения
2. Найти инструкции по билду
3. Запустить необходимые команды
4. Проверить что действительно все установилось

# Выполнение лабораторной работы

1. Берем Гитхаб есть в стадиях проекта ТУИС - (/afs/.dk.sci.pfu.edu.ru/home/y/o/yokarpachev/work/study_2025/personal-project/stage2/report/report.docx)

2. Находи инструкции

![Команды (инструкции)](image/0.png){#fig:000 width=70%}

3. Вставляем инстукции в терминал

![Исполнение команд](image/1.png){#fig:001 width=70%}

![Начало установки DVWA](image/2.png){#fig:002 width=70%}

![Успешная установка](image/3.png){#fig:003 width=70%}

4. Проверяем что все действительно правильно установилось

![Открываем приложение](image/4.png){#fig:004 width=70%}


# Выводы

Я уствновил DVWA на виртуальную машину и провель верную первоначальную настройку DVWA

# Список литературы{.unnumbered}

::: {#refs}
:::
