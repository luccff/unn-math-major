Системы линейных уравнений.

$$\displaylines{
\begin{cases}
 3x_{1} - 2x_{2} - x_{3} - x_{4} = 1  \\
3x_{1}x - 2x_{2} - x_{3} - x_{4} = 2  \\
3x_{1} - 2x_{2} + 5x_{3} + 3x_{4} = 2
\end{cases} \\
\begin{pmatrix}
3  &  -2  & -1  & -1 |  & 1  \\
3 & -2 & -1 & -1| & 2 \\
3 & -2 & 5 & 3|  & 2
\end{pmatrix} \to  \begin{pmatrix}
3  &  -2  & -1  & -1 |  & 1   \\
0 & 0 & 0 & 0 |& 1 \\
3 & -2 & 5 & 3| & 2
\end{pmatrix} = \emptyset
}$$

$$\displaylines{
\begin{cases}
3x_{1}-2x_{2} + 5x_{3} + 4x_{4} = 2  \\
9x_{1} - 6x_{2} + 9x_{3} + 7x_{4} = 5 \\
3x_{1} - 2x_{2} - x_{3} - x_{4} = 1
\end{cases} \\
\begin{pmatrix}
3 & -2 & 5 & 4 & | & 2 \\
9 & -6 & 9 & 7 & |  & 5 \\
3 & -2 & -1 & -1 & | & 1
\end{pmatrix} \to \begin{pmatrix}
3 & -2 & -1 & -1 & | & 1 \\
0 & 0 & 6 & 5 & | & 1 \\
0 & 0 & 12 & 10 & | & 2 
\end{pmatrix} \to \begin{pmatrix}
18 & -12 & -6 & -6 & | & 6  \\
0 & 0 & 6 & 5 & | & 1 \\
\end{pmatrix} \\
\to  \begin{pmatrix}
18 & -12 & 0 & -1 &| &  7 \\
0 & 0 & 6 & 5 & | & 1
\end{pmatrix} \\
\begin{cases}
18x_{1} - 12x_{2} - x_{4} = 7  \\
6x_{3} + 5x_{4} = 1
\end{cases} \\
\begin{cases}
 x_{1} = \dfrac{12x_{2} + x_{4} - 7}{18} \\
x_{3} = \dfrac{1-5x_{4}}{6} 
\end{cases} \\
\text{ Общее решение: } (x_{1}, \ x_{2}, \ x_{3}, \ x_{4}) = \left( \frac{12x_{2}+x_{4} + 7}{18}, \ x_{2}, \ \frac{1-5x_{4}}{6}, \ x_{4} \right) \quad x_{2}, \ x_{4} \in \mathbb{R}
}$$
Перестановки и подстановки.

$$\displaylines{
f = \begin{pmatrix}
1 & 2 & 3 & 4 & 5 \\
2 & 3 & 1 & 5 & 4
\end{pmatrix} \\
g = \begin{pmatrix}
1 & 2 & 3 & 4 & 5 \\
3 & 2 & 1 & 5 & 4 
\end{pmatrix} \\
(fg)(i) = f(g(i)) \\
M = \{ 1, \ 2, \ 3, \ 4, \ 5 \} \\
\underbrace{ M \stackrel{ g }{ \to  } M \stackrel{ f }{ \to } M }_{ f \circ g }  \\
fd = \begin{pmatrix}
1 & 2 & 3 & 4 & 5 \\
1 & 3 & 2 & 4 & 5
\end{pmatrix} \\
f-1 = \begin{pmatrix}
1 & 2 & 3 & 4 & 5 \\
3 & 1 & 2 & 5 & 4
\end{pmatrix}
}$$---
Определители.
$$\displaylines{
\begin{vmatrix}
1 & 2 & 3 & 4 \\
-1 & 3 & -1 & 7  \\
4 & -2 & 2 & 6 \\
5 & 5 & 1 & 3
\end{vmatrix} =
2 \cdot \begin{vmatrix}
 1 & 2 & 3 & 4 \\
-1 & 3 & -1 & 7  \\
2 & -1 & \boxed{1} & 3 \\
5 & 5 & 1 & 3
\end{vmatrix} = 2 \cdot \begin{vmatrix}
-5 & 5 & 3 & -5 \\
1 & 2 & -1 & 10 \\
0 & 0 & 1 & 0 \\
3 & 6 & 1 & 0
\end{vmatrix} = 2 \cdot  5 \cdot 3\begin{vmatrix}
-1 & 1 & -1 \\
1 & 2 & 10 \\
1 & 2 & 0
\end{vmatrix} = 30 \begin{vmatrix}
-1 & 1 & -1 \\
0 & 0 & 10 \\
1 & 2 & 0
\end{vmatrix} = -300 \begin{vmatrix}
-1 & 1 \\
1 & 2
\end{vmatrix} = -300 \cdot -3 = 900
}$$

