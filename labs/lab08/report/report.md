---
## Front matter
title: "Лабораторная работа №8"
author: "Гэинэ Андрей"

## Generic otions
lang: ru-RU
toc-title: "Содержание"

## Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

## Pdf output format
toc: true # Table of contents
toc-depth: 2
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

Познакомиться с операционной системой Linux. Получить практические навыки работы с редактором vi, установленным по умолчанию практически во всех дистрибутивах.

# Задание

1. Ознакомиться с теоретическим материалом.
2. Ознакомиться с редактором vi.
3. Выполнить упражнения, используя команды vi


# Ход работы

Задание 1. Создание нового файла с использованием vi
1. Создайте каталог с именем ~/work/os/lab06.
2. Перейдите во вновь созданный каталог.
3. Вызовите vi и создайте файл hello.sh

![Рис.1](image\picture1.png)

4. Нажмите клавишу i и вводите следующий текст.
  1 #!/bin/bash
  2 HELL=Hello
  3 function hello {
  4 LOCAL HELLO=World
  5 echo $HELLO
  6 }
  7 echo $HELLO
  8 hello

5. Нажмите клавишу Esc для перехода в командный режим после завершения ввода
текста.
6. Нажмите : для перехода в режим последней строки и внизу вашего экрана появится
приглашение в виде двоеточия.
7. Нажмите w (записать) и q (выйти), а затем нажмите клавишу Enter для сохранения
вашего текста и завершения работы.

![Рис.2](image\picture2.png)

8. Сделайте файл исполняемым

![Рис.3](image\picture3.png)

Задание 2. Редактирование существующего файла
1. Вызовите vi на редактирование файла

![Рис.4](image\picture1.png)

2. Установите курсор в конец слова HELL второй строки.
3. Перейдите в режим вставки и замените на HELLO. Нажмите Esc для возврата в командный режим.
4. Установите курсор на четвертую строку и сотрите слово LOCAL.
5. Перейдите в режим вставки и наберите следующий текст: local, нажмите Esc для
возврата в командный режим.
6. Установите курсор на последней строке файла. Вставьте после неё строку, содержащую
следующий текст: echo $HELLO.
7. Нажмите Esc для перехода в командный режим.
8. Удалите последнюю строку.
9. Введите команду отмены изменений u для отмены последней команды.
10. Введите символ : для перехода в режим последней строки. Запишите произведённые
изменения и выйдите из vi.

![Рис.5](image\picture4.png)

# Выводы

Благодаря данной работе мы научились работать с коммандами vi.

# Контрольные вопросы

1. Дайте краткую характеристику режимам работы редактора vi.

Lorem ipsum dolor sit amet, consectetur adipiscing elit,

2. Как выйти из редактора, не сохраняя произведённые изменения?

sed do eiusmod tempor incididunt ut labore et dolore magna aliqua

3. Назовите и дайте краткую характеристику командам позиционирования.

Ut enim ad minim veniam, quis nostrud exercitation ullamco

4. Что для редактора vi является словом?

laboris nisi ut aliquip ex ea commodo consequat. Duis aute

5. Каким образом из любого места редактируемого файла перейти в начало (конец)
файла?

irure dolor in reprehenderit in voluptate velit

6. Назовите и дайте краткую характеристику основным группам команд редактирования.

esse cillum dolore eu fugiat nulla pariatur

7. Необходимо заполнить строку символами $. Каковы ваши действия?

Excepteur sint occaecat cupidatat non proident, sunt in culpa

8. Как отменить некорректное действие, связанное с процессом редактирования?

qui officia deserunt mollit anim id est laborum.

9. Назовите и дайте характеристику основным группам команд режима последней строки.

Lorem ipsum dolor sit amet, consectetur adipiscing elit,

10. Как определить, не перемещая курсора, позицию, в которой заканчивается строка?

sed do eiusmod tempor incididunt ut labore et dolore magna a

11. Выполните анализ опций редактора vi (сколько их, как узнать их назначение и т.д.).

Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris n

12. Как определить режим работы редактора vi?

aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. 

13. Постройте граф взаимосвязи режимов работы редактора vi

Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.