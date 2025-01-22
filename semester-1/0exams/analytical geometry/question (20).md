#### Вывод формулы для смешанного произведения в ортонормированном базисе.
---
Пусть в ортонормированном базисе ${\displaystyle \vec{i}, \ \vec{j}, \ \vec{k}}$:
$$\displaylines{
\begin{matrix}
\vec{a} = (a_{1}, \  a_{2}, \  a_{3}) \\
\vec{b} = (b_{1}, \  b_{2}, \  b_{3}) \\
\vec{c} = (c_{1}, \  c_{2}, \  c_{3})
\end{matrix} \implies \vec{a} \cdot  (\vec{b} \times  \vec{c}) = \begin{vmatrix} a_{1} & a_{2} & a_{3} \\ b_{1} & b_{2} & b_{3} \\ c_{1}&c_{2}&c_{3} \end{vmatrix}
}$$
Доказательство:
$$\displaylines{
\vec{b}\times \vec{c} = \begin{vmatrix}
\vec{i} & \vec{j} & \vec{k} \\
b_{ 1 } & b_{ 2 } & b_{ 3 } \\
c_{ 1 } & c_{ 2 } & c_{ 3 }
\end{vmatrix} = \begin{vmatrix}
b_{ 2 } & b_{ 3 } \\
c_{ 2 } & c_{ 3 }
\end{vmatrix} \cdot \vec{i} - \begin{vmatrix}
b_{ 1 } & b_{ 3 } \\
c_{ 1 } & c_{ 3 }
\end{vmatrix}\cdot \vec{j} + \begin{vmatrix}
b_{ 1 } & b_{ 2 } \\
c_{ 1 } & c_{ 2 }
\end{vmatrix} \cdot \vec{k} = \\
= (b_{2}c_{3}-b_{3}c_{2})\vec{i} - (b_{1}c_{3} - b_{3}c_{1}) \vec{j} + (b_{1}c_{2} - b_{2}c_{1})\vec{k} \\ \\
\vec{a} \cdot (\vec{b}\times \vec{c}) = a_{1}(b_{2}c_{3}-b_{3}c_{2}) - a_{2}(b_{1}c_{3} - b_{3}c_{1})   + a_{3}(b_{1}c_{2} - b_{2}c_{1}) = \begin{vmatrix} a_{1} & a_{2} & a_{3} \\ b_{1} & b_{2} & b_{3} \\ c_{1}&c_{2}&c_{3} \end{vmatrix}
}$$