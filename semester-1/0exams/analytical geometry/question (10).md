#### Общее уравнение прямой. Алгебраические линии первого порядка.
---
Уравнение прямой с заданной точкой и направляющим вектором:
$$\displaylines{
M \in l(A, \  \overline{a}) \equiv \vec{AM} || \vec{a} \\
A(x_{ 0 }, \  y_{ 0 }), \  M(x, \ y ) \\
\vec{a}(a_{ 1 }, \  a_{ 2 }) \\
\vec{AM}(x-x_{ 0 }, \  y-y_{ 0 }) \\
\implies \begin{vmatrix}
x - x_{ 0 } & y-y_{ 0 } \\
a_{ 1 }  &  a_{ 2 }
\end{vmatrix} = 0  \quad  (5)
}$$
Из ${\displaystyle (5)}$ вытекает общее уравнение прямой:
$$\displaylines{
(5) \implies a_{ 2 }(x-x_{ 0 } ) - a_{ 1 }(y-y_{ 0 }) = 0 \\
\underbrace{ a_{ 2 } }_{ A }x \  \underbrace{ - a_{ 1 } }_{ B }y \underbrace{ - a_{ 2 }x_{ 0 } + a_{ 1 }y_{ 0 } }_{ C } = 0 \\ \\
Ax + By + C = 0, \  \text{ где }  A^{ 2 } + B^{ 2 } \neq 0
}$$
Это уравнение также называется уравнением алгебраической линии первого порядка, которая является прямой.

Доказательство:
Пусть ${\vec{a}(-B, \ A)}$ от общего уравнения прямой, и ${\displaystyle \ M_{ 0 } \left( \dfrac{-AC}{A^{ 2 }+ B^{ 2 }} , \ \dfrac{-BC}{A^{ 2 }+ B^{ 2 }}\right)}$
$$\displaylines{
l (M_{ 0 }, \  \vec{a}) \stackrel{ (5) }{ \implies }  \begin{vmatrix}
x + \dfrac{AC}{A^{ 2 } + b^{ 2 }}  & y + \dfrac{BC}{A^{ 2 }+B^{ 2 }} \\
 -B & A
\end{vmatrix} = 0 \\
\implies  Ax  + By + \frac{A^{ 2 }C}{A^{ 2 }+B^{ 2 }} + \frac{B^{ 2 }C}{A^{ 2 }+B^{ 2 }} = 0 \\
\implies  Ax + By + C\left( \frac{A^{ 2 }}{A^{ 2 } + B^{ 2 }} + \frac{B^{ 2 }}{A^{ 2 }+ B^{ 2 }}   \right) = 0
}$$
Замечание. Для прямой, заданной уравнением таким уравнением направляющий вектор ${\vec{a}(-B, \ A)}$
Следствие. ${\vec{p}(p_{ 1 }, \ p_{ 2 }) \ || \  l:Ax+By+C = 0 \iff Ap_{ 1 } + Bp_{ 2 } = 0}$
Доказательство:
$$\displaylines{
\vec{a} (-A, \  B) \\
\vec{a}||\vec{p} \iff \begin{vmatrix}
p_{ 1 } & p_{ 2 }  \\
-B & A 
\end{vmatrix} = Ap_{ 1 } + B p_{ 2 } = 0
}$$
Уточнение:
$$\displaylines{
\vec{a}(a_{1}, \  a_{2}), \  \vec{b} (b_{1}, \  b_{2}) \\
\vec{a} || \vec{b} \iff  \exists \lambda \in  \mathbb{R} : \vec{b} = \lambda\vec{a} 
}$$
Определитель как проверка измеряет площадь параллелограмма, образованного этими двумя векторами. 
$$\displaylines{
\vec{a}||\vec{b} \iff  \begin{vmatrix}
a_{1} & a_{2} \\
b_{1} & b_{2}
\end{vmatrix} = 0
}$$
Если он равен нулю, площадь параллелограмма равна нулю, что означает, что вектора лежат на одной прямой, то есть они коллинеарны.