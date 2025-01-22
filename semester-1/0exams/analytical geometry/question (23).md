#### Уравнение в плоскости, проходящей через три точки.
---
Пусть ${\displaystyle M(x, \ y, \ z), \ M_{ 0 }(x_{0}, \ y_{0}, \ z_{0})}$ в аффинном репере ${\displaystyle (O, \ \{ \vec{e}_{ 1 }, \ \vec{e}_{ 2 }, \ \vec{e}_{ 3 } \})}$.
$$\displaylines{
\implies \begin{cases}
x = x_{ 0 } + \lambda a_{ 1 } + \mu b_{ 1 } \\
y = y_{ 0 } + \lambda a_{2} + \mu b_{ 2 } \\
z = z_{ 0 } + \lambda a_{3} + \mu b_{ 3 }
\end{cases} \quad \begin{matrix}
\text{ где } \vec{a} = (a_{1}, \  a_{2}, \  a_{3})  \\
\vec{b} = (b_{1}, \  b_{2}, \  b_{3}) \\
\text{ в базисе } \{ \vec{e}_{ 1 }, \  \vec{e}_{ 2 }, \  \vec{e}_{ 3 } \}
\end{matrix}

}$$
![[Pasted image 20250119214142.png | 500]]
${\displaystyle \vec{M_{ 0 }M_{ 1 }}, \ \vec{M_{ 0 }M_{ 2 }}}$ - базис направляющего пространства плоскости ${\displaystyle \pi}$. ${\displaystyle M \in \pi \iff \vec{M_{ 0 }M_{ 1 }}, \ \vec{M_{ 0 }M_{ 2 }}, \ \vec{M_{ 0 }M}}$ - компланарны. То есть
$$\displaylines{
\begin{vmatrix}
x-x_{ 0 } & y-y_{0} & z-z_{0}\\
x_{1}-x_{ 0 } & y_{2}-y_{0} & z_{1}-z_{0}  \\
x_{2}-x_{ 0 } & y_{3}-y_{0} & z_{2}-z_{0}
\end{vmatrix} = 0
}$$
Это называется уравнением плоскости, проходящее через 3 точки.
Его можно записать в векторном виде, где ${\displaystyle r-r_{ 0 }, \ r_{ 1 }-r_{ 0 }, \ r_{ 2 }-r_{ 0 }}$ - радиус векторы.
