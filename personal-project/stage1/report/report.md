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

Установите дистрибутив Kali Linux в виртуальную машину.
В качестве среды виртуализации предлагается использовать VirtualBox.
Сайт Kali Linux: https://www.kali.org/

# Задание

1. Найти образ (скачать так чтобы он был полным а не поврежденным)
2. сделайть настройку Vbox
3. провести установку системы настроек и тд
4. Запустить виртуалку и убидиться что действительно работает

# Выполнение лабораторной работы

1. Скачиваем образ iso с сайта kali linux (https://www.kali.org/get-kali/#kali-installer-images)

2. Вставляем образ в Vbox выбераем подтип uduntu (4096cpu 3core 42gb)

3. Запуска выполняем иструкции - устанавливаем язык, выбераем имя хоста, имя юзера, устанавливам сначала систему, потом выбераем дефолтные иструменты и устанавливам их тоже

![Язык](image/1.png){#fig:001 width=70%}

![Имя хоста](image/2.png){#fig:002 width=70%}

![Имя юзера](image/3.png){#fig:003 width=70%}

![Установко системы](image/4.png){#fig:004 width=70%}

![Установа инструментов](image/5.png){#fig:005 width=70%}

![Установка завершена](image/6.png){#fig:006 width=70%}

4. Перезапускам и проверям что все верноустановленно (зашел на сайт RUDN со своим акком)

![Сайт с моим аккаунтом](image/7.png){#fig:007 width=70%}


# Выводы

Я правильно установил kali linux на Vbox

# Список литературы{.unnumbered}

::: {#refs}
:::
