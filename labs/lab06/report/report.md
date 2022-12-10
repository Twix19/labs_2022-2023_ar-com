---
## Front matter
title: "Отчёт по лабораторной работе №5"
subtitle: "Дисциплина: Архитектура Вычислительных Систем"
author: "Дедова Виктория Сергеевна"

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

Приобретение практических навыков работы в Midnight Commander. Освоение инструкций языка ассемблера mov и int.


# 5.3 Выполнение лабораторной работы

Открываем терминал и открываем Midnight Commander с помощью команды mc
![picture1](/home/vsdedova/Pictures/Screenshots/1.png)
Создайте папку lab06 и  заходим в созданный каталог, создаем файл lab6-1.asm.
![picture2](/home/vsdedova/Pictures/Screenshots/2.png)
Oткрываем файл lab6-1.asm для редактирования во встроенном редакторе.Ввjlbv текст программы из листинга 6.1, сохраняем изменения и закрываем файл.
![picture3](/home/vsdedova/Pictures/Screenshots/3.png)
Оттранслируем текст программы lab6-1.asm в объектный файл. Выполняем компоновку объектного файла и запускаем получившийся исполняемый файл. Программа выводит строку 'Введите строку:' и ожидает ввода с клавиатуры. На запрос вводим Наше ФИО.
![picture4](/home/vsdedova/Pictures/Screenshots/4.png)
Скачиваем  файл in_out.asm со страницы курса в ТУИС. Подключаемый файл in_out.asm должен лежать в том же каталоге, что и
файл с программой, в которой он используется.
![p5](/home/vsdedova/Pictures/Screenshots/5.png)
![p6](/home/vsdedova/Pictures/Screenshots/6.png)
С помощью функциональной клавиши F6 создаём копию файла lab6-1.asm с именем lab6-2.asm. 
![p7](/home/vsdedova/Pictures/Screenshots/7.png)
Исправляем текст программы в файле lab6-2.asm с использование подпрограмм из внешнего файла in_out.asm в соответствии с листингом 6.2. Создайте исполняемый файл и проверьте его работу.
![p8](/home/vsdedova/Pictures/Screenshots/8.png)
![p9](/home/vsdedova/Pictures/Screenshots/9.png)
![p10](/home/vsdedova/Pictures/Screenshots/10.png)
 В файле lab6-2.asm заменяем подпрограмму sprintLF на sprint. Создаём исполняемый файл и проверяем его работу.
 ![p12](/home/vsdedova/Pictures/Screenshots/12.png)
![p11](/home/vsdedova/Pictures/Screenshots/11.png)
sprintLF строку для ввода переносит вниз, а sprint на той же строке,где и выводится "Введите строку"


# 5.4. Задание для самостоятельной работы

Создаём копию файла lab6-1.asm. Вносим изменения в программу (без
использования внешнего файла in_out.asm).Получаем исполняемый файл и проверяем его работу. На приглашение
ввести строку вводим свою фамилию.
![p14](/home/vsdedova/Pictures/Screenshots/14.png)
![p13](/home/vsdedova/Pictures/Screenshots/13.png)
![p15](/home/vsdedova/Pictures/Screenshots/15.png)
Создаём копию файла lab6-2.asm. Исправляем текст программы с использованием подпрограмм из внешнего файла in_out.asm.Создаём исполняемый файл и проверяем его работу.
![p16](/home/vsdedova/Pictures/Screenshots/16.png)
![p17](/home/vsdedova/Pictures/Screenshots/17.png)


# Выводы

На данной лабораторной работе я приобрела навыки работы в Midnight Commander.



::: {#refs}
:::
