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

Получение практических навыков работы в консоли с атрибутами фай-
лов для групп пользователей

# Задание

1. В установленной операционной системе создайте учётную запись поль-
зователя guest (использую учётную запись администратора):
useradd guest
2. Задайте пароль для пользователя guest (использую учётную запись ад-
министратора):
passwd guest
3. Аналогично создайте второго пользователя guest2.
4. Добавьте пользователя guest2 в группу guest:
gpasswd -a guest2 guest
5. Осуществите вход в систему от двух пользователей на двух разных кон-
солях: guest на первой консоли и guest2 на второй консоли.
6. Для обоих пользователей командой pwd определите директорию, в кото-
рой вы находитесь. Сравните её с приглашениями командной строки.
7. Уточните имя вашего пользователя, его группу, кто входит в неё
и к каким группам принадлежит он сам. Определите командами
groups guest и groups guest2, в какие группы входят пользовате-
ли guest и guest2. Сравните вывод команды groups с выводом команд
id -Gn и id -G.
8. Сравните полученную информацию с содержимым файла /etc/group.
Просмотрите файл командой
cat /etc/group
9. От имени пользователя guest2 выполните регистрацию пользователя
guest2 в группе guest командой
newgrp guest
10. От имени пользователя guest измените права директории /home/guest,
разрешив все действия для пользователей группы:
chmod g+rwx /home/guest
11. От имени пользователя guest снимите с директории /home/guest/dir1
все атрибуты командой
chmod 000 dirl

# Выполнение лабораторной работы

1. Логинемся через корень  создаем двоих юзеров, ставим на всех пароль, создаем и определяем пользователей в группы.

![Команды для вышеуказанных действий](image/1.png){#fig:001 width=70%}

2. Логинемся по отдельности в каждого пользователя и получаем информацию, айди, в каких группах состоит пользователь и какие группы вообще есть (для 1го пользователя) (для pwd - /home/имяюзера)

![Консольный вывод на команды для 1го юзера](image/2.png){#fig:002 width=70%}

![Консольный вывод на команды для 2го юзера](image/3.png){#fig:003 width=70%}

3. Сравниваем информацию с файлом /etc/group/

![Содержание файла /etc/group/](image/4.png){#fig:004 width=70%}

4. Создаем через второго пользователя новую группу

![Создание группы через второго пользователя](image/5.png){#fig:004 width=70%}

5. Снимаем все разрешения с файла и проверяем что действительно снялись

![Проверка что разрешения снялись](image/6.png){#fig:004 width=70%}

6. Заполняем таблицу

| Операция                  | Минимальные права на директорию | Минимальные права на файл |
|---------------------------|---------------------------------|---------------------------|
| Создание файла           | w + x                           | – (не требуется)          |
| Удаление файла           | w + x                           | – (не требуется)          |
| Чтение файла             | x (если имя файла известно)     | r                         |
| Запись в файл            | x (для доступа к самому файлу)  | w                         |
| Переименование файла     | w + x                           | – (не требуется)          |
| Создание поддиректории   | w + x                           | – (не требуется)          |
| Удаление поддиректории   | w + x                           | – (не требуется)          |

# Выводы

Я получил практические навыки работы в консоли с атрибутами фай-
лов для групп пользователей

# Список литературы{.unnumbered}

::: {#refs}
:::
