# Темы:
1) Комплексные числа.
2) Системы линейных уравнений. Приведение к ступенчатому виду. 
3) Метод Гаусса
4) Подстановки.
5) Матрицы. Теория определителей

---
# 1. Комплексные числа.

==Определение== Комплексным числом называется выражение ${z = a + bi}$, где ${a}$ и ${b \in \mathbb{R}, \ i \in \mathbb{C}}$. Число ${a}$ называется действительной частью (${\mathrm{Re} \ z}$), а ${b}$ - мнимой частью (${\mathrm{Im} \ z}$).

Комплексная плоскость состоит из двух осей:
1. ${\mathrm{Re} \ z}$ - действительная ось (абсцисс)
2. ${\mathrm{Im} \ z}$ - мнимая ось (ординат)

Действительные числа - частный случай комплексных числе. В более строгом виде - ${\mathbb{R} }$ является подмножеством множества ${\mathbb{C}}$.

---
==Алгебраическая форма комплексного числа. Сложение, вычитание, умножение и деление комплексных чисел.==
Алгебраическая форма - ${z = a + bi}$.

### Сложить два комплексных числа.
$$\displaylines{
z_{1} = 1+3i, \  z_{2} = 4-5i\\
\text{ Для того чтобы их сложить, нужно сложить их действительные и мнимые части.} \\
z_{1}+z_{2} = 1+4+3i-5i = \boxed{5-2i} \\
\\
\text{ Также выполняется коммутативность: } \\
z_{1}+z_{2} = z_{2}+z_{1}
}$$
### Найти разность двух комплексных чисел:
$$\displaylines{
z_{1} = -2+i, \  z_{2} = \sqrt{ 3 }+5i \\
\text{ Аналогично сложению, только не забыть скобки. } \\
z_{1}-z_{2} = -2+i -(\sqrt{ 3 } +5i) = -2-\sqrt{ 3 }+i-5i = \boxed{-2-\sqrt{ 3 } -4i}
}$$
### Умножение комплексных чисел.
$$\displaylines{
\boxed{i^{ 2 } = -1}
}$$
Пример. Найти произведение комплексных чисел.
$$\displaylines{
z_{1} = 1-i, \  z_{2} = 3+6i \\
z_{1}\cdot z_{2} = (1-i)(3+6i) = 1 \cdot 3 + 1\cdot  6i -i\cdot 3 -i\cdot 6i = 3+6i-3i \underbrace{ -6i^{ 2 } }_{ -6\cdot (-1) \ = \ +6 } =9+3i 
}$$
### Деление комплексных чисел.
Деление чисел осуществляется методом умножения знаменателя и числителя на сопряженное знаменателю число.

$$\displaylines{
z_{1} = 13+i, \ z_{2}=7-6i\\
\frac{z_{1}}{z_{2}} = \frac{(13+i)\cdot (7+6i)}{(7-6i)\cdot (7+6i)} = \frac{91+7i+78i+6i^{ 2 }}{7^{ 2 }-(6i)^{ 2 }} = \frac{85+85i}{85} = \boxed{1+i}
}$$

---
### **Тригонометрическая форма.**
Любое комплексное число (кроме нуля) вида ${z = a+bi}$ можно записать в тригонометрический форме:
$$\displaylines{
z = |z| \cdot (\cos{(\varphi)} + i\sin{(\varphi)}) - \text{ где } |z| - \text{ модуль, а } \varphi - \text{ аргумент к. числа }
}$$
**Модулем** комплексного числа называется расстояние от начала координат до соответствующей точки комплексной плоскости. Попросту говоря, модуль – это длина радиус-вектора.
$$\displaylines{
|z| = \sqrt{ a^{ 2 }+b^{ 2 } }, \  \forall{ \ a, \ b}
}$$
**Аргументом** комплексного числа называется угол ${\varphi}$ между положительной полуосью действительной оси и радиус-вектором. Аргумент не определен для единственного числа ${z = 0}$.

Формула ${\varphi = \arg z}$ для правой полуплоскости:
$$\displaylines{
\arg z = \arctan{\left( \frac{b}{a} \right)}
}$$
2 координатная четверть:
$$\displaylines{
\arg z = \pi + \arctan{\left( \frac{b}{a} \right)}
}$$
3 координатная четверть:
$$\displaylines{
\arg z = -\pi + \arctan{\left( \frac{b}{a} \right)}
}$$
---
### Возведение комплексного числа в степень.

Формула Муавра. Если ${z}$ представлено в тригонометрической форме, то при его возведении в степень справедлива формула:
$$\displaylines{
z^{ n } = |z|^{ n } \cdot (\cos{(n\cdot \varphi)+i\sin{(n \cdot \varphi)}})
}$$
---
### Корни из комплексных чисел.

Для вычисления корней комплексных чисел используется их представление в тригонометрической (или показательной) форме. Комплексное число $z = a + bi$ можно записать как:

$$
z = r \left( \cos \theta + i \sin \theta \right),
$$

где $r = |z| = \sqrt{a^2 + b^2}$ — модуль числа, а $\theta = \arg(z)$ — его аргумент, который можно найти как $\theta = \arctan\left( \frac{b}{a} \right)$.

Корень квадратный от комплексного числа $z$ равен:

