### Полунепрерывность (односторонняя непрерывность) в точке.
---
Определение. Функция называется:
 1. **Полунепрерывной сверху в точке** ${\displaystyle x_{0}}$, если:
$$\displaylines{
\forall \varepsilon > 0 \, \exists \delta > 0 : 0 < |x - x_0| < \delta \implies f(x) < f(x_0) + \varepsilon.
}$$
2. **Полунепрерывной снизу в точке** ${\displaystyle x_{0}}$​, если:
$$\displaylines{
\forall \varepsilon > 0 \, \exists \delta > 0 : 0 < |x - x_0| < \delta \implies f(x) > f(x_0) - \varepsilon.
}$$
Связь с односторонними пределами:
$$\displaylines{
\lim_{ x \to x_{0} } {\sup(f(x))} \leq f(x_{0}) \\
\lim_{ x \to x_{0} } {\inf(f(x))} \geq f(x_{0})
}$$

Свойства полунепрерывности:
1. Если функция непрерывна в точке ${\displaystyle x_{0}}$, то она одновременно полунепрерывна сверху и снизу в этой точке.
2. Полунепрерывность сверху или снизу не требует существования предела функции в точке ${\displaystyle x_{0}}$

Примеры:
1. $$\displaylines{
f(x) = \begin{cases}
x, \  & x<0 \\
1, \ &  x\geq 0
\end{cases}
}$$
В точке ${\displaystyle x_{0} = 0}$ функция полунепрерывна сверху, так как ${\displaystyle f(x)<f(0)+ \varepsilon}$
2. $$\displaylines{
f(x) = \begin{cases}
-1, \  & x\leq 0 \\
x, \ &  x> 0
\end{cases}
}$$
В точке ${\displaystyle x_{0} = 0}$ функция полунепрерывна снизу, так как ${\displaystyle f(x)>f(0)- \varepsilon}$
