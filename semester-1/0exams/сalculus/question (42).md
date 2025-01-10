### Непрерывность дифференцируемой функции. Доказать.
---
Теорема. Если функция ${\displaystyle f(x)}$ дифференцируема в точке ${\displaystyle x_{0}}$, то она непрерывна в этой точке.

Доказательство:
Дифференцируемость означает, что существует предел
$$\displaylines{
\lim_{ x \to x_{0} } {\frac{f(x)-f(x_{0})}{x-x_{0}} } = f'(x_{0})
}$$
Выразим разность ${\displaystyle f(x)-f(x_{0}) }$:
$$\displaylines{
\frac{f(x) -f(x_{0})  }{x-x_{0}} = f'(x_{0})+\varepsilon(x) \\
f(x)-f(x_{0}) = (x-x_{0})(f'(x_{0})+\varepsilon(x)) 
}$$
Значит ${\displaystyle f(x) \to f(x_{0})}$ при ${\displaystyle x \to x_{0}}$. Следовательно ${\displaystyle \lim_{ x \to x_{0} } {f(x)} = f(x_{0})}$
