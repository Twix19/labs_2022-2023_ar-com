---
## Front matter
title: "Лабораторная работа № 6"
subtitle: "Дисциплина: Архитектура компьютера"
author: "Дедова Виктория Сергеевна"



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

Освоение арифметических инструкций языка ассемблера NASM.                                                                                                         |

# Выполнение лабораторной работы

Создайте каталог для программам лабораторной работы No 7, перейдите в
него и создайте файл lab7-1.asm:

![1](/home/vsdedova/Pictures/Screenshots/1.png)

Рассмотрим примеры программ вывода символьных и численных значе-
ний. Программы будут выводить значения записанные в регистр eax.
Вводим в файл lab7-1.asm текст программы из листинга 7.1
![2](/home/vsdedova/Pictures/Screenshots/2.png)
Создаём исполняемый файл и запускаем  его.
![3](/home/vsdedova/Pictures/Screenshots/3.png)
![3](/home/vsdedova/Pictures/Screenshots/3(1).png)
![3](/home/vsdedova/Pictures/Screenshots/3(2).png)
![3](/home/vsdedova/Pictures/Screenshots/4.png)
Далее изменим текст программы и вместо символов, запишем в реги-
стры числа, mov eax,'6' mov ebx,'4' на строки mov eax,6 mov ebx,4
![4](/home/vsdedova/Pictures/Screenshots/4(1).png)
![4](/home/vsdedova/Pictures/Screenshots/4(1).png)

Код 10 соответствует символу переходу строки.
![4](/home/vsdedova/Pictures/Screenshots/4(4).png)
Создаём файл lab7-2.asm в каталоге ~/work/arch-pc/lab07 и вводим в него
текст программы из листинга 7.2. 
![5(1)](/home/vsdedova/Pictures/Screenshots/5.png)
В результате работы программы получаем 106.
![5](/home/vsdedova/Pictures/Screenshots/6.png)
Замените строки mov eax,'6' mov ebx,'4' на строки mov eax,6 mov ebx,4
Создаём исполняемый файл и запускаем его. 
![7](/home/vsdedova/Pictures/Screenshots/7.png)
Результат будет 10.
Заменяем функцию iprintLF на iprint. Создаёте исполняемый файл и запу-
стите его.
![7](/home/vsdedova/Pictures/Screenshots/7(intr).png)
![7(1)](/home/vsdedova/Pictures/Screenshots/7(intrit).png)
Вывод функций отличается переходом на другую строку.

Приведем программу вычисления арифметического выражения 𝑓(𝑥) = (5 ∗ 2 + 3)/3.
Создаём файл lab7-3.asm в каталоге ~/work/arch-pc/lab07 и вводим текст листинга 7.3.ьщ
![8](/home/vsdedova/Pictures/Screenshots/8.png)
![9](/home/vsdedova/Pictures/Screenshots/9.png)
Измените текст программы для вычисления выражения 𝑓(𝑥) = (4 ∗ 6 + 2)/5.
Создаём исполняемый файл и проверяем его работу.
![10](/home/vsdedova/Pictures/Screenshots/10.png)
Создаём файл variant.asm. вводим текст из листинга 7.4.
![11](/home/vsdedova/Pictures/Screenshots/11.png)
![12](/home/vsdedova/Pictures/Screenshots/12.png)
Вопросы:
1. mov eax and rem call sprint
2. mov ecx,x-запись входной переменной в регистр ecx; mov edx,80 -запись размера переменной в регистре edx;
call sread-вызов процедуры чтения даннных.
3.call atoi - функция преобразующая ASCII код символа в целое число и записывающая результат в регистр eax
4.xor edx,edx mov ebx,20 div ebx, inc edx.
5.div ebx-ebx
6.inc- используется для увеличения операнда на единицу
7.mov eax,rem call sprint mov eax,edx call iprintLV
 
#Задание для самостоятельной работы

Напишем программу вычисления выражения 𝑦 = 𝑓(𝑥). Программа должна
выводить выражение для вычисления, выводить запрос на ввод значения
𝑥, вычислять заданное выражение в зависимости от введенного 𝑥, выво-
дить результат вычислений. Вид функции 𝑓(𝑥) выбрать из таблицы 6.3
вариантов заданий в соответствии с номером полученным при выполне-
нии лабораторной работы. Создаём исполняемый файл и проверьте его
работу для значений 𝑥1 и 𝑥2 из 6.3
![13](/home/vsdedova/Pictures/Screenshots/13.png)
![14](/home/vsdedova/Pictures/Screenshots/14.png)
![15](/home/vsdedova/Pictures/Screenshots/15.png)






# Выводы
На данной лабораторной работе мы освоили арифметические инструкции языка ассемблера NASM



::: {#refs}
:::
