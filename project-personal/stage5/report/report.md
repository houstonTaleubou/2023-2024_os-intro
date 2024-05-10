---
## Front matter
title: "5 этап индивидуалного проекта"
subtitle: "Добавить с сайту все остальные элементы."
author: "Талебу тенке франк устон"

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
Добавить с сайту все остальные элементы.

    Сделать записи для персональных проектов.
    Сделать пост по прошедшей неделе.
    Добавить пост на тему по выбору.
    Языки научного программирования.

# Выполнение лабораторной работы
Добавить с сайту все остальные элементы.

    Сделать записи для персональных проектов.
    Сделать пост по прошедшей неделе.
    Добавить пост на тему по выбору.
       Языки научного программирования.
       
(рис. [-@fig:001]).

![Название рисунка](image/1.png){#fig:001 width=70%}

(рис. [-@fig:002]).

![Название рисунка](image/2.png){#fig:002 width=70%}

(рис. [-@fig:003]).

![Название рисунка](image/3.png){#fig:003 width=70%}

(рис. [-@fig:004]).

![Название рисунка](image/4.png){#fig:004 width=70%}


(рис. [-@fig:005]).

![Название рисунка](image/5.png){#fig:005 width=70%}

(рис. [-@fig:006]).

![Название рисунка](image/6.png){#fig:006 width=70%}

(рис. [-@fig:007]).
![Название рисунка](image/7.png){#fig:007 width=70%}

(рис. [-@fig:008]).

![Название рисунка](image/8.png){#fig:008 width=70%}

(рис. [-@fig:009]).

![Название рисунка](image/9.png){#fig:009 width=70%}

(рис. [-@fig:010]).

![Название рисунка](image/10.png){#fig:010 width=70%}

# Список литературы{.unnumbered}

::: {#refs}
:::