$$
\sqrt{z} = \sqrt{r} \left( \cos \frac{\theta}{2} + i \sin \frac{\theta}{2} \right).
$$

Пример: Найдём $\sqrt{1 + i}$.

1. Определим $r = |z| = \sqrt{1^2 + 1^2} = \sqrt{2}$.
2. Определим аргумент $\theta = \tan^{-1} \left( \frac{1}{1} \right) = \frac{\pi}{4}$.

Тогда

$$
\sqrt{1 + i} = \sqrt{\sqrt{2}} \left( \cos \frac{\pi}{8} + i \sin \frac{\pi}{8} \right).
$$

### Корень $n$-ой степени от комплексного числа

Корень $n$-ой степени от $z$ можно вычислить по следующей формуле:

$$
\sqrt[n]{z} = \sqrt[n]{r} \left( \cos \frac{\theta + 2\pi k}{n} + i \sin \frac{\theta + 2\pi k}{n} \right),
$$

где $k = 0, 1, 2, \dots, n-1$. Эта формула даёт $n$ различных значений (корней) комплексного числа.

Пример: Найдём $\sqrt[3]{8}$.

1. Переведём $z = 8$ в тригонометрическую форму: $r = |z| = 8$, $\theta = 0$.
2. Найдём корни с $k = 0, 1, 2$.

Для $k = 0$:

$$
\sqrt[3]{8} = \sqrt[3]{8} \left( \cos \frac{0}{3} + i \sin \frac{0}{3} \right) = 2.
$$

Для $k = 1$:

$$
\sqrt[3]{8} = \sqrt[3]{8} \left( \cos \frac{2\pi}{3} + i \sin \frac{2\pi}{3} \right) = 2 \left( -\frac{1}{2} + i \frac{\sqrt{3}}{2} \right) = -1 + i \sqrt{3}.
$$

Для $k = 2$:

$$
\sqrt[3]{8} = \sqrt[3]{8} \left( \cos \frac{4\pi}{3} + i \sin \frac{4\pi}{3} \right) = 2 \left( -\frac{1}{2} - i \frac{\sqrt{3}}{2} \right) = -1 - i \sqrt{3}.
$$

Итак, корни третьей степени от $8$ — это $2$, $-1 + i \sqrt{3}$ и $-1 - i \sqrt{3}$.

---
### Формула Эйлера для комплексных чисел

Формула Эйлера — это фундаментальная формула в комплексном анализе, которая связывает комплексные числа с тригонометрическими функциями. Формула имеет вид:

$$
e^{i\theta} = \cos \theta + i \sin \theta,
$$

где $e$ — основание натурального логарифма, $i$ — мнимая единица, а $\theta$ — угол в радианах. 

Эта формула позволяет представлять комплексные числа в показательной форме. Для комплексного числа $z = r (\cos \theta + i \sin \theta)$, где $r = |z|$ — модуль числа, можно записать:

$$
z = r e^{i\theta}.
$$

#### Пример использования формулы Эйлера

Пусть $z = 1 + i$. Найдём модуль и аргумент числа $z$.

1. Модуль: $r = |z| = \sqrt{1^2 + 1^2} = \sqrt{2}$.
2. Аргумент: $\theta = \arg(z) = \tan^{-1} \left(\frac{1}{1}\right) = \frac{\pi}{4}$.

Теперь мы можем записать $z$ в показательной форме с использованием формулы Эйлера:

$$
z = \sqrt{2} e^{i \frac{\pi}{4}}.
$$

### Первообразный корень $n$-й степени из $1$

Первообразные корни $n$-й степени из $1$ — это комплексные числа, которые при возведении в степень $n$ дают $1$, но не дают $1$ при возведении в степень, меньшую $n$.

Корни $n$-й степени из $1$ находятся по формуле:

$$
\omega_k = e^{i \frac{2 \pi k}{n}},
$$

где $k = 0, 1, 2, \dots, n-1$. Здесь $\omega_k$ представляют собой $n$ различных корней $n$-й степени из $1$.

Первообразный корень $n$-й степени из $1$ — это корень, порождающий все остальные корни. Обычно выбирают $\omega = e^{i \frac{2 \pi}{n}}$ как первообразный корень. Все остальные корни могут быть получены как степени этого первообразного корня: $\omega, \omega^2, \dots, \omega^{n-1}$.

#### Пример: Кубические корни из $1$

Найдём кубические корни из $1$, т.е. $n = 3$. 

Формула для корней:

$$
\omega_k = e^{i \frac{2 \pi k}{3}}, \quad k = 0, 1, 2.
$$

1. Для $k = 0$:
   $$
   \omega_0 = e^{i \frac{2 \pi \cdot 0}{3}} = e^{i \cdot 0} = 1.
   $$

2. Для $k = 1$:
   $$
   \omega_1 = e^{i \frac{2 \pi \cdot 1}{3}} = e^{i \frac{2 \pi}{3}} = -\frac{1}{2} + i \frac{\sqrt{3}}{2}.
   $$

3. Для $k = 2$:
   $$
   \omega_2 = e^{i \frac{2 \pi \cdot 2}{3}} = e^{i \frac{4 \pi}{3}} = -\frac{1}{2} - i \frac{\sqrt{3}}{2}.
   $$

