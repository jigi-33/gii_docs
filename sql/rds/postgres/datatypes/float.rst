Числа с плавающей точкой
========================

.. code-block:: sql

    0.1::real * 10 = 1.0::real
    -------
    false  -- значения хранятся не точно


real
----

4 байта, 6 десятичных цифр


float, double precision
-----------------------

8 байт, 15 десятичных цифр


numeric, decimal
----------------

131072 цифр до десятичной точки и 16383 после

numeric(n) - целые числа до n цифр
numeric(n, m) - вещественные числа до n цифр, из них m после десятичной точки


Функции
-------

div
+++

Целочисленное деление

.. code-block:: sql

    div(7.0, 2.0)
    ---
    3

mod
+++

Остаток от деления

.. code-block:: sql

    mod(7, 2)
    ---
    1

.. code-block:: sql

    7 % 2
    ---
    1

power
+++++

Возведение в степень

.. code-block:: sql

    power(2, 3)
    ---
    8

.. code-block:: sql

    2 ** 3
    ---
    8


abs
+++

Абсолютное значение

.. code-block:: sql

    abs(-2.7)
    ---
    2.7

sign
++++

Знак

.. code-block:: sql

    sign(-2.7), sign(0), sign(2.7)
    ---
    -1, 0, 1

trunc, ceil, ceiling, round, floor
++++++++++++++++++++++++++++++++++

Округление

.. code-block:: sql

    trunc(-2.7), ceil(-2.7), round(-2.7), floor(-2.7)
    ---
    -2, -2, -3, -3

.. code-block:: sql

    trunc(2.7), ceil(2.7), round(2.7), floor(2.7)
    ---
    2, 3, 3, 2

to_number
+++++++++

Приведение строки к числу

* 9 - цифра
* . - (точка) - десятичная точка
* , - (запятая) - разделитель разрядов
* MI - минус (<0)
* 0 - цифра с ведущим нулем
* D - точка или запятая из локали
* G - разделитель разрядов из локали
* PL - плюс (>0)
* SG - плюс или минус

.. code-block::sql

    to_number('3,1416', '99D00')
    , to_number('3,1416', '99D000000')
    , to_number('123,45', '99D000000')
    ---
    3.14
    , 3.1416
    , numeric field overflow
