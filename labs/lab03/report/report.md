---
## Front matter
title: "Лабораторная работа №3"
subtitle: "Markdown"
author: "Тулеуов Мади"

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

Научиться оформлять отчёты с помощью легковесного языка разметки Markdown.

# Задание

- Сделать отчёт по предыдущей лабораторной работе в формате Markdown.

# Теоретическое введение

## Базовые сведения о Markdown:

Чтобы создать заголовок, используйте знак ( # ), например:

```
1. # This is heading 1
2. ## This is heading 2
3. ### This is heading 3
4. #### This is heading 4
```

Чтобы задать для текста полужирное начертание, заключите его в двойные звездочки:
This text is **bold**.

Чтобы задать для текста курсивное начертание, заключите его в одинарные звездочки:
 This text is *italic*.

Чтобы задать для текста полужирное и курсивное начертание, заключите его в тройные звездочки:
> This is text is both ***bold and italic***.

Блоки цитирования создаются с помощью символа >:
- > The drought had lasted now for ten million years, and the reign of
the terrible lizards had long since ended. Here on the Equator, in
the continent which would one day be known as Africa, the battle
for existence had reached a new climax of ferocity, and the victor
was not yet in sight. In this barren and desiccated land, only the
small or the swift or the fierce could flourish, or even hope to
survive.

Неупорядоченный (маркированный) список можно отформатировать с помощью звездочек или тире:
> - List item 1*
> - List item 2*
> - List item 3*

Чтобы вложить один список в другой, добавьте отступ для элементов дочернего списка:
> -  List item 1*
>   -  List item A*
>   -  List item B*
> -  List item 2*

Упорядоченный список можно отформатировать с помощью соответствующих цифр:

>1. First instruction*
>1. Second instruction*
>1. Third instruction*

Чтобы вложить один список в другой, добавьте отступ для элементов дочернего списка:

>1. First instruction*
>-  1. Sub-instruction*
>-  1. Sub-instruction*
>1. Second instruction*

Синтаксис Markdown для встроенной ссылки состоит из части [link text] , представляющей текст гиперссылки, и части (file-name.md) – URL-адреса или имени файла,
на который дается ссылка:
> [link text](file-name.md)

Markdown поддерживает как встраивание фрагментов кода в предложение, так и их
размещение между предложениями в виде отдельных огражденных блоков. Огражденные
блоки кода — это простой способ выделить синтаксис для фрагментов кода. Общий
формат огражденных блоков кода:

>- ``` language
>-  your code goes in here
>-  ``` 

# Выполнение лабораторной работы

**1.** Открыл шаблон отчета и заполнил титульный лист(рис. [-@fig:001])

![Редактирование титульного листа](image/1.png){ #fig:001 width=70% }

**2.** Расписал цель работы и задания(рис. [-@fig:002])

![Цель работы и задания](image/2.png){ #fig:002 width=70% }

**3.** Сохранил все скриншоты из отчета в формате *doc* в папку *image*(рис. [-@fig:003])

![Сохранение всех скриншиотов](image/5.png){ #fig:003 width=70% }

**4.** Заполнил ход работы(рис. [-@fig:004])

![Заполнение хода работы](image/6.png){ #fig:004 width=70% }

**5.** Скопировал контрольные вопросы и ответы на них из отчета(рис. [-@fig:005])

![Контрольные вопросы](image/7.png){ #fig:005 width=70% }

**6.** Записал вывод.(рис. [-@fig:006])

![Вывод](image/8.png){ #fig:006 width=70% }


# Выводы

Мы научились оформлять отчёты с помощью легковесного языка разметки Markdown.