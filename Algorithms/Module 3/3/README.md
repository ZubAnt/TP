# Задача 3. Декартово дерево (4 балла)
Дано число `N < 10^6`​ и последовательность пар целых чисел из `[-2^31​ .. 2^ 31​]` длиной `N`. Построить декартово дерево
из `N` узлов, характеризующихся парами чисел `{X[i]​ , Y[i]​}`. Каждая пара чисел `{X​[i​], Y​[i] }` определяет ключ `X​[i]`​ и
приоритет `Y​[i]`​ в декартовом дереве.
Добавление узла в декартово дерево выполняйте второй версией алгоритма, рассказанного на лекции:

* При добавлении узла `(x, y)` выполняйте спуск по ключу до узла `P` с меньшим приоритетом. Затем разбейте найденное
поддерево по ключу `x` так, чтобы в первом поддереве все ключи меньше `x`, а во втором больше или равны `x`.
Получившиеся два дерева сделайте дочерними для нового узла `(x, y)`. Новый узел вставьте на место узла `P`.

Построить также наивное дерево поиска по ключам `X​[i]`​ методом из задачи 2.

**Вычислить разницу глубин наивного дерева поиска и декартового дерева. Разница может быть отрицательна.**

| in | out |
|----|-----|
|10<br>5 11<br>18 8<br>25 7<br>50 12<br>30 30<br>15 15<br>20 10<br>22 5<br>40 20<br>45 9 | 2 |
|10<br>38 19<br>37 5<br>47 15<br>35 0<br>12 3<br>0 42<br>31 37<br>21 45<br>30 26<br>41 6 | 2 |