---
## Front matter
lang: ru-RU
title: Лаб 4 git
subtitle: Продвинутое использование git
author:
  - Талебу тенке ф.
institute:
  - Российский университет дружбы народов, Москва, Россия
  - Объединённый институт ядерных исследований, Дубна, Россия
date: 01 января 1970

## i18n babel
babel-lang: russian
babel-otherlangs: english

## Formatting pdf
toc: false
toc-title: Содержание
slide_level: 2
aspectratio: 169
section-titles: true
theme: metropolis
header-includes:
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
 - '\makeatletter'
 - '\beamer@ignorenonframefalse'
 - '\makeatother'
---

# Информация

## Докладчик

:::::::::::::: {.columns align=center}
::: {.column width="70%"}

  * Талебу тенке франк устон.
  * д.ф.-м.н., профессор
  * профессор кафедры прикладной информатики и теории вероятностей
  * Российский университет дружбы народов
  * [kulyabov-ds@rudn.ru](mailto:kulyabov-ds@rudn.ru)
  * <https://yamadharma.github.io/ru/>

:::
::: {.column width="30%"}

![](./image/kulyabov.jpg)

:::
::::::::::::::

# Вводная часть

## Актуальность

Рабочий процесс Gitflow

## Объект и предмет исследования

- Презентация как текст
- Программное обеспечение для создания презентаций
- Входные и выходные форматы презентаций

## Цели и задачи
еоретические сведения

    Рабочий процесс Gitflow
        Общая информация
        Процесс работы с Gitflow
    Семантическое версионирование
        Краткое описание семантического версионирования
        Программное обеспечение
    Общепринятые коммиты
        Описание


## Материалы и методы

- Процессор `pandoc` для входного формата Markdown
- Результирующие форматы
	- `pdf`
	- `html`
- Автоматизация процесса создания: `Makefile`

# Создание презентации

## Процессор `pandoc`

- Pandoc: преобразователь текстовых файлов
- Сайт: <https://pandoc.org/>
- Репозиторий: <https://github.com/jgm/pandoc>

## Формат `pdf`