Таким образом, кубические корни из $1$ — это $1$, $-\frac{1}{2} + i \frac{\sqrt{3}}{2}$ и $-\frac{1}{2} - i \frac{\sqrt{3}}{2}$. Первообразный корень в этом случае — $\omega = e^{i \frac{2 \pi}{3}}$.

---
# 2. Системы линейных уравнений. Приведение к ступенчатому виду. 
Для решения системы линейных алгебраических уравнений (СЛАУ) часто используют метод приведения к ступенчатому виду. Этот метод основан на преобразовании системы уравнений так, чтобы упростить её решение. Ниже приведены основные шаги для приведения матрицы системы к ступенчатому виду.

### Теория: Приведение к ступенчатому виду

Пусть у нас есть система линейных уравнений:
$$
\begin{cases}
a_{11}x_1 + a_{12}x_2 + \dots + a_{1n}x_n = b_1, \\
a_{21}x_1 + a_{22}x_2 + \dots + a_{2n}x_n = b_2, \\
\vdots \\
a_{m1}x_1 + a_{m2}x_2 + \dots + a_{mn}x_n = b_m.
\end{cases}
$$

Эту систему можно записать в матричной форме как:
$$
AX = B,
$$
где $A$ — матрица коэффициентов, $X$ — столбец переменных, а $B$ — столбец свободных членов.

Для приведения матрицы $A$ к ступенчатому виду выполняются следующие шаги.

### 1. Выбор ведущего элемента

Начинаем с первого столбца и находим в нём первый ненулевой элемент, который станет ведущим элементом. Если в первом столбце все элементы равны нулю, переходим ко второму столбцу и так далее.

### 2. Преобразование строки с ведущим элементом

Если ведущий элемент находится не на первой позиции, строки переставляются так, чтобы ведущий элемент оказался на нужном месте. Далее, строка с ведущим элементом умножается на такое число, чтобы ведущий элемент стал равен $1$.

### 3. Обнуление элементов ниже ведущего

После того как ведущий элемент равен $1$, используем его для того, чтобы обнулить все элементы ниже него в том же столбце. Это делается путём вычитания из каждой нижней строки строки с ведущим элементом, умноженной на коэффициент, равный элементу в соответствующей строке и столбце.

### 4. Переход к следующему столбцу и повторение шагов

Переходим к следующему столбцу и повторяем шаги 1–3 для оставшейся части матрицы, начиная с подматрицы, образованной оставшимися строками и столбцами. Повторяем, пока не дойдём до последней строки.

### 5. Получение ступенчатого вида

В результате этих шагов матрица $A$ будет приведена к ступенчатому виду, где каждая строка начинается с нуля вплоть до первого ненулевого элемента, который расположен правее, чем в предыдущей строке. Такой вид матрицы позволяет легко находить решения системы уравнений методом обратной подстановки.

### Пример приведения к ступенчатому виду

Рассмотрим следующую систему уравнений:
$$
\begin{cases}
2x + 4y - 2z = 2, \\
4x + 9y - 3z = 8, \\
-2x + 3y + 7z = 10.
\end{cases}
$$

Запишем её в матричной форме:
$$
\begin{pmatrix}
2 & 4 & -2 & | & 2 \\
4 & 9 & -3 & | & 8 \\
-2 & 3 & 7 & | & 10 \\
\end{pmatrix}
$$

1. **Выбираем ведущий элемент** в первом столбце. Ведущий элемент — $4$ (второй строке). Поменяем первую и вторую строки местами:
   $$
   \begin{pmatrix}
   4 & 9 & -3 & | & 8 \\
   2 & 4 & -2 & | & 2 \\
   -2 & 3 & 7 & | & 10 \\
   \end{pmatrix}
   $$

2. **Делим первую строку на $4$**, чтобы сделать ведущий элемент равным $1$:
   $$
   \begin{pmatrix}
   1 & \frac{9}{4} & -\frac{3}{4} & | & 2 \\
   2 & 4 & -2 & | & 2 \\
   -2 & 3 & 7 & | & 10 \\
   \end{pmatrix}
   $$

3. **Обнуляем элементы ниже ведущего в первом столбце**. Для этого вычитаем из второй строки первую, умноженную на $2$, и прибавляем к третьей строке первую, умноженную на $2$:
   $$
   \begin{pmatrix}
   1 & \frac{9}{4} & -\frac{3}{4} & | & 2 \\
   0 & -\frac{1}{2} & -\frac{1}{2} & | & -2 \\
   0 & \frac{15}{2} & \frac{11}{2} & | & 14 \\
   \end{pmatrix}
   $$

4. Переходим ко второму столбцу. **Ведущий элемент** во второй строке — $-\frac{1}{2}$. Делим вторую строку на $-\frac{1}{2}$, чтобы сделать ведущий элемент равным $1$:
   $$
   \begin{pmatrix}
   1 & \frac{9}{4} & -\frac{3}{4} & | & 2 \\
   0 & 1 & 1 & | & 4 \\
   0 & \frac{15}{2} & \frac{11}{2} & | & 14 \\
   \end{pmatrix}
   $$

5. **Обнуляем элемент ниже ведущего** во втором столбце. Для этого из третьей строки вычитаем вторую, умноженную на $\frac{15}{2}$:
   $$
   \begin{pmatrix}
   1 & \frac{9}{4} & -\frac{3}{4} & | & 2 \\
   0 & 1 & 1 & | & 4 \\
   0 & 0 & -2 & | & -16 \\
   \end{pmatrix}
   $$

