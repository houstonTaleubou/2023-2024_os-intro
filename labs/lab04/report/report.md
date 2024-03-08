---
## Front matter
title: "Шаблон отчёта по лабораторной работе"
subtitle: "Продвинутое исполльзование git"
author: "Талебу тенке франк устно"
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
lot: false # List of tables
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


    Рабочий процесс Gitflow Workflow. Будем описывать его с использованием пакета git-flow.

Общая информация

    Gitflow Workflow опубликована и популяризована Винсентом Дриссеном.
    Gitflow Workflow предполагает выстраивание строгой модели ветвления с учётом выпуска проекта.
    Данная модель отлично подходит для организации рабочего процесса на основе релизов.
    Работа по модели Gitflow включает создание отдельной ветки для исправлений ошибок в рабочей среде.
    Последовательность действий при работе по модели Gitflow:
        Из ветки master создаётся ветка develop.
        Из ветки develop создаётся ветка release.
        Из ветки develop создаются ветки feature.
        Когда работа над веткой feature завершена, она сливается с веткой develop.
        Когда работа над веткой релиза release завершена, она сливается в ветки develop и master.
        Если в master обнаружена проблема, из master создаётся ветка hotfix.
        Когда работа над веткой исправления hotfix завершена, она сливается в ветки develop и master.


# Задание
    Выполнить работу для тестового репозитория.
    Преобразовать рабочий репозиторий в репозиторий с git-flow и conventional commits.


# Теоретическое введение
Рабочий процесс Gitflow
 Рабочий процесс Gitflow Workflow. Будем описывать его с использованием пакета git-flow.

Общая информация
    Gitflow Workflow опубликована и популяризована Винсентом Дриссеном.
    Gitflow Workflow предполагает выстраивание строгой модели ветвления с учётом выпуска проекта.
    Данная модель отлично подходит для организации рабочего процесса на основе релизов.
    Работа по модели Gitflow включает создание отдельной ветки для исправлений ошибок в рабочей среде.
    Последовательность действий при работе по модели Gitflow:


# Выполнение лабораторной работы
Установка программного обеспечения
Установка git-flow
(рис. [-@fig:001]).
![Название рисунка](image/1.jpg){#fig:001 width=70%}

Установка Node.js
(рис. [-@fig:002]).
![Название рисунка](image/2.jpg){#fig:002 width=70%}

Настройка Node.js
Для работы с Node.js добавим каталог с исполняемыми файлами, устанавливаемыми yarn, в переменную PATH.
(рис. [-@fig:003]).
![Название рисунка](image/3.jpg){#fig:003 width=70%}

(рис. [-@fig:009]).
![Название рисунка](image/9.jpg){#fig:009 width=70%}

    Перелогиньтесь, или выполните:
    source ~/.bashrc
Общепринятые коммиты
    commitizen
    (рис. [-@fig:010]).
![Название рисунка](image/10.jpg){#fig:010 width=70%}

Данная программа используется для помощи в форматировании коммитов.
    (рис. [-@fig:011]).
![Название рисунка](image/11.jpg){#fig:011 width=70%}

(рис. [-@fig:004]).

![Название рисунка](image/4.jpg){#fig:004 width=70%}
Данная программа используется для помощи в форматировании коммитов.
 При этом устанавливается скрипт git-cz, который мы и будем использовать для коммитов.
standard-changelog
(рис. [-@fig:005]).
![Название рисунка](image/5.jpg){#fig:005 width=70%}

Подключение репозитория к github
    Создайте репозиторий на GitHub. Для примера назовём его git-extended.
    Делаем первый коммит и выкладываем на github:
(рис. [-@fig:006]).

![Название рисунка](image/6.jpg){#fig:006 width=70%}
Конфигурация общепринятых коммитов
    Конфигурация для пакетов Node.js
    pnpm init
    Необходимо заполнить несколько параметров пакета.
    (рис. [-@fig:012]).
    ![Название рисунка](image/12.jpg){#fig:012 width=70%}
    (рис. [-@fig:013]).
    ![Название рисунка](image/13.jpg){#fig:013 width=70%}
    Добавим новые файлы:
git add .
Выполним коммит:
git cz
Отправим на githu
(рис. [-@fig:014]).
![Название рисунка](image/14.jpg){#fig:014 width=70%}
    
(рис. [-@fig:015]).
    ![Название рисунка](image/15.jpg){#fig:015 width=70%}
    
рис. [-@fig:016]).
![Название рисунка](image/16.jpg){#fig:016 width=70%}
    Конфигурация git-flow

    Инициализируем git-flow
рис. [-@fig:017]).
![Название рисунка](image/17.jpg){#fig:017 width=70%}
    
    Проверьте, что Вы на ветке develop:
рис. [-@fig:018]).
[Название рисунка](image/18.jpg){#fig:018 width=70%}
    Добавим журнал изменений в индекс
    рис. [-@fig:019]).
[Название рисунка](image/19.jpg){#fig:019 width=70%}
    Зальём релизную ветку в основную ветку
    Отправим данные на github
     рис. [-@fig:020]).
    ![Название рисунка](image/20.jpg){#fig:020 width=70%}
# Выводы

Здесь кратко описываются итоги проделанной работы.
