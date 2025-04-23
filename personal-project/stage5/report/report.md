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

Взломать пароль с помощью Burp Suit

# Задание

0. приготовить mysql, apache2
1. сделать настройку браузера
2. перехватить посылку неправильного пароля
3. подготовить и запустить атаку
4. найти запрос который пересылает нас на новую страницу и ретранслировать его

# Выполнение лабораторной работы

1. запускаем две команды одна для mysql, другая для apache2, а также сам Burp Suit

![Запуск команд](image/1.png){#fig:001 width=70%}

2. настраиваем окружение

![рокси для браузера](image/2.png){#fig:002 width=70%}

![перехват в преложении](image/3.png){#fig:003 width=70%}

![возможность перехвата в браузере](image/4.png){#fig:004 width=70%}

3. перехватываем нужный запрос

![запрос с неверными данными](image/6.png){#fig:006 width=70%}


4. готовим атаку

![гатовим аттаку](image/7.png){#fig:007 width=70%}

5. запускаем атаку

![пройденная аттаку](image/8.png){#fig:008 width=70%}

6. находим запрос который отличается

![отличный запрос](image/9.png){#fig:009 width=70%}

7. ретланслируем

![ретрансляция верного пароля](image/10.png){#fig:0010 width=70%}

# Выводы

я научился использовать burp suit для взлома паролей

Я научился находить уязвимости с помощью утилиты nikto
