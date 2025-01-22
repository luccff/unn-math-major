#### Критерий компланарности, использующий смешанное произведение.
---
Для компланарности векторов ${\displaystyle \vec{a}, \ \vec{b}, \ \vec{c}}$ трехмерного пространства необходимо и достаточно, чтобы их смешанное произведение было равно нулю.
Доказательство:
${\displaystyle \implies}$ Предположение: вектора компланарны. Это означает, что ${\displaystyle \vec{c}}$ можно выразить как линейную комбинацию ${\displaystyle \vec{a}, \ \vec{b}}$:
$$\displaylines{
\vec{c} = \alpha\vec{a} + \beta\vec{b}, \   \quad \alpha, \  \beta \in  \mathbb{R} \\
[\vec{a}, \  \vec{b}, \  \vec{c}] = (\vec{a}\times \vec{b}) \cdot  \vec{c}  = (\vec{a} \times  \vec{b}) \cdot  (\alpha\vec{a} + \beta\vec{b}) = \\
= \alpha((\vec{a}\times \vec{b}) \cdot  \vec{a}) + \beta((\vec{a}\times \vec{b})\cdot \vec{b})
}$$
${\displaystyle (\vec{a} \times \vec{b}) \cdot \vec{a}}$ = 0, так как ${\displaystyle \vec{a}\times\vec{b} \perp \vec{a}}$
${\displaystyle (\vec{a} \times \vec{b}) \cdot \vec{b}}$ = 0, так как ${\displaystyle \vec{a}\times\vec{b} \perp \vec{b}}$
Тогда ${\displaystyle [\vec{a}, \ \vec{b}, \ \vec{c}] = 0}$.

${\displaystyle \impliedby}$ Если смешанное равно нулю, то вектора компланарны:
$$\displaylines{
[\vec{a}, \  \vec{b}, \  \vec{c}] = (\vec{a} \times  \vec{b}) \cdot  \vec{c} = 0
}$$
Это означает, что ${\displaystyle \vec{c}}$ ортогонален ${\displaystyle (\vec{a} \times \vec{b})}$, а значит, лежит в той же плоскости, что и ${\displaystyle \vec{a} }$ и ${\displaystyle \vec{b}}$.
