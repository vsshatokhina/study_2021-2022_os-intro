---
## Front matter
title: "Отчёт по Индивидуальному проекту этап 4"
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

Добавить к сайту ссылки на научные и библиометрические ресурсы. Опубликовать пост.

# Задание

Зарегистрироваться на соответствующих ресурсах и разместить на них ссылки на сайте:

Сделать пост по прошедшей неделе.
   
Добавить пост на тему по выбору: Оформление отчёта.
        
# Выполнение

Демидова Анастасия Вячеславовна разрешила не регистрироваться на сайтах. Поэтому я разместила ссылки на свои социальные сети. (рис. [-@fig:001])

![Размещение ссылок](image/1.png){ #fig:001 width=70% }

Далее я сделала пост по прошлой неделе.  (рис. [-@fig:002])

![Пост по неделе](image/2.png){ #fig:002 width=70% }

Также написала и опубликовала пост на тему "Оформление отчёта" (рис. [-@fig:003])

![Пост на тему](image/3.png){ #fig:003 width=70% }


# Выводы

Добавили к сайту ссылки на научные и библиометрические ресурсы. Опубликовали посты.

# Список литературы{.unnumbered}

::: {#refs}
:::
