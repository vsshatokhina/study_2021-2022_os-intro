---
## Front matter
lang: ru-RU
title: Индивидуальный проект. Этап 2
author: |
    Шатохина Виктория Сергеевна
date: 06.05.2022

## Formatting
toc: false
slide_level: 2
theme: metropolis
header-includes: 
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
 - '\makeatletter'
 - '\beamer@ignorenonframefalse'
 - '\makeatother'
aspectratio: 43
section-titles: true
---


# Цель работы

Добавление на сайт информации о себе. И создание поста.

# Выполнение лабораторной работы

Для начала зашли в файл `content/authors/admin/_index.md` и написали свои данные.

## Выполнение лабораторной работы

Далее в папку `content/authors/admin/` кладём свою фотографию и даём ей имя `avatar.jpg`

## Выполнение лабораторной работы
Создаём пост.
Я выбрала тему Git.
Для создания поста я зашла в файл `content/post/getting-started/index.md` и изменила в нем контент для нашего поста.

## Выполнение лабораторной работы

Делаем пост по прошедшей неделе.

Нам нужно обновить данные нашего сайта на github pages, чтобы все что мы сделали было не только на localhost.

Для этого воспользуемся командой `hugo` для сборки сайта, в папке `./public` появятся новые static файлы.
Их необходимо будет отправить на гитхаб в репозиторий `<username>.github.io` командой `git push origin main`, предварительно добавив новые файлы (`git add .`) и создав новый коммит (`git commit -am "stage02"`).

В результате получим обновленную страничку.

# Вывод

Отредактировали информацию о себе (Biography, Interests, Education). А также добавили пост на тему контроль версий git.

## {.standout}
Спасибо за внимание!!!
