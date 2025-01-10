### Теоремы о пределах функции, связанных с равенствами. Доказать на основании определения предела по Гейне.
---
1. Предел суммы функций:
$$\displaylines{
\lim_{ x \to a } {( f(x) + g(x))} = \lim_{ x \to a } {(f(x))} + \lim_{ x \to a } {(g(x))}
}$$
2. Предел разности функций:
$$\displaylines{
\lim_{ x \to a } {( f(x) - g(x))} = \lim_{ x \to a } {(f(x))} - \lim_{ x \to a } {(g(x))}
}$$
3. Предел произведения функций:
$$\displaylines{
\lim_{ x \to a } {( f(x) \cdot  g(x))} = \lim_{ x \to a } {(f(x))} \cdot  \lim_{ x \to a } {(g(x))}
}$$
3. Предел частного функций:
$$\displaylines{
\lim_{ x \to a } {\left( \frac{f(x)}{g(x)}  \right)} = \cfrac{\displaystyle\lim_{ x \to a } {f(x)}}{\displaystyle\lim_{ x \to a } {g(x)}} 
}$$
*Доказательство*:
Предел суммы функций:
Пусть ${\displaystyle \lim_{ x \to a } {f(x)} = A}$ и ${\displaystyle \lim_{ x \to a } {g(x)} = B}$. Это означает, что для любой последовательности ${\displaystyle \{ x_{n} \} \to a, \ x_{n} \neq a}$ последовательности ${\displaystyle \{ f(x) \}}$ и ${\displaystyle \{ g(x) \}}$ стремятся к ${\displaystyle A}$ и ${\displaystyle B}$ соответственно.
Рассмотрим ${\displaystyle \{ x_{n} \} \to a, \ x_{n} \neq a}$:
$$\displaylines{
f(x_{n}) \to  A \text{ при } n \to  \infty \\
g(x_{n}) \to B \text{ при  } n \to  \infty \\
f(x_{n})+ g(x_{n}) \to  A + B \text{ при  } n \to \infty
}$$
Следовательно, по определению предела по Гейне:
$$\displaylines{
\lim_{ x \to a } {(f(x)+g(x))} = A + B = \lim_{ x \to a } {f(x)} + \lim_{ x \to a } {g(x)}
}$$
Аналогично доказывается остальное.