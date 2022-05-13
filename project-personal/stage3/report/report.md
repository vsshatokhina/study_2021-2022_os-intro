---
## Front matter
title: "Отчёт по этапу №3 Индивидуального проекта"
subtitle: "Операционные системы"
author: "Шатохина Виктория Сергеевна"

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

Добавить к сайту достижения.

# Выполнение лабораторной работы

1. Добавили информацию о навыках (Skills). (рис. [-@fig:001])

![Skills](image/1.png){ #fig:001 width=70% }

2. Добавили информацию об опыте (Experience).(рис. [-@fig:002])

![Experience](image/2.png){ #fig:002 width=70% }

3. Добавили информацию о достижениях (Accomplishments). (рис. [-@fig:003])

![Accomplishments](image/3.png){ #fig:003 width=70% }

4. Сделали пост по прошедшей неделе. (рис. [-@fig:004])

![Пост](image/4.png){ #fig:004 width=70% }

5. Добавили пост на тему (рис. [-@fig:005])

![Сайт](image/5.png){ #fig:005 width=70% }

![Сайт](image/6.png){ #fig:006 width=70% }

# Выводы

Добавили на сайт новую информацию.

# Список литературы{.unnumbered}

::: {#refs}
:::
