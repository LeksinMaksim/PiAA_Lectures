# Что такое класс P?

 P - класс задач, решаемых за полиномиальное время (от размера входа). Примеры таких задач: задача о существовании пути в графе, задача о взаимно простых числах и тп

# Что такое полиномиальное время?

Говорят, что алгоритм работает за полиномиальное время, если время работы ограничено сверху многочленом от размера входа алгоритма, те $T(n)=O(n^k)$ для некоторой константы k.

Примеры задач: целочисленное сложение, умножение, деление, взятие остатка от деления, умножение матриц, выяснение связности графов, сортировка множества из n чисел, нахождение эйлерова цикла на графе из m ребер, обнаружение в тексте длиной n некоторого слова, построение мод.

# Что такое класс NP?

NP - класс задач, верифицируемых (проверяемых) за полиномиальное время. Те класс задач, решение которых можно проверить за полиномиальное время на недетерминированной машине Тьюринга. 

ДМТ - абстрактный вычислитель, который имеет четко определенное поведение на каждом шаге. НДМТ - для каждой комбинации текущего состояния и символа может быть несколько допустимых переходов, те нет определенного поведения.

Примеры задач: задача о выполнимости булевой формулы, задача о вершинном покрытии, задача о клике и тп.

# Как доказать, что задача принадлежит классу NP?

- Привести алгоритм решения задачи, работающий полиномиальное время на недетерминированной машине Тьюринга
или
- Описать сертификат и привести алгоритм верификации, работающий полиномиальное время на детерминированной машине Тьюринга 

Сертификат - доп информация, позволяющая быстро решить задачу. Важно помнить, что размер сертификата должен быть полиномиален относительно размера самой задачи.

Алгоритм верификации - принимает на вход экземпляр задачи и сертификат в нему, возвращает ответ к задаче (0 или 1).

Грубо говоря, к классу NP относятся те задачи, правильность решения которых можно проверить быстро (за полиномиальное время). К классу P относятся те задачи, которые можно быстро решить.