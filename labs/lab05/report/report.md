---
## Front matter
title: "Лабораторная работа №5"
subtitle: "Настройка рабочей среды"
author: "талебу тенке франк"

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

- Цель работы является научиться настраивать рабочую среду.

# Задание

- 1. Менеджер паролей pass
- 2. Дополнительное программное обеспечение
- 3. Ежедневные операции c chezmoi

# Выполнение лабораторной работы

## Менеджер паролей pass

- установка pass. (рис. [-@fig:001]).

![рисунок 1](image/1.png){#fig:001 width=100%}

- установка gopass. (рис. [-@fig:002]).

![рисунок 2](image/2.png){#fig:002 width=100%}

- Настройка ключи GPG. (рис. [-@fig:003]).

![рисунок 3](image/3.png){#fig:003 width=100%}

- Инициализация хранилища (рис. [-@fig:004]).

![рисунок 4](image/4.png){#fig:004 width=100%}

- Синхронизация с git. Создаём структуру git. (рис. [-@fig:005]).

![рисунок 5](image/5.png){#fig:005 width=100%}

- создание новой репозитории. (рис. [-@fig:006]).

![рисунок 6](image/6.png){#fig:006 width=100%}

- Прямые изменения. (рис. [-@fig:007]).

![рисунок 7](image/7.png){#fig:007 width=100%}


## Настройка интерфейса с броузером

- Интерфейс для взаимодействия с броузером (native messaging). (рис. [-@fig:008]).

![рисунок 8](image/8.png){#fig:008 width=100%}

- (рис. [-@fig:009]).

![рисунок 9](image/9.png){#fig:009 width=100%}


## Сохранение пароля

- Добавить новый пароль. Отображение пароль для указанного имени файла (рис. [-@fig:010]).

![рисунок 10](image/10.png){#fig:010 width=100%}

- Замените существующий пароль (рис. [-@fig:011]).

![рисунок 11](image/11.png){#fig:011 width=100%}


## Дополнительное программное обеспечение

- Установка дополнительного программного обеспечении. (рис. [-@fig:012]).

![рисунок 12](image/12.png){#fig:012 width=100%}

- Установка шрифты. (рис. [-@fig:013]).

![рисунок 13](image/13.png){#fig:013 width=100%}

 (рис. [-@fig:014]).

![рисунок 14](image/14.png){#fig:014 width=100%}

 (рис. [-@fig:015]).

![рисунок 15](image/15.png){#fig:015 width=100%}

- Установка бинарного файла. Скрипт определяет архитектуру процессора и операционную систему и скачивает необходимый файл. (рис. [-@fig:016]).

![рисунок 16](image/16.png){#fig:016 width=100%}

## Создание собственного репозитория с помощью утилит

- Будем использовать утилиты командной строки для работы с github. Создадим свой репозиторий для конфигурационных файлов на основе шаблона. (рис. [-@fig:017]).

![рисунок 17](image/17.png){#fig:017 width=100%}

## Подключение репозитория к своей системе

- Инициализация chezmoi с вашим репозиторием dotfiles. (рис. [-@fig:018]).

![рисунок 18](image/18.png){#fig:018 width=100%}

- Проверка, какие изменения внесёт chezmoi в домашний каталог, запустив. (рис. [-@fig:019]).

![рисунок 19](image/19.png){#fig:019 width=100%}


## Ежедневные операции c chezmoi

- Извлеките последние изменения из репозитория и примените их. (рис. [-@fig:020]).

![рисунок 20](image/20.png){#fig:020 width=100%}

- Извлеките последние изменения из своего репозитория и посмотрите, что изменится, фактически не применяя изменения. (рис. [-@fig:021]).

![рисунок 21](image/21.png){#fig:021 width=100%}

- Автоматически фиксируйте и отправляйте изменения в репозиторий. (рис. [-@fig:022]).

![рисунок 22](image/22.png){#fig:022 width=100%}


# Выводы

- В этой лабораторной работе, я научила настраивать рабочую среду.

# Список литературы{.unnumbered}

::: {#refs}
:::