6. Переходим к третьей строке и третьему столбцу. Ведущий элемент — $-2$. **Делим третью строку на $-2$**:
   $$
   \begin{pmatrix}
   1 & \frac{9}{4} & -\frac{3}{4} & | & 2 \\
   0 & 1 & 1 & | & 4 \\
   0 & 0 & 1 & | & 8 \\
   \end{pmatrix}
   $$

Теперь система находится в ступенчатом виде, и её можно легко решить методом обратной подстановки:
1. Из третьего уравнения находим $z = 8$.
2. Подставляем $z$ во второе уравнение и находим $y = -4$.
3. Подставляем $y$ и $z$ в первое уравнение и находим $x = 3$.

Таким образом, решение системы:
$$
x = 3, \quad y = -4, \quad z = 8.
$$
---
# 3. Метод Гаусса

Метод Гаусса — это алгоритм для решения систем линейных уравнений, приведения матрицы к ступенчатому виду и нахождения её ранга. Этот метод основан на преобразовании системы уравнений с использованием элементарных операций над строками.

Рассмотрим систему линейных уравнений в матричной форме:
$$
AX = B,
$$
где $A$ — матрица коэффициентов, $X$ — вектор неизвестных, а $B$ — вектор свободных членов.

Цель метода Гаусса — привести матрицу $A$ к ступенчатому или треугольному виду, чтобы упростить решение системы.

### Основные шаги метода Гаусса

Метод Гаусса состоит из трёх типов элементарных операций над строками:

1. Перестановка строк.
2. Умножение строки на ненулевое число.
3. Прибавление к одной строке другой строки, умноженной на некоторое число.

С помощью этих операций мы приводим матрицу к ступенчатому виду, где каждая следующая строка начинается с нуля до тех пор, пока не встретится первый ненулевой элемент, который расположен правее, чем в предыдущей строке.

### Пошаговое описание метода Гаусса

1. **Выбор ведущего элемента**: Начинаем с первого столбца и находим первый ненулевой элемент (ведущий элемент). Если его нет, переходим к следующему столбцу.

2. **Приведение ведущего элемента к 1**: Делим строку, содержащую ведущий элемент, на значение этого элемента, чтобы сделать его равным $1$.

3. **Обнуление остальных элементов столбца**: Используем ведущий элемент для обнуления всех остальных элементов в его столбце, прибавляя или вычитая из других строк текущую строку, умноженную на подходящий коэффициент.

4. **Переход к следующей строке и столбцу**: Повторяем процесс для оставшихся строк и столбцов, пока не получим ступенчатый вид.

5. **Обратная подстановка**: Если необходимо, проводим обратную подстановку для нахождения решений системы.

### Пример метода Гаусса

Рассмотрим систему уравнений:
$$
\begin{cases}
x + y + z = 6, \\
2y + 5z = -4, \\
2x + 5y - z = 27.
\end{cases}
$$

1. Запишем эту систему в виде расширенной матрицы:
   $$
   \begin{pmatrix}
   1 & 1 & 1 & | & 6 \\
   0 & 2 & 5 & | & -4 \\
   2 & 5 & -1 & | & 27 \\
   \end{pmatrix}
   $$

2. **Приведём первый элемент в первой строке к 1**. Он уже равен $1$, поэтому переходим к следующему шагу.

3. **Обнулим элементы ниже первого элемента первого столбца**. Для этого:
   - Вычитаем из третьей строки первую, умноженную на $2$:
   $$
   \begin{pmatrix}
   1 & 1 & 1 & | & 6 \\
   0 & 2 & 5 & | & -4 \\
   0 & 3 & -3 & | & 15 \\
   \end{pmatrix}
   $$

4. **Переходим ко второму столбцу** и находим ведущий элемент во второй строке (он равен $2$). Делим вторую строку на $2$:
   $$
   \begin{pmatrix}
   1 & 1 & 1 & | & 6 \\
   0 & 1 & \frac{5}{2} & | & -2 \\
   0 & 3 & -3 & | & 15 \\
   \end{pmatrix}
   $$

5. **Обнуляем элемент ниже ведущего во втором столбце**. Для этого вычитаем из третьей строки вторую, умноженную на $3$:
   $$
   \begin{pmatrix}
   1 & 1 & 1 & | & 6 \\
   0 & 1 & \frac{5}{2} & | & -2 \\
   0 & 0 & -\frac{21}{2} & | & 21 \\
   \end{pmatrix}
   $$

6. **Переходим к третьей строке** и приводим ведущий элемент в третьем столбце к $1$, деля строку на $-\frac{21}{2}$:
   $$
   \begin{pmatrix}
   1 & 1 & 1 & | & 6 \\
   0 & 1 & \frac{5}{2} & | & -2 \\
   0 & 0 & 1 & | & -2 \\
   \end{pmatrix}
   $$

Теперь матрица находится в ступенчатом виде. Можно перейти к обратной подстановке для нахождения решений.

7. **Обратная подстановка**:
   - Из третьей строки находим $z = -2$.
   - Подставляем $z = -2$ во вторую строку: $y + \frac{5}{2} \cdot (-2) = -2$. Отсюда $y = 3$.
   - Подставляем $y = 3$ и $z = -2$ в первую строку: $x + 3 - 2 = 6$. Отсюда $x = 5$.

