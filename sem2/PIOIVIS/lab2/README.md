# Лабораторная работа №2 по дисциплине "Представление и обработка информации в интеллектуальных системах"

## Цель
Разработать библиотеку для работы со структурой данных множество на любом императивнойм языке программирования (Pascal, C\C++, Java, C#, Python и др.)

Разработать тестовую программу, которая демонстрирует работоспособность реализованной библиотеки работы со структурой данных.

Разработать систему тестов, которые продемонстрировали бы работоспособность реализованной библиотеки. Система тестов должна отвечать требованиям полноты, адекватности и непротиворечивости.

Система тестов должна учитывать не только корректную работу на правильных данных, но и предусматривать корректное завершение программы в случае некорректных данных.
## Задание
- Реализовать программу, формирующую без повторений всевозможные ориентированные
множества из элементов исходного неориентированного множества, количество
элементов в сформированных множествах должно быть равно исходному натуральному n.

## Список понятий
* Множество – простейшая информационная конструкция и математическая структура, позволяющая рассматривать какие-то объекты как целое, связывая их.
* Объекты, связываемые некоторым множеством, называются элементами этого множества.
* Неориентированное множество  - это объект, представляющий собой совокупность вершин и ребер, где каждое ребро соединяет две вершины, не имея определенного направления.
* Ориентированное множество - это объект, состоящий из множества вершин и множества ориентированных ребер, которые указывают направление связи между вершинами.


## Алгоритм

1. Запросить у пользователя количество элементов множества и сохранить значение в переменной n.
2. Создать множество myset типа UnorderedSet.
3. Вызвать функцию creating(myset), которая запрашивает у пользователя элементы множества и сохраняет их в myset.  Функция creating(myset) определена следующим образом:
* Запросить у пользователя элементы множества до тех пор, пока не будет введено значение "q".
* Добавлять каждый введенный элемент в множество myset.set.
4. Вызвать функцию building(myset, n), которая генерирует и выводит на экран все возможные перестановки элементов множества myset.set из n элементов. Функция building(myset, n) определена следующим образом:
* Получить список элементов множества myset.set в виде вектора elements.
* Отсортировать вектор elements.
* Генерировать и выводить на экран все возможные перестановки элементов вектора elements, состоящие из n элементов, используя функцию next_permutation().
* Повторять до тех пор, пока все перестановки не будут сгенерированы.

## Тесты

### Тест 1
Количество элементов:
> 3  

Сами элементы: 
> {3,4,5,6} 7 8

Результат: 
<img src =https://github.com/iit-22170x/RPIIS/blob/%D0%93%D1%80%D0%B8%D0%BD%D1%8C_%D0%9D_%D0%90/sem2/lab2/img/2023-04-16_23-15-01.png >

### Тест 2
Количество элементов:
> 4

Сами элементы: 
> <1,2,3> 4 5 6 
 
 Результат: 

<img src =https://github.com/iit-22170x/RPIIS/blob/%D0%93%D1%80%D0%B8%D0%BD%D1%8C_%D0%9D_%D0%90/sem2/lab2/img/2023-04-16_23-21-16.png >


### Тест 3
Количество элементов:
> 3  

Сами элементы: 
> A2 7 b

Результат: 

<img src =https://github.com/iit-22170x/RPIIS/blob/%D0%93%D1%80%D0%B8%D0%BD%D1%8C_%D0%9D_%D0%90/sem2/lab2/img/2023-04-16_23-21-49.png>

### Тест 4
Количество элементов:
> 2

Сами элементы: 
> lol 88

Результат:
<img src =https://github.com/iit-22170x/RPIIS/blob/%D0%93%D1%80%D0%B8%D0%BD%D1%8C_%D0%9D_%D0%90/sem2/lab2/img/2023-04-16_23-22-14.png>

### Тест 5
Количество элементов:
> 4

Сами элементы: 
> a1 a2 a3  <a3,a4,a5>
 
 Результат: 
<img src =https://github.com/iit-22170x/RPIIS/blob/%D0%93%D1%80%D0%B8%D0%BD%D1%8C_%D0%9D_%D0%90/sem2/lab2/img/2023-04-16_23-22-47.png >

### Тест 6 7
Тесты с пустыми множествами

 Результат: 

<img src =https://github.com/iit-22170x/RPIIS/blob/%D0%93%D1%80%D0%B8%D0%BD%D1%8C_%D0%9D_%D0%90/sem2/lab2/img/2023-04-25_00-18-26.png >

### Тест 8
Тест c повторяющимися множествами

 Результат: 

<img src =https://github.com/iit-22170x/RPIIS/blob/%D0%93%D1%80%D0%B8%D0%BD%D1%8C_%D0%9D_%D0%90/sem2/lab2/img/2023-04-25_00-45-28.png >


## Вывод
В рамках данной лабораторной работы я научился работать со множествами, систематизировал и обобщил материал курса по дискретной математике, улучшил навыки работы с кодом на языке С++.

## Список использованных источников:
1. Дискретная математика для программистов / Ф.А. Новиков – СПб:
Питер, 2000. – 304 с.
2. Основы с++ программирование для начинающих: https://www.youtube.com/playlist?list=PLQOaTSbfxUtCrKs0nicOg2npJQYSPGO9r