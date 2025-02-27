---
## Front matter
title: "Лабораторная 1"
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

Целью данной работы является приобретение практических навыков
установки операционной системы на виртуальную машину, настройки ми-
нимально необходимых для дальнейшей работы сервисов.

# Задание

1. создать папку в нужном месте

2. открыть virtual box и выполнить настройку

3. сделать настройку виртуальной машины

4. запустить виртуальную машину и выполнить внутренню настройку

5. установка и перезагрузка

# Выполнение лабораторной работы

1. создаем папку /var/tmp/yokarpachev

![Терминал с папкой](image/1.png){#fig:001 width=70%}

2. Отрыть виртуал бокс и изменить дефолтную папку для машин на /var/tmp/yokarpachev

3. Сделать настройку машины

![Общии настройки](image/2.png){#fig:002 width=70%}
![это нужно отключить](image/3.png){#fig:003 width=70%}
![память](image/4.png){#fig:004 width=70%}
![диск жесткий](image/5.png){#fig:005 width=70%}

4. запустить виртуальную машину и выполнить внутренню настройку

![язык](image/6.png){#fig:002 width=70%}

![Настройки внутренние](image/7.png){#fig:002 width=70%}

5. установка и перезагрузка

![Проверка верности установки](image/8.png){#fig:002 width=70%}

# Выводы

Я зопустил минимальную виртуальную машину

# Список литературы{.unnumbered}

::: {#refs}
:::