Итак, решение системы:
$$
x = 5, \quad y = 3, \quad z = -2.
$$

---
# 4. Подстановки
### Подстановки и их обозначение

Подстановкой называется перестановка, записанная в форме отображения множества на себя. Подстановки часто записываются в форме двух строк: верхняя строка обозначает исходные позиции элементов, а нижняя — новые позиции этих элементов после перестановки.

Пример: Подстановка
$$
\begin{pmatrix}
1 & 2 & 3 \\
2 & 3 & 1 \\
\end{pmatrix}
$$
означает, что элемент $1$ переходит на позицию $2$, элемент $2$ — на позицию $3$, а элемент $3$ — на позицию $1$.

### Транспозиция

Транспозиция — это подстановка, меняющая местами два элемента, оставляя остальные элементы на своих местах. Любую перестановку можно представить в виде произведения транспозиций.

Пример: Подстановка
$$
\begin{pmatrix}
1 & 2 & 3 \\
3 & 2 & 1 \\
\end{pmatrix}
$$
может быть представлена как произведение транспозиций $(1 \; 3)$.

### Циклы в подстановках

Цикл — это последовательность элементов, которые последовательно переходят друг в друга, в то время как остальные элементы остаются на своих местах. Любую подстановку можно представить как произведение независимых циклов.

Пример: Подстановка
$$
\begin{pmatrix}
1 & 2 & 3 & 4 & 5 \\
2 & 3 & 1 & 5 & 4 \\
\end{pmatrix}
$$
состоит из двух циклов: $(1 \; 2 \; 3)$ и $(4 \; 5)$.

Эта подстановка переводит $1 \to 2 \to 3 \to 1$ и $4 \leftrightarrow 5$, оставляя структуру, где каждый цикл отображает переход элементов между позициями.

### Чётность подстановок

Чётность подстановки определяется количеством транспозиций, на которые её можно разложить. Если подстановка может быть разложена на чётное число транспозиций, то она называется **чётной**, если на нечётное — **нечётной**.

#### Теорема о чётности подстановок

Чётность подстановки не зависит от конкретного разложения на транспозиции. То есть, если подстановка является чётной, она всегда будет чётной, каким бы образом её ни разлагали на транспозиции.

#### Определение чётности по числу инверсий

Инверсией называется пара $(i, j)$, где $i < j$, но $a_i > a_j$. Чётность числа инверсий в подстановке определяет её чётность: если количество инверсий чётное, то подстановка чётная; если нечётное, то подстановка нечётная.

### Знак подстановки

Для обозначения чётности или нечётности подстановки используют её знак:
- $\operatorname{sgn}(\sigma) = +1$, если подстановка $\sigma$ чётная.
- $\operatorname{sgn}(\sigma) = -1$, если подстановка $\sigma$ нечётная.

### Примеры

1. **Подстановка в виде транспозиций**: Подстановка $\sigma = (1 \; 3 \; 2)$ можно разложить как $(1 \; 3)(1 \; 2)$. Поскольку она состоит из двух транспозиций, она чётная, и $\operatorname{sgn}(\sigma) = +1$.

2. **Подстановка по числу инверсий**: Рассмотрим подстановку $\sigma = (3, 1, 2)$. Для неё:
   - Пары инверсий: $(3, 1)$ и $(3, 2)$, всего $2$ инверсии.
   - Поскольку количество инверсий чётное, $\sigma$ — чётная подстановка.

### Применение подстановок

Подстановки широко используются в алгебре, комбинаторике и теории чисел, особенно для нахождения детерминантов матриц, поскольку определитель можно вычислить, суммируя произведения элементов с учётом знаков подстановок, как это выражается в формуле:

$$
\det(A) = \sum_{\sigma \in S_n} \operatorname{sgn}(\sigma) \prod_{i=1}^{n} a_{i, \sigma(i)},
$$

где $S_n$ — множество всех перестановок $n$ элементов, а $\operatorname{sgn}(\sigma)$ — знак подстановки $\sigma$.

### Классификация подстановок

- **Тождественная подстановка**: Подстановка, при которой все элементы остаются на своих местах. Обозначается как $\operatorname{id}$.
- **Простая подстановка**: Подстановка, которая может быть представлена как одна транспозиция.
- **Циклическая подстановка**: Подстановка, представляющая собой цикл (последовательность перестановок, в которых элементы переходят друг в друга по кругу).

### Свойства подстановок

1. Произведение двух чётных или двух нечётных подстановок является чётной подстановкой.
2. Произведение чётной и нечётной подстановок является нечётной подстановкой.
3. Тождественная подстановка является чётной.
---
# 5. Матрицы. Теория определителей

#### Основные типы матриц

1. **Квадратная матрица** — матрица, у которой число строк равно числу столбцов. Например, $3 \times 3$ матрица:
   $$
   A = \begin{pmatrix} a_{11} & a_{12} & a_{13} \\ a_{21} & a_{22} & a_{23} \\ a_{31} & a_{32} & a_{33} \end{pmatrix}
   $$

