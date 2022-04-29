---
## Front matter
title: "Отчёт первого этапа индивидуального проекта"
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

Размещение на Github pages заготовки для персонального сайта.

# Задание

Установить необходимое программное обеспечение.
Скачать шаблон темы сайта.
Разместить его на хостинге git.
Установить параметр для URLs сайта.
Разместить заготовку сайта на Github pages.


# Выполнение работы

Скачиваем исполняемый файл Hugo для того, чтобы генерировать страницы сайта (рис. [-@fig:001])

![Файл Hugo](image/1.png){ #fig:001 width=70% }

Выбираем нужный нам файл (рис. [-@fig:002])

![Выбор файла](image/2.png){ #fig:002 width=70% }

Откываем скачавшийся файл и извлекаем в текущую папку (рис. [-@fig:003])

![Извлекаем файл](image/3.png){ #fig:003 width=70% }

Выбираем файл hugo, создаём в домашнем каталоге папку bin и копируем в неё файл hugo (рис. [-@fig:004])

![Перенос файла hugo](image/4.png){ #fig:004 width=70% }

Далее создаём репозиторий, используя шаблон. Указываем имя блога (рис. [-@fig:005])

![Создание репозитория](image/5.png){ #fig:005 width=70% }

Репозиторий создался. Теперь мы можем его клонировать. Копируем ссылку (рис. [-@fig:006])

![Созданный репозиторий и ссылка на него](image/6.png){ #fig:006 width=70% }

Вставляем ссылку в терминал с командой git clone. Создался каталог блога. (рис. [-@fig:007])

![Клонирование](image/7.png){ #fig:007 width=70% }

Теперь переходим в блог и выполняем команду ~/bin/hugo (рис. [-@fig:008])

![Выполнение нужной команды](image/8.png){ #fig:008 width=70% }

Видим, что появился каталог public. Удаляем его (пока он не нужен нам) (рис. [-@fig:009])

![Удаление каталога public](image/9.png){ #fig:009 width=70% }

Далее выполняем команду ~/bin/hugo server (рис. [-@fig:010])

![Выполнение нужной команды](image/10.png){ #fig:010 width=70% }

Благодаря этой команде мы получили ссылку. Переходим по ней. Получаем сайт, который создался благодаря этой команде. Но нужно удалить один из файлов, чтобы исчез зелёный фон. (рис. [-@fig:011])

![Первоначальный вид сайта](image/11.png){ #fig:011 width=70% }

Чтобы удалить файл нужно перейти в каталог content/home/ и удалить файл demo.md , впоследствии зелёный фон пропал.  (рис. [-@fig:012])

![Убираем залёный фон](image/12.png){ #fig:012 width=70% }

Нужно создать ещё один репозиторий, чтобы доступ к сайту осуществлялся с любого компьютера.

Переходим на Github и создаём новый репозиторий с определённым названием. (рис. [-@fig:013])

![Созаём новый репозиторий](image/13.png){ #fig:013 width=70% }

В терминале клонируем созданный второй репозиторий. Создаём пустой файл README.md (рис. [-@fig:014])

![Клонирование и создание пустого файла](image/14.png){ #fig:014 width=70% }

Теперь мы выполняем команду, которая подключит наш репозиторий к папке паблик нашего блога. (рис. [-@fig:015])

![Подключение репозитория](image/15.png){ #fig:015 width=70% }

Далее заходим в gitignore и комментируем public. (рис. [-@fig:016])

![Комментируем public](image/16.png){ #fig:016 width=70% }

Нужно убедиться, что не будет игнорироваться каталог public (рис. [-@fig:017])

![Выполнение команды](image/17.png){ #fig:017 width=70% }

Проверяем появились ли в каталоге паблик файлы. (рис. [-@fig:018])

![Проверка](image/18.png){ #fig:018 width=70% }

Проверяем подключён ли каталог к репозиторию. (рис. [-@fig:019])

![Проверяем подключение каталога](image/19.png){ #fig:019 width=70% }

Последний шаг. (рис. [-@fig:020])

![Последний шаг](image/20.png){ #fig:020 width=70% }

Проверяем, что всё работает. Обновляем рипозиторий, видим все файлы имеются.

Получаем наш сайт! Готово! (рис. [-@fig:021])

![Проверяем подключение каталога](image/21.png){ #fig:021 width=70% }


# Выводы
Я разместила на Github pages заготовки для своего персонального сайта.




::: 
:::
