---
## Front matter
title: "Третий этап индивидуалный проект"
subtitle: "Skills, Accomplish­ments and posts"
author: "Талебу тенке Франк устон"

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

Продолжить редактирование личного сайта. Добавить к сайту достижения.

# Задание
    Список достижений.
    Добавить информацию о навыках (Skills).
    Добавить информацию об опыте (Experience).
    Добавить информацию о достижениях (Accomplishments).
    Сделать пост по прошедшей неделе.
    Добавить пост на тему по выбору:
    Легковесные языки разметки.
    Языки разметки. LaTeX.
    Язык разметки Markdown.

# Выполнение лабораторной работы
    Добавить информацию о навыках (Skills).
    Добавить информацию об опыте (Experience).
    Добавить информацию о достижениях (Accomplishments).
    Сделать пост по прошедшей неделе.
    Язык разметки Markdown.
    
    (рис. [-@fig:001]).

    ![Рис.1](image/1.png){ #fig:001 width=100%}

    (рис. [-@fig:002]).

    ![Рис.2](image/2.png){ #fig:002 width=100%}

    (рис. [-@fig:003]).

    ![Рис.3](image/3.png){ #fig:003 width=100%}

   (рис. [-@fig:004]).

    ![Рис.4](image/4.png){ #fig:004 width=100%}

    (рис. [-@fig:005]).

    ![Рис.5](image/5.png){ #fig:005 width=100%}

    ((рис. [-@fig:006]).

    ![Рис.6](image/6.png){ #fig:006 width=100%}

    (рис. [-@fig:007]).

    ![Рис.7](image/7.png){ #fig:007 width=100%}

    (рис. [-@fig:008]).

    ![Рис.8](image/8.png){ #fig:008 width=100%}

    (рис. [-@fig:009]).

    ![Рис.9](image/9.png){ #fig:009 width=100%}


    (рис. [-@fig:010]).

    ![Рис.10](image/10.png){ #fig:006 width=100%}


# Список литературы{.unnumbered}

::: {#refs}
:::