2. **Прямоугольная матрица** — матрица, у которой число строк и столбцов различно. Например, $2 \times 3$ матрица:
   $$
   B = \begin{pmatrix} b_{11} & b_{12} & b_{13} \\ b_{21} & b_{22} & b_{23} \end{pmatrix}
   $$

3. **Нулевая матрица** — матрица, все элементы которой равны нулю. Обозначается как $O$.

4. **Единичная матрица** — квадратная матрица, у которой на главной диагонали стоят единицы, а остальные элементы равны нулю. Обозначается как $I$. Например, $3 \times 3$ единичная матрица:
   $$
   I = \begin{pmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1 \end{pmatrix}
   $$

5. **Диагональная матрица** — квадратная матрица, у которой все элементы вне главной диагонали равны нулю. Например:
   $$
   D = \begin{pmatrix} d_{11} & 0 & 0 \\ 0 & d_{22} & 0 \\ 0 & 0 & d_{33} \end{pmatrix}
   $$

6. **Треугольная матрица** — квадратная матрица, у которой либо все элементы ниже главной диагонали равны нулю (верхняя треугольная матрица), либо все элементы выше главной диагонали равны нулю (нижняя треугольная матрица).

#### Основные операции с матрицами

1. **Сложение и вычитание матриц**. Сложение матриц выполняется поэлементно, и возможно только для матриц одинакового размера.

2. **Умножение матриц**. Если $A$ — матрица размера $m \times n$, а $B$ — матрица размера $n \times p$, то произведение $C = AB$ будет матрицей размера $m \times p$. Элемент $c_{ij}$ находится как сумма произведений элементов $i$-й строки $A$ на элементы $j$-го столбца $B$:
   $$
   c_{ij} = \sum_{k=1}^{n} a_{ik} b_{kj}
   $$

3. **Умножение матрицы на число**. Каждый элемент матрицы умножается на это число.

#### Транспонированная матрица

Транспонированная матрица $A^T$ — это матрица, полученная из $A$ путём замены строк на столбцы. Например, если
$$
A = \begin{pmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \end{pmatrix},
$$
то транспонированная матрица $A^T$ будет
$$
A^T = \begin{pmatrix} 1 & 4 \\ 2 & 5 \\ 3 & 6 \end{pmatrix}.
$$

#### Определитель матрицы

Определитель (детерминант) — это число, которое можно вычислить для квадратной матрицы. Определитель матрицы $A$ обозначается как $\det(A)$ или $|A|$.

Частные случаи:
	Для $2 \times 2$ матрицы $A = \begin{pmatrix} a & b \\ c & d \end{pmatrix}$ определитель равен:
	$$
	\det(A) = ad - bc.
	$$
	Для $3 \times 3$ матрицы $A = \begin{pmatrix} a & b & c \\ d & e & f \\ g & h & i \end{pmatrix}$ определитель равен:
	$$
	\det(A) = a(ei - fh) - b(di - fg) + c(dh - eg).
	$$
### Формула для нахождения определителя через миноры

Для вычисления определителя матрицы $n \times n$ можно использовать метод разложения по минорам. Минором $M_{ij}$ элемента $a_{ij}$ матрицы $A$ называется определитель матрицы, полученной из $A$ удалением $i$-й строки и $j$-го столбца. 

Определитель матрицы $A$ можно найти, разлагая его по элементам любой строки или столбца. Формула разложения по элементам $i$-й строки:

$$
\det(A) = \sum_{j=1}^{n} (-1)^{i+j} a_{ij} M_{ij},
$$

где $a_{ij}$ — элемент матрицы $A$ в $i$-й строке и $j$-м столбце, а $M_{ij}$ — минор этого элемента.

Аналогично, можно разложить определитель по элементам $j$-го столбца:

$$
\det(A) = \sum_{i=1}^{n} (-1)^{i+j} a_{ij} M_{ij}.
$$

### Пример: Вычисление определителя через миноры для $3 \times 3$ матрицы

Рассмотрим матрицу
$$
A = \begin{pmatrix} 1 & 2 & 3 \\ 0 & 4 & 5 \\ 1 & 0 & 6 \end{pmatrix}.
$$

Вычислим определитель, разлагая по элементам первой строки:

1. Для элемента $a_{11} = 1$, минор $M_{11}$ равен определителю матрицы, полученной удалением первой строки и первого столбца:
   $$
   M_{11} = \begin{vmatrix} 4 & 5 \\ 0 & 6 \end{vmatrix} = 4 \cdot 6 - 5 \cdot 0 = 24.
   $$

2. Для элемента $a_{12} = 2$, минор $M_{12}$ равен:
   $$
   M_{12} = \begin{vmatrix} 0 & 5 \\ 1 & 6 \end{vmatrix} = 0 \cdot 6 - 5 \cdot 1 = -5.
   $$

3. Для элемента $a_{13} = 3$, минор $M_{13}$ равен:
   $$
   M_{13} = \begin{vmatrix} 0 & 4 \\ 1 & 0 \end{vmatrix} = 0 \cdot 0 - 4 \cdot 1 = -4.
   $$

Теперь подставим значения в формулу:

$$
\det(A) = 1 \cdot 24 - 2 \cdot (-5) + 3 \cdot (-4) = 24 + 10 - 12 = 22.
$$

Таким образом, $\det(A) = 22$.

#### Обратная матрица

Обратная матрица $A^{-1}$ для квадратной матрицы $A$ — это такая матрица, что $A \cdot A^{-1} = I$, где $I$ — единичная матрица. Обратная матрица существует только для тех матриц, определитель которых не равен нулю.

Для $2 \times 2$ матрицы $A = \begin{pmatrix} a & b \\ c & d \end{pmatrix}$ обратная матрица равна:
$$
A^{-1} = \frac{1}{\det(A)} \begin{pmatrix} d & -b \\ -c & a \end{pmatrix},
$$
где $\det(A) = ad - bc \neq 0$.

#### Метод нахождения обратной матрицы для $n \times n$ матрицы

1. **Записываем исходную матрицу** и рядом с ней единичную матрицу того же размера.
2. **Преобразуем исходную матрицу к единичной матрице** с помощью элементарных операций над строками, при этом выполняем те же операции над единичной матрицей.
3. Когда слева получается единичная матрица, справа будет стоять обратная матрица исходной.

### Ранг матрицы

Рангом матрицы называется максимальное число линейно независимых строк (или столбцов) матрицы. В другом определении, ранг матрицы — это максимальный порядок ненулевого минора, который можно выделить из матрицы.

Ранг матрицы показывает, сколько линейно независимых уравнений или переменных содержится в системе, представленной этой матрицей.

#### Метод приведения к ступенчатому виду (Метод Гаусса)

Метод приведения к ступенчатому виду заключается в преобразовании матрицы с помощью элементарных операций над строками, пока не будет получен ступенчатый вид. После этого количество ненулевых строк в полученной матрице равно рангу матрицы.

##### Шаги метода:

1. Применяем элементарные операции над строками матрицы (перестановка строк, умножение строки на ненулевой коэффициент и сложение строк), чтобы привести её к ступенчатому виду.
2. Получив ступенчатый вид, подсчитываем количество ненулевых строк. Это число и будет равняться рангу матрицы.

##### Пример:

Рассмотрим матрицу:
$$
A = \begin{pmatrix} 1 & 2 & 3 \\ 2 & 4 & 6 \\ 1 & 1 & 1 \end{pmatrix}.
$$

1. Вычтем из второй строки первую, умноженную на $2$, чтобы занулить элемент во втором столбце второй строки:
   $$
   \begin{pmatrix} 1 & 2 & 3 \\ 0 & 0 & 0 \\ 1 & 1 & 1 \end{pmatrix}.
   $$

2. Вычтем из третьей строки первую, чтобы занулить элемент в первом столбце:
   $$
   \begin{pmatrix} 1 & 2 & 3 \\ 0 & 0 & 0 \\ 0 & -1 & -2 \end{pmatrix}.
   $$

Теперь матрица находится в ступенчатом виде, и в ней две ненулевые строки, значит, $\operatorname{rank}(A) = 2$.

#### Пример операций над матрицами

Рассмотрим матрицы $A$ и $B$:

$$
A = \begin{pmatrix} 1 & 2 \\ 3 & 4 \end{pmatrix}, \quad B = \begin{pmatrix} 5 & 6 \\ 7 & 8 \end{pmatrix}.
$$

1. **Сложение** $A + B$:
   $$
   A + B = \begin{pmatrix} 1+5 & 2+6 \\ 3+7 & 4+8 \end{pmatrix} = \begin{pmatrix} 6 & 8 \\ 10 & 12 \end{pmatrix}.
   $$

2. **Умножение** $A \cdot B$:
   $$
   A \cdot B = \begin{pmatrix} 1 \cdot 5 + 2 \cdot 7 & 1 \cdot 6 + 2 \cdot 8 \\ 3 \cdot 5 + 4 \cdot 7 & 3 \cdot 6 + 4 \cdot 8 \end{pmatrix} = \begin{pmatrix} 19 & 22 \\ 43 & 50 \end{pmatrix}.
   $$

3. **Транспонирование** $A^T$:
   $$
   A^T = \begin{pmatrix} 1 & 3 \\ 2 & 4 \end{pmatrix}.
   $$

4. **Определитель** $A$:
   $$
   \det(A) = 1 \cdot 4 - 2 \cdot 3 = -2.
   $$

5. **Обратная матрица** $A^{-1}$:
   $$
   A^{-1} = \frac{1}{-2} \begin{pmatrix} 4 & -2 \\ -3 & 1 \end{pmatrix} = \begin{pmatrix} -2 & 1 \\ \frac{3}{2} & -\frac{1}{2} \end{pmatrix}.
   $$
---
### Свойства определителей 

#### 1. Определитель единичной матрицы равен 1

Если $I$ — единичная матрица, то $\det(I) = 1$.

**Пример:**
$$
I = \begin{pmatrix} 1 & 0 \\ 0 & 1 \end{pmatrix}.
$$
Для этой матрицы:
$$
\det(I) = 1 \cdot 1 - 0 \cdot 0 = 1.
$$

#### 2. Определитель транспонированной матрицы равен определителю исходной матрицы

Если $A^T$ — транспонированная матрица для $A$, то $\det(A^T) = \det(A)$.

**Пример:**
$$
A = \begin{pmatrix} 1 & 2 \\ 3 & 4 \end{pmatrix}, \quad A^T = \begin{pmatrix} 1 & 3 \\ 2 & 4 \end{pmatrix}.
$$
$$
\det(A) = 1 \cdot 4 - 2 \cdot 3 = -2,
$$
$$
\det(A^T) = 1 \cdot 4 - 3 \cdot 2 = -2.
$$

#### 3. Определитель произведения двух матриц равен произведению их определителей

Если $A$ и $B$ — квадратные матрицы одинакового размера, то $\det(AB) = \det(A) \cdot \det(B)$.

**Пример:**
Пусть
$$
A = \begin{pmatrix} 1 & 0 \\ 0 & 2 \end{pmatrix}, \quad B = \begin{pmatrix} 3 & 0 \\ 0 & 4 \end{pmatrix}.
$$
Вычислим $\det(A)$ и $\det(B)$:
$$
\det(A) = 1 \cdot 2 = 2, \quad \det(B) = 3 \cdot 4 = 12.
$$
Теперь найдём $\det(AB)$:
$$
AB = \begin{pmatrix} 3 & 0 \\ 0 & 8 \end{pmatrix}, \quad \det(AB) = 3 \cdot 8 = 24.
$$
Проверяем: $\det(A) \cdot \det(B) = 2 \cdot 12 = 24$, что совпадает с $\det(AB)$.

#### 4. Определитель матрицы с нулевой строкой или столбцом равен нулю

**Пример:**
$$
A = \begin{pmatrix} 0 & 0 \\ 1 & 2 \end{pmatrix}.
$$
Определитель:
$$
\det(A) = 0 \cdot 2 - 0 \cdot 1 = 0.
$$

#### 5. Если две строки или два столбца матрицы одинаковы, то её определитель равен нулю

**Пример:**
$$
A = \begin{pmatrix} 1 & 2 \\ 1 & 2 \end{pmatrix}.
$$
Здесь первая и вторая строки одинаковы. Определитель:
$$
\det(A) = 1 \cdot 2 - 2 \cdot 1 = 0.
$$

#### 6. При перестановке двух строк или столбцов определитель меняет знак

**Пример:**
$$
A = \begin{pmatrix} 1 & 2 \\ 3 & 4 \end{pmatrix}, \quad A' = \begin{pmatrix} 3 & 4 \\ 1 & 2 \end{pmatrix}.
$$
Вычислим $\det(A)$ и $\det(A')$:
$$
\det(A) = 1 \cdot 4 - 2 \cdot 3 = -2,
$$
$$
\det(A') = 3 \cdot 2 - 4 \cdot 1 = 2.
$$
Замена строк изменила знак определителя.

#### 7. Если умножить строку или столбец матрицы на число $k$, то определитель умножится на это число

**Пример:**
$$
A = \begin{pmatrix} 1 & 2 \\ 3 & 4 \end{pmatrix}.
$$
Определитель $A$:
$$
\det(A) = 1 \cdot 4 - 2 \cdot 3 = -2.
$$
Теперь умножим первую строку на $3$ и найдём определитель новой матрицы:
$$
A' = \begin{pmatrix} 3 & 6 \\ 3 & 4 \end{pmatrix}, \quad \det(A') = 3 \cdot 4 - 6 \cdot 3 = -18.
$$
Мы видим, что $\det(A') = 3 \cdot \det(A) = 3 \cdot -2 = -18$.

#### 8. Определитель треугольной матрицы равен произведению элементов на её главной диагонали

**Пример:**
$$
A = \begin{pmatrix} 2 & 0 & 0 \\ 1 & 3 & 0 \\ 4 & 5 & 6 \end{pmatrix}.
$$
Так как $A$ — нижняя треугольная матрица, определитель равен:
$$
\det(A) = 2 \cdot 3 \cdot 6 = 36.
$$

#### 9. Определитель обратной матрицы равен обратному значению определителя исходной матрицы

Если матрица $A$ обратима, то
$$
\det(A^{-1}) = \frac{1}{\det(A)}.
$$

**Пример:**
Пусть
$$
A = \begin{pmatrix} 1 & 2 \\ 3 & 4 \end{pmatrix}.
$$
Тогда $\det(A) = 1 \cdot 4 - 2 \cdot 3 = -2$.

Обратная матрица $A^{-1}$:
$$
A^{-1} = \frac{1}{-2} \begin{pmatrix} 4 & -2 \\ -3 & 1 \end{pmatrix} = \begin{pmatrix} -2 & 1 \\ \frac{3}{2} & -\frac{1}{2} \end{pmatrix}.
$$
Для обратной матрицы:
$$
\det(A^{-1}) = \frac{1}{\det(A)} = \frac{1}{-2} = -0.5.
$$

#### 10. Если к одной строке прибавить другую строку, умноженную на число, то определитель не изменится

**Пример:**
Пусть
$$
A = \begin{pmatrix} 1 & 2 \\ 3 & 4 \end{pmatrix}.
$$
Теперь добавим ко второй строке первую, умноженную на $-3$:
$$
A' = \begin{pmatrix} 1 & 2 \\ 0 & -2 \end{pmatrix}.
$$
Для обеих матриц определитель одинаков:
$$
\det(A) = 1 \cdot 4 - 2 \cdot 3 = -2,
$$
$$
\det(A') = 1 \cdot (-2) - 2 \cdot 0 = -2.
$$
Определитель не изменился.


