---
## Front matter
title: "Отчёт по Индивидуальному проекту этап 5"
subtitle: "Операционные системы"
author: "Шатохина Виктория Сергеевна "

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

Добавить к сайту все остальные элементы.

# Задание

Сделать записи для персональных проектов.
Сделать пост по прошедшей неделе.
Добавить пост на тему "Языки научного программирования"
   
# Выполнение

Сделали записи для персональных проектов. (рис. [-@fig:001]) (рис. [-@fig:002]) https://github.com/vsshatokhina/study_2021-2022_os-intro/blob/master/project-personal/stage5/report/image/1.png  https://github.com/vsshatokhina/study_2021-2022_os-intro/blob/master/project-personal/stage5/report/image/2.jpg

![Записи для персональных проектов](image/1.png){ #fig:001 width=70% }

![Проект](image/2.jpg){ #fig:002 width=70% }

Сделала пост по прошлой неделе. (рис. [-@fig:003])  https://github.com/vsshatokhina/study_2021-2022_os-intro/blob/master/project-personal/stage5/report/image/3.png

![Пост по прошлой неделе](image/3.png){ #fig:003 width=70% }

Добавила пост на тему по выбору. (рис. [-@fig:004]) https://github.com/vsshatokhina/study_2021-2022_os-intro/blob/master/project-personal/stage5/report/image/4.png

![Пост по прошлой неделе](image/4.png){ #fig:004 width=70% }

# Выводы

Добавили к сайту все остальные элементы.

# Список литературы{.unnumbered}

::: {#refs}
:::
