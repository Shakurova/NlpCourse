# NLP_course
Here will be homeworks for Natural Language Processing course at NRU HSE

<b>HW 2</b>

1. Взять набор данных – выборку из корпуса про судебные разбирательства. На основании этих данных выделить наиболее типичные для суда действия (словосочетания типа принять решение), применив два различных метода.

Методы могут различаться:

* выбором двух разных метрик;
* выбором разных ограничений на части речи и ширину окна (сравнить один и тот же метод при разных ограничениях);

... либо вы выбираете метод и ограничения, смотрите на результат и предлагаете какие-то эвристики, которые позволяют улучшить результат.

2. Для оценки результата:
    Пользуясь словарями, интуицией и т.п. составляете золотой стандарт – ранжированный топ 10 коллокаций.
    Смотрите, какую позицию занимают коллокации из золотого стандарта среди списка, отранжированного по мере коллокационной связи.
    Считаете меру качества – ранговый коэффициент корреляции Спирмена между двумя списками.

Итогом работы является скрипт на питоне, который либо использует nltk, либо вами вручную написанную функцию для подсчета коллокационной метрики. В конце скрипта нужно приписать вывод, в котором вы пишете, что вы сделали: какие методы использовали, какой результат получили и что вы об этом думаете. 

<b>HW 3</b>

1. Возьмите два небольших корпуса (можно взять "Анну Каренину" и сонеты Шекспира). Напишите программу, которая наглядно демонстрирует ответ на вопрос: можно ли различить предложения этих двух текстов, пользуясь лишь следующими признаками:

* длина предложения в буквах,
* число различных букв в предложении,
* число гласных в предложении,
* медиана числа букв в слове,
* медиана числа гласных в слове.

Для этого превратите каждое предолжение в список соответствующих чисел. Выведите на экран распределение данных по предложениям по двум осям, дающим наилучшее разделение (пара осей для обоих текстов должна быть одинаковой).

2. Взять признаки из предыдущего задания и построить классификатор, который пытался бы угадать, к какому корпусу относится предложение с определенным набором признаков. Привести 3 примера, где классификатор ошибается.

<b>HW 4</b>

1) Найти все значения (синсеты) для лексемы plant
2) Найти определение для лексемы plant в значении (а) "завод" и в значении (b) "растение"
3) Найдите два произвольных контекста для слова plant в значениях (a) "завод" и (b) "растение"; продемонстрируйте на них действие алгоритма Леска для разрешения неоднозначности
4) Найдите гиперонимы для значения (a) и гиперонимы для значения (b)
5) Вычислите наименьшее расстояние между значением plant "завод" и значениями лексемы industry, а также plant "растение" и значениями лексемы leaf
Найти min (d(plant: "завод", industry), d(plant: "завод", leaf)), а также min (d(plant: "растение", industry), d(plant: "растение", leaf))
6) Вычислить двумя разными способами расстояние:
d(plant: "растение", rattlesnake's master) и d(organism, whole)

Есть ли разница в расстояниях? Какое из расстояний, по Вашему мнению, в лучшей степени отражает интуитивное представление о семантчиеской близости слов?