Обратная матрица.
$$\displaylines{
(AB)^{ -1 } \text{ и } (5A)^{ -1 } =? \\
A^{ -1 } = \begin{pmatrix}
1 & 2 \\
-1 & 3
\end{pmatrix}, \   B^{ -1 } = \begin{pmatrix}
0 & 1 \\
1 & 2
\end{pmatrix} \\
\text{ Решение: } (AB)^{ -1 } = B^{ -1 }A^{ -1 } =\begin{pmatrix}
0 & 1 \\
1 & 2
\end{pmatrix}\begin{pmatrix}
1 & 2 \\
-1 & 3
\end{pmatrix} = \begin{pmatrix}
-1 & 3 \\
-1 & 8
\end{pmatrix} \\
(5A)^{ -1 } = \frac{1}{5} \cdot \begin{pmatrix}
1 & 2 \\
-1 & 3
\end{pmatrix} = \begin{pmatrix}
\dfrac{1}{5} & \dfrac{2}{5} \\
-\dfrac{1}{5} & \dfrac{3}{5}
\end{pmatrix}
}$$
$$\displaylines{
(AB)^{ -1 } \text{ и } (-3A)^{ -1 } = ? \\
A^{ -1 } = \begin{pmatrix}
2  & 0 & 0 \\
0 & 3 & 0 \\
0 & 0 & -4
\end{pmatrix}, \   B^{ -1 } = \begin{pmatrix}
0 & 1 & -1 \\
2 & 3 & -5 \\
4 & -2 & 1
\end{pmatrix} \\
\text{ Решение:} \ (AB)^{ -1 } = \begin{pmatrix}
0 & 1 & -1  \\
2 & 3 & -5 \\
4 & -2 & 1
\end{pmatrix}\begin{pmatrix}
2 & 0 & 0 \\
0 & 3 & 0 \\
0 & 0 & -4
\end{pmatrix} = \begin{pmatrix}
0 & 3 & 4 \\
4 & 9 & 20 \\
8 & -6 & -4
\end{pmatrix} \\
(-3A)^{ -1 } = \begin{pmatrix}
-\dfrac{2}{3} & 0 & 0 \\
0 & -1 & 0  \\
0 & 0 & \dfrac{4}{3}
\end{pmatrix} \\
(B^{ -1 } | E) = \begin{pmatrix}
0 & 1 & -1  & |  & 1 & 0 & 0\\
2 & 3 & -5  & |  & 0 & 1 & 0\\
4 & -2 & 1 & | & 0 & 0 & 1 
\end{pmatrix} \to \begin{pmatrix}
2 & 3 & -5 & | & 0 & 1 & 0 \\
0 & 1 & -1 & | & 1 & 0 & 0 \\
0 & -8 & 11 & | & 0 & 2 & 1
\end{pmatrix} \to  \begin{pmatrix}
2 & 3 & -5 & | & 0 & 1 & 0 \\
0 & 1 & -1 & | & 1 & 0 & 0 \\
0 & 0 & 3 & | & 8 & -2 & 1
\end{pmatrix} \\
\to \begin{pmatrix}
6 & 9 & -15 & | & 0 & 3 & 0 \\
0 & 3 & -3 & | & 3 & 0 & 0 \\
0 & 0 & 3 & | & 8 & -2 & 1
\end{pmatrix} \to \begin{pmatrix}
6 & 9 & 0 & | & 40 & -7 & 5 \\
0 & 3 & 0 & | & 11 & -2 & 1 \\
0 & 0 & 3 & | & 8 & -2 & 1
\end{pmatrix} \to  \begin{pmatrix}
6 & 0 & 0 & | & 7 &-1 & 2 \\
0 & 3 & 0 & | & 11 & -2 & 1 \\
0 & 0 & 3 & | & 8 & -2 & 1 
\end{pmatrix} \to \frac{1}{6} \begin{pmatrix}
7 & -1 & 2 \\
22 & -4 & 2 \\
16 & -4 & 1
\end{pmatrix}
}$$
Комплексные числа.
Тригонометрическая форма.
$$\displaylines{
\begin{aligned}
& 1 = \cos{(0)} + i\sin{(0)} = \cos{(2\pi)} + i\sin{(2\pi)}\\
& -1 = \cos{(\pi)} + i\sin{(\pi)}\\
& i = \cos{\left( \frac{\pi}{2} \right)} + i\sin{\left( \frac{\pi}{2} \right)} \\
& -i = \cos{\left( -\frac{\pi}{2} \right)} + i\sin{\left( -\frac{\pi}{2} \right)}\\
& 1 + i = \sqrt{ 2 } \left(\cos{\left( \frac{\pi}{4} \right)} + i\sin{\left( \frac{\pi}{4} \right)}\right)\\
& \sqrt{ 3 }- i = 2\left( \cos{\left( -\frac{\pi}{6} \right) + i\sin{\left( -\frac{\pi}{6} \right)}} \right)\\
& 4-3i = 5\left( \cos{\left( \arctan{\left( -\frac{3}{4} \right)} \right)} + i\sin{\left( \arctan{\left( -\frac{3}{4} \right)} \right)} \right)\\
& -\cos{\left( \frac{\pi}{7} \right)} + i\sin{\left( \frac{\pi}{7} \right)} = \cos{\left( \pi-\frac{\pi}{7} \right)} + i\sin{\left( \pi-\frac{\pi}{7} \right)} = \cos{\left( \frac{6\pi}{7} \right)} + i \sin{\left( \frac{6\pi}{7} \right)}
\end{aligned}
}$$
Извлечение корней.
$$\displaylines{
\begin{aligned}
& \sqrt[4]{ -1 } = \left\{ \sqrt[4]{ 1 } \left( \cos{\left( \frac{\pi+2\pi k}{4} \right)} + i\sin{\left( \frac{\pi+2\pi k}{4} \right)}  \right) \middle| k = \overline{0, \  3}\right\} = \left\{  \frac{\sqrt{ 2 }}{2} (\pm 1 \pm i)  \right\}\\
& w_{ 0 } = \frac{\sqrt{ 2 }}{2} + i\frac{\sqrt{ 2 }}{2} \\
& \sqrt[3]{ (1+i)^{ 3 } } = \left\{  1 + i, \  \sqrt{ 2 }\cos{\left( \frac{11\pi}{4} \right) + \sqrt{ 2 }i\sin{\left( \frac{11\pi}{12} \right)}}, \  \sqrt{ 2 }\left( \cos{\left( -\frac{5\pi}{12} \right)}  + i\sin{\left( -\frac{5\pi}{12} \right)}\right)  \right\} \\
& \sqrt[4]{ \frac{-1 + i}{1-i\sqrt{ 3 }} } = \left\{  2^{ 1/8 } \left( \cos{\left( \frac{\frac{13\pi}{2} + 2\pi k}{4}  \right)} + i\sin{\left( \frac{13\pi + 24\pi k}{48} \right)} \right), \  k = \overline{0, \  3}  \right\}

\end{aligned}
}$$
