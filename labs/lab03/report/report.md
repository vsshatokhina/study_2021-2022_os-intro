---
## Front matter
title: "Отчёт по лабораторной работе №3"
subtitle:--
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
## lof: true # List of figures
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
1 Изучить идеологию и применение средств контроля знаний.
2 Освоить умения по работе с git


# Задание

Создать базовую конфигурацию для работы с git.
– Создать ключ SSH.
– Создать ключ PGP.
– Настроить подписи git.
– Зарегистрироваться на Github.
– Создать локальный каталог для выполнения заданий по предмету.
# Теоретическое введение

Здесь описываются теоретические аспекты, связанные с выполнением работы.

Например, в табл. [-@tbl:std-dir] приведено краткое описание стандартных каталогов Unix.

: Описание некоторых каталогов файловой системы GNU Linux {#tbl:std-dir}

| Имя каталога | Описание каталога                                                                                                          |
|--------------|----------------------------------------------------------------------------------------------------------------------------|
| `/`          | Корневая директория, содержащая всю файловую                                                                               |
| `/bin `      | Основные системные утилиты, необходимые как в однопользовательском режиме, так и при обычной работе всем пользователям     |
| `/etc`       | Общесистемные конфигурационные файлы и файлы конфигурации установленных программ                                           |
| `/home`      | Содержит домашние директории пользователей, которые, в свою очередь, содержат персональные настройки и данные пользователя |
| `/media`     | Точки монтирования для сменных носителей                                                                                   |
| `/root`      | Домашняя директория пользователя  `root`                                                                                   |
| `/tmp`       | Временные файлы                                                                                                            |
| `/usr`       | Вторичная иерархия для данных пользователя                                                                                 |

Более подробно об Unix см. в [@gnu-doc:bash;@newham:2005:bash;@zarrelli:2017:bash;@robbins:2013:bash;@tannenbaum:arch-pc:ru;@tannenbaum:modern-os:ru].

# Выполнение лабораторной работы
Задаём имя и email владельца репозитория, настраиваем utf-8 в выводе
сообщений git. (рис.[-@fig:001])https://github.com/vsshatokhina/study_2021-2022_os-intro/blob/master/labs/lab03/report/image/%E2%84%961.jpg
![Рис. №1 «Создаём базовую конфигурацию, задаём имя, настраиваем utf-8»](image/№1.jpg){ #fig:001 width=70% }

Настраиваем верификацию и подписание коммитов git. Задаём имя начальной ветки (master), параметр autocrlf и параметр safecrlf. (рис.[ -@fig:002])
![Рис. №2 «Настройка верификации, подписание коммитов, задача имени и параметров»](image/2.jpg){ #fig:002 width=70% }

По алгоритму rsa с ключом размером 4096 бит настраиваем ключ.(рис.[-@fig:003]) 
![Рис. №3 «Выполнение по алгоритму rsa»](image/3.jpg){ #fig:003 width=70% }
![Рис. №4 «Создание ключа ssh»](image/4.jpg){ #fig:004 width=70% }

Далее работаем с сервером репозиториев. Для последующей идентификации
пользователя на сервере репозиториев необходимо сгенерировать пару ключей
(приватный и открытый):
затем, скопировав из локальной консоли ключ в буфер обмена, вставляем ключ
в появившееся на сайте поле.(рис.[ -@fig:005])
![Рис. №5 «Генерируем ключи»](image/5.jpg){ #fig:005 width=70% }
![Рис. №6 «Вставляем ключ на сайт»](image/6.jpg){ #fig:006 width=70% }
Для загрузки репозитория из локального каталога на сервер выполняем следующие
команды: git remote add origin
 ssh://git@github.com/<username>/<reponame>.git
git push -u origin master

Создаём репозиторий.(рис.[ -@fig:007])
![Рис. №7 «Создание репозитоия»](image/7.jpg){ #fig:007 width=70%}
![Рис. №8 «Репозиторий создан»](image/8.jpg){ #fig:008 width=70%}

Создать ключ PGP
Генерируем ключ и выбираем нужные нам опции(рис.[ -@fig:008])
![Рис. №9 «Генерируем ключ»](image/9.jpg){ #fig:009 width=70%}
![Рис. №10 «Выбор нужных условий»](image/10.jpg){ #fig:010 width=70%}

Далее следует ввести пароль. (рис.[ -@fig:011])
![Рис. №11 «Вводим пароль»](image/11.jpg){ #fig:011 width=70%}

Выполняем это задание следующим образом: используя введённый email, указываем Git (применять его при подписи коммитов) (рис.[ -@fig:012])
![Рис. №12 «Выполнение задание №4»](image/12.jpg){ #fig:012 width=70%}
Во время выполнения лабораторной работы я выполнила регистрацию.(рис.[ -@fig:013])
![Рис. №13 «Регистрация на Githab»](image/13.jpg){ #fig:013 width=70%}
Задание было выполнено мною. Каталог создан.(рис.[ -@fig:014])
![Рис. №14 «Созданный каталог»](image/14.jpg){ #fig:014 width=70%}
# Выводы
Мною были изучены идеология и применение средств контроля знаний, освоены умения по работе с git.
