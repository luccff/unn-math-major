#### Параметрические уравнения плоскости - векторное и в координатах.
---
${\displaystyle \mathcal{L} \subset \mathbb{R}^{ 3 }}$ - линейное подпространство, ${\displaystyle \dim\mathcal{L} = 2}$. ${\displaystyle \mathcal{L}}$ - направляющее пространство плоскости ${\displaystyle \pi}$.
$$\displaylines{
\vec{a}, \  \vec{b} - \text{ базис пространства  } \mathcal{L} \\
\pi = M_{ 0 } + \mathcal{L} = \{ M \in  \pi  \ \big| \ \vec{M_{ 0 }M} = \lambda\vec{a} + \mu \vec{b} \} \\
\vec{r} = \vec{r}_{ 0 } + \vec{M_{ 0 }M} = \underbrace{ \vec{r}_{ 0 } + \lambda \vec{a} + \mu \vec{b} }_{ \text{ век-парам. урав. } };  \quad \lambda, \  \mu \in  \mathbb{R} ; [a, \  b] \neq 0
}$$
где ${\displaystyle \vec{r}_{ 0 }(x_{0}, \ y_{0}, \ z_{0})}$ - радиус-вектор некоторой фиксированной точки плоскости.
Чтобы ${\displaystyle \vec{r}}$ был радиус-вектором некоторой точки плоскости, необходимо, чтобы ${\displaystyle \vec{r}-\vec{r}_{ 0 }}$, ${\displaystyle \vec{a}-\vec{b}}$ лежали в одной плоскости, то есть их смешанное произведение ${\displaystyle =0}$.

Координатное разложение:
$$\displaylines{
x = x_{ 0 } + \lambda a_{ 1 } + \mu b_{ 1 } \\
y = y_{ 0 } + \lambda a_{2} + \mu b_{ 2 } \\
z = z_{ 0 } + \lambda a_{3} + \mu b_{ 3 }
}$$
Это система параметрических уравнений, выражающая координаты произвольной точки ${\displaystyle M(x, \ y, \ z)}$ через параметры.

Извлечение общего уравнения плоскости:
Вектор ${\displaystyle \vec{M_{ 0 }M} = (x-x_{0}, \ y-y_{ 0 }, \ z-z_{ 0 })}$. 
Плоскость как линейная комбинация векторов ${\displaystyle \vec{a}, \ \vec{b}}$: ${\displaystyle \vec{M_{ 0 }M} = \lambda\vec{a}+ \mu\vec{b}}$.
Нормальный вектор ${\displaystyle \vec{n} = \vec{a} \times \vec{b} = \begin{vmatrix} \vec{i} & \vec{j} & \vec{k} \\ a_{1} & a_{2}&a_{3} \\ b_{1}&b_{2}&b_{3}\end{vmatrix}}$ где ${\displaystyle \vec{n} = (n_{1}, \ n_{2}, \ n_{3})}$ - координаты нормального вектора:
$$\displaylines{
n_{1}(x-x_{ 0 }) + n_{ 2 }(y-y_{0}) + n_{3}(z-z_{0}) = 0
}$$
Раскрывая скобки:
$$\displaylines{
n_{1}x+n_{2}y+n_{3}z + D = 0
}$$
где ${\displaystyle D = -(n_{1}x_{ 0 } + n_{2}y_{0} + n_{3}z_{0})}$.

Получаем итоговое координатное уравнение.