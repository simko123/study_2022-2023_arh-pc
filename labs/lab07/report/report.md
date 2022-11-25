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

Освоение арифметических инструкций языка ассемблера NASM.

# Выполнение лабораторной работы

![рис. 1](image/i1.png){ #fig:001 width=60% }
Создаем директорию для нашей лаб. работы и в ней создаем .asm файл.

![рис. 2](image/i2.png){ #fig:002 width=60% }
Пишем код.

![рис. 3](image/i3.png){ #fig:003 width=60% }
Собираем и запускаем.

![рис. 4](image/i4.png){ #fig:004 width=60% }
Заменяем в коде символы на числа.

![рис. 5](image/i5.png){ #fig:005 width=60% }
Снова собираем и запускаем. 

![рис. 6](image/i6.png){ #fig:006 width=60% }
Создаем новый .asm и пишем в него код.

![рис. 7](image/i7.png){ #fig:007 width=60% }
Собираем и запускаем.

![рис. 8](image/i8.png){ #fig:008 width=60% }
Заменив символы на числа, наконец, получаем интересующий нас результат!

![рис. 9](image/i9.png){ #fig:009 width=60% }
Заменяем в программе функцию iprintLF на iprint

![рис. 10](image/i10.png){ #fig:010 width=60% }
Теперь вывод отличается от предыдущего, в нем нет переноса строки.

![рис. 11](image/i11.png){ #fig:011 width=60% }
Пишем новую программу.

![рис. 12](image/i12.png){ #fig:012 width=60% }
Собираем и запускаем. Результат соответствует ожидаемому.

![рис. 13](image/i13.png){ #fig:013 width=60% }
Немного меняем формулу.

![рис. 14](image/i14.png){ #fig:014 width=60% }
Получаем новый результат.

![рис. 15](image/i15.png){ #fig:015 width=60% }
Пишем программу генерации варианта на основе номера студ. билета.

![рис. 16](image/i16.png){ #fig:016 width=60% }
Собираем и запускаем. Посчитав вручную, удостоверяемся, что результат правильный.

# Ответы на вопросы

1. Первые две строки во входной функции.
2. Инструкции отвечают за ввод студ. билета.
3. Для преобразования ASCII в число (aSCII to iNTEGER).
4. xor edx,edx; mov ebx,20; div ebx; inc edx
5. edx
6. Прибавить к значению в edx единицу.
7. mov eax,rem; call sprint; mov eax,edx; call iprintLF

# Самостоятельная работа

![рис. 17](image/i17.png){ #fig:017 width=60% }
Пишем программу

![рис. 18](image/i18.png){ #fig:018 width=60% }
Проверяем результат для интересующих значений

# Выводы

Мы изучили арифметические операции в nasm.