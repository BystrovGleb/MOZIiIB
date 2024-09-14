---
## Front matter
title: "Отчёт по лабораторной работе №1"
subtitle: "Простейший вариант"
author: "<Быстров Глеб Андреевич>"

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
mainfont: IBM Plex Serif
romanfont: IBM Plex Serif
sansfont: IBM Plex Sans
monofont: IBM Plex Mono
mathfont: STIX Two Math
mainfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
romanfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
sansfontoptions: Ligatures=Common,Ligatures=TeX,Scale=MatchLowercase,Scale=0.94
monofontoptions: Scale=MatchLowercase,Scale=0.94,FakeStretch=0.9
mathfontoptions:
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

Научиться программировать на языке Julia и узнать как работает шифр Цезаря и шифр Атбаш.

# Задание

1. Реализовать шифр Цезаря с произвольным ключом k
2. Реализовать шифр Атбаш

# Теоретическое введение

Шифр Цезаря (также он является шифром простой замены) - это
моноалфавитная подстановка, т.е. каждой букве открытого текста ставится в соответсвие одна буква шифртекста.
В основе функционирования шифров простой замены лежит следующий
принцип: для получения шифротекста отдельные символы или группы символов исходного алфавита заменяются символами или группами символов шифроалфавита. На практике при создании шифра простой
замены в качестве шифроалфавита берется исходный алфавит, но с нарушенным порядком букв (алфавитная перестановка). Для запоминания нового порядка букв перемешивание алфавита осуществляется с помощью пароля. В качестве пароля могут выступать слово или несколько слов с неповторяющимися буквами.

Данный шифр является шифром сдвига на всю длину алфавита. Для
алфавита, состоящего только из русских букв и пробела, таблица шифрования будет иметь следующий вид:
абвгдежзийклмноп рстуфхцчшщъыьэюя
яюэьыъщшчцхфутср по нм л к й и з же г в б а

# Выполнение лабораторной работы

1. Реализовал на языке Julia шифр Цезаря с произвольным ключом k(рис. [-@fig:001]).

![Код с выводом](image/1.png){#fig:001 width=70%}

2. Реализовал на языке Julia шифр Атбаш (рис. [-@fig:001]).

![Код с выводом](image/2.png){#fig:001 width=70%}

# Выводы

Успешно удалось научиться программировать на языке Julia и узнать как работает шифр Цезаря и шифр Атбаш.

# Список литературы{.unnumbered}

::: {#refs}
:::
