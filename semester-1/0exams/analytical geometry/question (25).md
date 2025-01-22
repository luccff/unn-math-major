#### Угол между плоскостями. Взаимное расположение плоскостей.
---
Взаимное расположение плоскостей
Пусть
$$\displaylines{
\pi_{ 1 }: A_{ 1 }x + B_{ 1 }y + C_{ 1 }z + D_{ 1 } = 0 \\
\pi_{ 2 }: A_{ 2}x + B_{ 2 }y + C_{ 2}z + D_{ 2 } = 0
}$$
Они совпадают если ${\displaystyle \exists \lambda \in R: A_{ 2 } = \lambda A_{ 1 }, \ B_{ 2 } = \lambda B_{ 1 }, \ C_{ 2 } = \lambda C_{ 1 }, \ D_{ 2 } = \lambda D_{ 1 }}$. Заметим, что ${\displaystyle \frac{A_{ 1 }}{A_{ 2 }} = \frac{B_{ 1 }}{B_{ 2 }} = \frac{C_{ 1 }}{C_{ 2 }}}$, так как совпадение - частный случай параллельности. Ввиду совпадения плоскостей, координаты ${\displaystyle (x, \ y, \ z)}$ в ${\displaystyle \pi_{ 1 }}$ и ${\displaystyle \pi_{ 2 }}$ совпадают.

Плоскости параллельны, но не совпадают, если их нормальные векторы ${\displaystyle \vec{n}_{ 1 } = (A_{ 1 }, \ B_{ 1 }, \ C_{ 1 })}$ и ${\displaystyle \vec{n}_{ 2 } = (A_{ 2 }, \ B_{ 2 }, \ C_{ 2 })}$ коллинеарны, то есть 
$$\displaylines{
\frac{A_{ 1 }}{A_{ 2 }} = \frac{B_{ 1 }}{B_{ 2 }} = \frac{C_{ 1 }}{C_{ 2 }}
}$$
однако, в отличие от случая совпадения, свободные члены ${\displaystyle D_{ 1 }}$ и ${\displaystyle D_{ 2 }}$ не пропорциональны, то есть:
$$\displaylines{
\frac{D_{ 1 }}{D_{ 2 }} \neq  \frac{A_{ 1 }}{A_{ 2 }} \dots 
}$$
${\displaystyle \vec{n}_{ 1 } || \vec{n}_{ 2 }}$ - критерий параллельности плоскостей. Если ${\displaystyle \vec{n}_{ 1 }}$ можно выразить через ${\displaystyle \lambda\vec{n}_{ 2 }}$, то ${\displaystyle \vec{n}_{ 1 } \times \vec{n}_{ 2 } = 0 \implies \vec{n}_{ 1 } || \vec{n}_{ 2 }}$. 

Если плоскости не параллельны, то они пересекаются по прямой. Условие для этого: ${\displaystyle \vec{n}_{ 1 } \cancel{||} \vec{n}_{ 2 }}$, то есть:
$$\displaylines{
\frac{A_{ 1 }}{A_{ 2 }} \neq  \frac{B_{ 1 }}{B_{ 2 }}  \quad \text{ или }  \quad \frac{B_{ 1 }}{B_{ 2 }} \neq  \frac{C_{ 1 }}{C_{ 2 }}
}$$
Чтобы найти уравнение прямой пересечения нужно решить систему:
$$\displaylines{
\begin{cases}
 A_{ 1 }x + B_{ 1 }y + C_{ 1 }z + D_{ 1 } = 0 \\
 A_{ 2}x + B_{ 2 }y + C_{ 2}z + D_{ 2 } = 0
\end{cases}
}$$

Плоскости перпендикулярны, если их нормальные векторы ортогональны:
$$\displaylines{
\vec{n}_{ 1 } \cdot  \vec{n}_{ 2 } = 0
}$$
Это означает, что ${\displaystyle A_{ 1 }A_{ 2 } + B_{ 1 }B_{ 2 } + C_{ 1 }C_{ 2 } = 0}$.

Угол между двумя плоскостями определяется как угол между их нормальными векторами ${\displaystyle \in \left[ 0; \frac{\pi}{2} \right]}$.
Пусть ${\displaystyle \vec{n}_{ 1 } = (A_{ 1 }, \ B_{ 1 }, \ C_{ 1 })}$ и ${\displaystyle \vec{n}_{ 2 } = (A_{ 2 }, \ B_{ 2 }, \ C_{ 2 })}$ для плоскостей ${\displaystyle \pi_{ 1 }, \ \pi_{ 2 }}$.
$$\displaylines{
\cos{(\theta)} = \frac{|\vec{n}_{ 1 } \cdot  \vec{n}_{ 2 }|}{|\vec{n}_{ 1 }| \cdot |\vec{n}_{ 2 }|} = \frac{A_{ 1 }A_{ 2 } + B_{ 1 }B_{ 2 } + C_{ 1 }C_{ 2 }}{\sqrt{ A_{ 1 }^{ 2 } + B_{ 1 }^{ 2 } + C_{ 1 }^{ 2 } } \cdot \sqrt{ A_{ 2 }^{ 2 } + B_{ 2 }^{ 2 } + C_{ 2 }^{ 2 } }} \\
\theta = \arccos{(\cos{(\theta)})}
}$$
Отсюда вытекают частные случаи взаимного расположения плоскостей:
1. ${\displaystyle \vec{n}_{ 1 } \cdot \vec{n}_{ 2 } = 0 \implies \cos{(\theta)} = 0 \implies \theta = 90^{ \circ }}$
2. ${\displaystyle \vec{n}_{ 1 } || \vec{n}_{ 2 } \implies \frac{\vec{n}_{ 1 }}{\vec{n}_{ 2 }} = \text{const} \implies \theta = 0^{ \circ }}$ или ${\displaystyle 180^{ \circ }}$, но мы всегда рассматриваем ${\displaystyle \theta = 0^{ \circ }}$ для параллельных плоскостей.