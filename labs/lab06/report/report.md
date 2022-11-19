---
## Front matter
title: "Отчет по лабораторной работе 6"
subtitle: "Основы работы с midnight commander. Структура программы на языке ассемблера NASM"
author: "Симко Сергей Евгеньевич"

## Generic otions
lang: ru-RU
toc-title: "Содержание"

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

Приобретение практических навыков работы с midnight commander. Освоение инструций языка ассемблера mov и int

# Выполнение лабораторной работы

![рис. 1](image/i1.png){ #fig:001 width=70% }
Открываем mc

![рис. 2](image/i2.png){ #fig:002 width=70% }
Создаем в каталоге с программами из прошлой лабораторной каталог lab06

![рис. 3](image/i3.png){ #fig:003 width=70% }
Командой touch создаем файл lab6-1.asm

![рис. 4](image/i4.png){ #fig:004 width=70% }
Пишем код из лабораторной работы и собираем в исполняемый файл

![рис. 5](image/i5.png){ #fig:005 width=70% }
Проверяем работу программы

![рис. 6](image/i6.png){ #fig:006 width=70% }
Устанавливаем файл in_out.asm

![рис. 7](image/i7.png){ #fig:007 width=70% }
Делаем копию первого .asm файла

![рис. 8](image/i8.png){ #fig:008 width=70% }
Переделываем программу с новыми функциями

![рис. 9](image/i9.png){ #fig:009 width=70% }
Собираем файл

![рис. 10](image/i10.png){ #fig:010 width=70% }
Делаем новый .asm файл

![рис. 11](image/i11.png){ #fig:011 width=70% }
Пишем программу, которая запрашивает строку, а затем выводит ее в консоль

![рис. 12](image/i12.png){ #fig:012 width=70% }
собираем

![рис. 13](image/i13.png){ #fig:013 width=70% }
Проверяем работу

![рис. 14](image/i14.png){ #fig:014 width=70% }
Делаем новый файл, делающий то же самое, но с функциями из in_out

![рис. 15](image/i15.png){ #fig:015 width=70% }
проверяем работу

# Выводы

Мы обрели навыки пользования midnight commander и изучили инструкции mov и int на ассемблере nasm.