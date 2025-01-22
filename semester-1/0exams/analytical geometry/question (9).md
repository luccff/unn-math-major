#### Векторное уравнение прямой. Параметрические уравнения прямой. Каноническое уравнение прямой. Уравнение прямой, проходящее через две точки.
---
Определение. Любой ненулевой вектор параллельной плоскости называется направляющим вектором данной прямой.

Обозначение. ${l(A, \ \overline{a})}$ - прямая, проходящая через ${A}$ с направлением вектора ${\overline{a}}$.
Определение. В системе аксиом Г. Вейля, прямая ${l(A, \ \overline{a}) = \{ M \in E^{ 2 } \ | \ \overline{AM} ||\overline{a} \}}$.

Виды уравнений прямой на плоскости:
1. Векторное уравнение прямой: 
$$\displaylines{
\overline{OM} = \overline{OA}+ \overline{AM} = \overline{OA} + t\overline{a}, \ t \in \mathbb{R}\\
\vec{r}_{ M } = \vec{r}_{ A } + t\vec{a}, \   t \in  \mathbb{R} 
}$$
2. Параметрическое уравнение прямой:
$$\displaylines{
R(O, \  B), \  B = \{ \vec{e}_{ 1 }, \  \vec{e}_{ 2 } \}. \\ 
\text{ Пусть } M(x, \  y), \  A(x_{ 0 }, \  y_{ 0 }), \  \vec{a}(a_{1}, \  a_{2}) \\
\underbrace{ x\vec{e}_{ 1 } + y \vec{e}_{ 2 } }_{ \vec{r}_{ M } } = \underbrace{ x_{ 0 } \vec{e}_{ 1 } + y_{ 0 }\vec{e}_{ 2 } }_{ \vec{r}_{ A } } + \underbrace{ t(a_{ 1 }\vec{e}_{ 1 } + a_{ 2 }\vec{e}_{ 2 }) }_{ t\vec{a} } \\
\begin{matrix}
\vec{e}_{ 1 }  \\
\vec{e}_{ 2 }
\end{matrix} \begin{cases}
x = x_{ 0 } + ta_{ 1 }, \  t \in  \mathbb{R}  \\
y = y_{ 0 } + ta_{ 2 }, \   t \in \mathbb{R} 
\end{cases}  \quad (2)
}$$
3. Каноническое уравнение прямой:
Пусть ${a_{ 1 } \cdot a_{ 2 } \neq 0}$ 
$$\displaylines{
(2) \implies \begin{matrix}
t = \dfrac{x-x_{ 0 }}{a_{ 1 }}  \\
t = \dfrac{ y - y_{ 0 }}{a_{ 2 }}
\end{matrix}  \quad  \dfrac{x-x_{ 0 }}{a_{ 1 }} = \frac{y-y_{ 0 }}{a_{ 2 }}  \quad   (3)
}$$

Замечание. Если один из коэффициентов ${a_{ 1 }, \ a_{ 2 }, \ \dots}$ , то будем полагать, что числитель равен 0. т.е. ${\dfrac{x- x_{ 0 }}{0} = \dfrac{y-y_{ 0 }}{a_{ 2 }} \equiv \begin{cases} x-x_{ 0 } = 0 \\ y = y_{ 0 }+ t a_{ 2 }\end{cases}}$
4. Уравнение прямой, проходящей через 2 точки: 
$$\displaylines{
\text{ Пусть } A(x_{1}, \ y_{1}), \ B(x_{2}, \ y_{2}) \in l, \ A\neq B \\
\text{ Пусть } \vec{a} = \vec{AB} = (x_{2}-x_{1}, \  y_{2}-y_{1}) \stackrel{ (3) }{ \implies  } \frac{x-x_{1}}{x_{2}-x_{1}} = \frac{y-y_{1}}{y_{2}-y_{1}}   
}$$