- Использование LaTeX
- Пакет для презентации: [beamer](https://ctan.org/pkg/beamer)
- Тема оформления: `metropolis`

## Код для формата `pdf`

```yaml
slide_level: 2
aspectratio: 169
section-titles: true
theme: metropolis
```

## Формат `html`

- Используется фреймворк [reveal.js](https://revealjs.com/)
- Используется [тема](https://revealjs.com/themes/) `beige`

## Код для формата `html`

- Тема задаётся в файле `Makefile`

```make
REVEALJS_THEME = beige 
```
# Результаты

## Получающиеся форматы

- Полученный `pdf`-файл можно демонстрировать в любой программе просмотра `pdf`
- Полученный `html`-файл содержит в себе все ресурсы: изображения, css, скрипты

# Элементы презентации

## Актуальность

- Даёт понять, о чём пойдёт речь
- Следует широко и кратко описать проблему
- Мотивировать свое исследование
- Сформулировать цели и задачи
- Возможна формулировка ожидаемых результатов

## Цели и задачи
![](./image/1.jpg)
еоретические сведения

    Рабочий процесс Gitflow
        Общая информация
        Процесс работы с Gitflow
    Семантическое версионирование
        Краткое описание семантического версионирования
        Программное обеспечение
    Общепринятые коммиты
        Описание


## Материалы и методы
![](./image/2.jpg)
- Представляйте данные качественно
- Количественно, только если крайне необходимо
- Излишние детали не нужны

## Содержание исследования

- Предлагаемое решение задач исследования с обоснованием
- Основные этапы работы

## Результаты
![](./image/3.jpg)
- Не нужны все результаты
- Необходимы логические связки между слайдами
- Необходимо показать понимание материала


## Итоговый слайд
![](./image/4.jpg)
- Запоминается последняя фраза. © Штирлиц
- Главное сообщение, которое вы хотите донести до слушателей
- Избегайте использовать последний слайд вида *Спасибо за внимание*

# Рекомендации

## Принцип 10/20/30

  - 10 слайдов
  - 20 минут на доклад
  - 30 кегль шрифта

## Связь слайдов

::: incremental

- Один слайд --- одна мысль
- Нельзя ссылаться на объекты, находящиеся на предыдущих слайдах (например, на формулы)
- Каждый слайд должен иметь заголовок

:::

## Количество сущностей

::: incremental

- Человек может одновременно помнить $7 \pm 2$ элемента
- При размещении информации на слайде старайтесь чтобы в сумме слайд содержал не более 5 элементов
- Можно группировать элементы так, чтобы визуально было не более 5 групп

:::

## Общие рекомендации

Установка git-flow
![](./image/5.jpg)
    Linux

        Fedora

            Установка из коллекции репозиториев Copr (https://copr.fedorainfracloud.org/coprs/elegos/gitflow/):

            # Enable the copr repository
            dnf copr enable elegos/gitflow
            # Install gitflow
            dnf install gitflow

Установка Node.js

На Node.js базируется программное обеспечение для семантического версионирования и общепринятых коммитов.

    Fedora

    dnf install nodejs
    apt-get install pnpm

Настройка Node.js

Для работы с Node.js добавим каталог с исполняемыми файлами, устанавливаемыми yarn, в переменную PATH.

    Запустите:
![](./image/5.jpg)
    pnpm setup

    Перелогиньтесь, или выполните:

    source ~/.bashrc

Общепринятые коммиты

    commitizen

        Данная программа используется для помощи в форматировании коммитов.

        pnpm add -g commitizen

        При этом устанавливается скрипт git-cz, который мы и будем использовать для коммитов.
![](./image/6.jpg)
    standard-changelog

        Данная программа используется для помощи в создании логов.

        pnpm add -g standard-changelog

    Практический сценарий использования git

        Создание репозитория git

            Подключение репозитория к github
![](./image/7.jpg)
                Создайте репозиторий на GitHub. Для примера назовём его git-extended.

                Делаем первый коммит и выкладываем на github:

                git commit -m "first commit"
                git remote add origin git@github.com:<username>/git-extended.git
                git push -u origin master

            Конфигурация общепринятых коммитов

                Конфигурация для пакетов Node.js

                pnpm init

                Необходимо заполнить несколько параметров пакета.
                    Название пакета.
                    Лицензия пакета. Список лицензий для npm: https://spdx.org/licenses/. Предлагается выбирать лицензию CC-BY-4.0.
![](./image/8.jpg)
                Сконфигурим формат коммитов. Для этого добавим в файл package.json команду для формирования коммитов:

                "config": {
                    "commitizen": {
                        "path": "cz-conventional-changelog"
                    }
                }

                Таким образом, файл package.json приобретает вид:
![](./image/9.jpg)
                {
                    "name": "git-extended",
                    "version": "1.0.0",
                    "description": "Git repo for educational purposes",
                    "main": "index.js",
                    "repository": "git@github.com:username/git-extended.git",
                    "author": "Name Surname <username@gmail.com>",
                    "license": "CC-BY-4.0",
                    "config": {
                        "commitizen": {
                            "path": "cz-conventional-changelog"
                        }
                    }    
                }
![](./image/10.jpg)
                Добавим новые файлы:

                git add .

                Выполним коммит:

                git cz

                Отправим на github:

                git push

            Конфигурация git-flow

                Инициализируем git-flow
![](./image/11.jpg)
                git flow init

                Префикс для ярлыков установим в v.

                Проверьте, что Вы на ветке develop:

                git branch

                Загрузите весь репозиторий в хранилище:

                git push --all
![](./image/12.jpg)
                Установите внешнюю ветку как вышестоящую для этой ветки:

                git branch --set-upstream-to=origin/develop develop

                Создадим релиз с версией 1.0.0

                git flow release start 1.0.0

                Создадим журнал изменений

                standard-changelog --first-release
![](./image/13.jpg)
                Добавим журнал изменений в индекс

                git add CHANGELOG.md
                git commit -am 'chore(site): add changelog'

                Зальём релизную ветку в основную ветку
![](./image/14.jpg)
                git flow release finish 1.0.0

                Отправим данные на github

                git push --all
                git push --tags

                Создадим релиз на github. Для этого будем использовать утилиты работы с github:
![](./image/15.jpg)
                gh release create v1.0.0 -F CHANGELOG.md

        Работа с репозиторием git

            Разработка новой функциональности

                Создадим ветку для новой функциональности:

                git flow feature start feature_branch
![](./image/16.jpg)
                Далее, продолжаем работу c git как обычно.

                По окончании разработки новой функциональности следующим шагом следует объединить ветку feature_branch c develop:

                git flow feature finish feature_branch

            Создание релиза git-flow
![](./image/17.jpg)
                Создадим релиз с версией 1.2.3:

                git flow release start 1.2.3

                Обновите номер версии в файле package.json. Установите её в 1.2.3.

                Создадим журнал изменений

                standard-changelog
![](./image/18.jpg)
                Добавим журнал изменений в индекс

                git add CHANGELOG.md
                git commit -am 'chore(site): update changelog'

                Зальём релизную ветку в основную ветку

                git flow release finish 1.2.3

                Отправим данные на github

                git push --all
                git push --tags
![](./image/19.jpg)
                Создадим релиз на github с комментарием из журнала изменений:

                gh release create v1.2.3 -F CHANGELOG.md
![](./image/20.jpg)


## Представление данных

::: incremental

- Лучше представить в виде схемы
- Менее оптимально представить в виде рисунка, графика, таблицы
- Текст используется, если все предыдущие способы отображения информации не подошли

:::

