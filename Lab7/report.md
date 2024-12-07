---
## Front matter
title: "Отчёт по лабораторной работе №7"
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

- Получить понимание как делать дискретное логарифмирование в конечном поле.

# Задание

- Реализовать алгоритм программно

# Теоретическое введение

Задача дискретного логарифмирования, как и задача разложения на
множители, применяется во многих алгоритмах криптографии с открытым
ключом. Предложенная в 1976 году У. Диффи и М. Хеллманом для установления
сеансового ключа, эта задача послужила основой для создания протоколов
шифрования и цифровой подписи, доказательств с нулевым разглашением и
других криптографических протоколов.

# Выполнение лабораторной работы

1. Реализовал алгоритм (рис. [-@fig:001]).

![Код](image/1.png){#fig:001 width=70%}

2. Реализовал алгоритм (рис. [-@fig:002]).

![Код и вывод](image/2.png){#fig:002 width=70%}

# Выводы

Успешно удалось получить понимание как делать дискретное логарифмирование в конечном поле. Реализовал на практике метод.

# Список литературы{.unnumbered}

::: {#refs}
:::
