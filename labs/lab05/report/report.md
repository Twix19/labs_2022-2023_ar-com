---
## Front matter
title: "Отчет по лабораторной №4"
subtitle: "Дисциплина:Архитектура компьютера"
author: "Дедова Виктория Сергеевна"
## Generic otions
lang: ru-RU
## Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl
## Pdf output format
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
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---
# 1.Цель работы
Освоение процедуры компиляции и сборки программ, написанных на ассем-
блере NASM
# 2.Выполнение лабораторной работы
Создаём кталог для работы с программами на языке ассемблера NASM и переходим в созданный каталог:
![1picture](/home/vsdedova/Pictures/1.png)
Создаём текстовый файл с именем hello.asm и открываем с помощью текстового редактора gedit:
![2picture](/home/vsdedova/Pictures/2.png)
![3picture](/home/vsdedova/Pictures/3.png)
Для компиляции текста,необходимо написать следующий текст и использовать команду ls:
![4picture](/home/vsdedova/Pictures/3.jpg)
Компилируем исходный файл hello.asm в obj.o(-o) и создаём файл листинга list.lst и проверяем,что файлы были созданы:
![5pictures](/home/vsdedova/Pictures/4.jpg)
Для того,чтобы получить исполняемую программу,файл передаем на обработку комповщику и прроверяем,что файл был создан:
![6picture](/home/vsdedova/Pictures/14.jpg)
Запускаем на выполнение созданный исполняемый файл:
![7pictures](/home/vsdedova/Pictures/7.jpg)
Задания для самостоятельной работы:
Создаем копию файла hello.asm с именем lab5.asm:
![8](/home/vsdedova/Pictures/8.jpg)
С помощью текстового редактора gedit, чтобы на экран выводилась строка с собственным именем и фамилией:
![9](/home/vsdedova/Pictures/9.jpg)
![10](/home/vsdedova/Pictures/10.jpg)
Оттранслируйем полученный текст программы lab5.asm в объектный
файл. Выполним компоновку объектного файла и запустим получившийся исполняемый файл.
![11](/home/vsdedova/Pictures/11.jpg)
Копируем файлы hello.asm и lab5.asm в локальный репозиторий
в каталог ~/work/study/2022-2023/"Архитектура компьютера"/arch-pc/labs/lab05/. Загружаем файлы на Github.
![12](/home/vsdedova/Pictures/12.jpg)
# 3.Выводы
На данной лабораторной мы освоили процедуры компиляции и сборки программ, написанных на ассем-
блере NASM.


::: {#refs}
:::
