#### Взаимное расположение прямых на плоскости.
---
Даны прямые ${l_{ 1 }: A_{ 1 }x + B_{ 1 }y + C_{ 1 } = 0}$ и ${l_{ 2 }: A_{ 2 }x + B_{ 2 }y + C_{ 2 } = 0}$
 1. ${\displaystyle l_{ 1 } = l_{ 2 } \iff}$ когда соответствующие коэффициенты совпадают, 
$$\displaylines{
\text{ то есть }  {\displaystyle \exists \lambda : \begin{cases}A_{ 2 } = \lambda A_{ 1 }  \\ B_{ 2 } = \lambda B_{ 1 }  \\C_{ 2 } = \lambda C_{ 1 } \end{cases}}
}$$
Доказательство:
$$\displaylines{
(\implies ) \ \text{ Направляющие векторы } \vec{a}_{ l_{ 1 } } || \  \vec{a}_{ l_{ 2 } } \implies  \exists\lambda \in  \mathbb{R} : \vec{a}_{ l_{ 2 } } = \lambda\vec{a}_{ l_{ 1 } } \\
\vec{a}_{ l_{ 2 } } = (-B_{ 2 }, \  A_{ 2 }), \  \vec{a}_{ l_{ 1 } } = (-B_{ 1 }, \  A_{ 1 }) \implies  \begin{cases}
A_{ 2 } = \lambda A_{ 1 } \\ 
B_{ 2 } = \lambda B_{ 1 }
\end{cases}  \quad (*)\\
\text{ Пусть } l_{ 1 } \ni M_{ 0 }(x_{ 0 }, \  y_{ 0 }) \in l_{ 2 }  \hookrightarrow A_{ 1 } x_{ 0 } + B_{ 1 } y_{ 0 } + C_{ 1 } = 0   \quad (1)\\
\text{ С учетом } (*) \ \lambda A_{ 1 }x_{0} + \lambda B_{ 1 } y_{ 0 } + C_{ 2 } = 0  \quad (2) \\
\lambda \cdot (1) - (2) = \lambda C_{ 1 } = C_{ 2 }
}$$
${\displaystyle (\impliedby)}$ Если коэффициенты пропорциональны, уравнения описывают одно и то же множество точек. Оба уравнения задают одно и то же множество точек, так как их уравнения отличаются лишь на множитель $\lambda$, а это не меняет геометрическую прямую.

 2. $\ l_{ 1 } || l_{ 2 } \iff$  когда соответствующие коэффициенты при неизвестных пропорциональны, и не пропорциональны свободным членам,
$$\displaylines{
\text{ то есть } \exists\lambda: \begin{cases} A_{ 2 } = \lambda A_{ 1 }  \\ B_{ 2 } = \lambda B_{ 1 }  \\ C_{ 2 } \neq \lambda C_{ 1 }\end{cases}
}$$
 Доказательство:
 $$\displaylines{
(\implies ) \ l_{ 1 } || l_{ 2 } \implies   \vec{a}_{ l_{ 1 } } || \ \vec{a}_{ l_{ 2 } } \implies  \begin{cases}
A_{ 2 } = \lambda A_{ 1 } \\ 
B_{ 2 } = \lambda B_{ 1 }
\end{cases} \\
\text{ Если } C_{ 2 } = \lambda C_{1}, \  \text{ то по доказанному } l_{ 1 } = l_{ 2 }. \text{ Противоречие. }
}$$
$$\displaylines{
(\impliedby ) \text{ Если } l_{ 1 } \cancel{||} l_{ 2 } \text{, то } \exists M_{ 0 } (x_{ 0 }, \  y_{ 0 }) \in l_{ 1 }, \  l_{ 2 } \\
A_{ 1 }x_{ 0 } + B_{ 1 } y_{ 0 } + C_{ 1 } = 0  \quad (1)\\
\text{ С учетом, что } \begin{cases}A_{ 2 } = \lambda A_{ 1 }  \\ B_{ 2 } = \lambda B_{ 1 }  \\C_{ 2 } \neq  \lambda C_{ 1 } \end{cases} \\
\lambda A_{ 1 } x_{ 0 } + \lambda B_{ 1 }y_{ 0 } + C_{ 2 } = 0  \quad (2)\\
\text{ Вычитая } \lambda (1) - (2) \text{ получаем } \lambda C_{ 1 } = C_{ 2 } - \text{ противоречие. }
}$$
 3. $l_{ 1 } \cap l_{ 2 } = \{ !M_{ 0 } \} \iff$ когда соответствующие коэффициенты при неизвестных не совпадают,
$$\displaylines{
\text{ то есть } \frac{A_{ 1 }}{A_{ 2 }} \neq  \frac{B_{ 1 }}{B_{ 2 }} 
}$$
Доказательство:
$$\displaylines{
\text{ Если } \begin{cases}A_{ 2 } = \lambda A_{ 1 }  \\ B_{ 2 } = \lambda B_{ 1 }  \\C_{ 2 } = \lambda C_{ 1 } \end{cases}, \   \text{ тогда } l_{ 1 } = l_{ 2 } - \text{ противоречие. } \\
\text{ Если } \begin{cases}A_{ 2 } = \lambda A_{ 1 }  \\ B_{ 2 } = \lambda B_{ 1 }  \\C_{ 2 } \neq  \lambda C_{ 1 } \end{cases}, \   \text{ тогда } l_{ 1 } || l_{ 2 } - \text{ противоречие. } 
}$$

 