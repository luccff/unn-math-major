### Сравнение бесконечно малых. Символика Э. Ландау.
---
Пусть ${\displaystyle f(x) \wedge g(x)}$ бесконечно малые функции в точке ${\displaystyle a}$.
$$\displaylines{
\begin{aligned}
&\frac{f(x)}{g(x)} \to  C, \  C \neq 0 \implies f(x) \sim g(x), \  x \to a \\ & \text{ Стремление к нулю с одинаковой скоростью } \\ \\
&\frac{f(x)}{g(x)} \to  0 \implies f(x) = o(g(x)), \  x \to  a \\ & f(x) \text{ стремится быстрее чем ${\displaystyle g(x)}$ } \\ \\
&\frac{f(x)}{g(x)} \to  \infty \implies g(x) = o(f(x)), \  x \to  a \\
& g(x) \text{ стремится быстрее чем ${\displaystyle f(x)}$ }
\end{aligned}
}$$

Символика Э. Ландау:

1. ${\displaystyle O(g(x))}$ (О большое) используется для обозначения функций, которые ограничены асимптотически сверху функцией ${\displaystyle g(x)}$ при ${\displaystyle x \to a}$.
Это означает, что существует постоянная ${\displaystyle C>0}$, в проколотой окрестности точки ${\displaystyle a}$, такая, что
$$\displaylines{
|f(x)| \leq  C \cdot |g(x)|
}$$
2.  ${\displaystyle \Omega(g(x))}$ (омега большое) используется для обозначения функций, которые ограничены асимптотически снизу функцией ${\displaystyle g(x)}$ при ${\displaystyle x \to a}$.
Это означает, что существует постоянная ${\displaystyle C>0}$, в проколотой окрестности точки ${\displaystyle a}$, такая, что
$$\displaylines{
C \cdot |g(x)| \leq  |f(x)|
}$$
3.  ${\displaystyle \Theta(g(x))}$ (тета большое) используется для обозначения функций, которые ограничены асимптотически снизу и сверху функцией ${\displaystyle g(x)}$ при ${\displaystyle x \to a}$.
Это означает, что существует постоянная ${\displaystyle C, \ C' >0}$, в проколотой окрестности точки ${\displaystyle a}$, такие, что
$$\displaylines{
C \cdot |g(x)| \leq  |f(x)| \leq  C' \cdot |g(x)|
}$$
4. ${\displaystyle o(g(x))}$ (о малое) используется для обозначения функций, которые стремятся к нулю быстрее, чем ${\displaystyle g(x)}$ при ${\displaystyle x \to a}$. Это означает, что 
$$\displaylines{
\lim_{ x \to a } {\frac{f(x)}{g(x)}} = 0
}$$
5. Символ ${\displaystyle \sim}$ обозначает асимптотическую эквивалентность функций ${\displaystyle f(x), \ g(x), \ x\to a}$. Это означает, что 
$$\displaylines{
\lim_{ x \to a } {\frac{f(x)}{g(x)}} = 1
}$$
6. Символы ${\displaystyle \gg \text{ и } \ll}$ обозначают асимптотическое превосходство одной функции над другой.
$$\displaylines{
f(x) \gg g(x) \iff f(x) \text{ растет значительно быстрее, чем } g(x) \\
f(x) \ll g(x) \iff  f(x) \text{ растет значительно медленнее, чем } g(x)
}$$
