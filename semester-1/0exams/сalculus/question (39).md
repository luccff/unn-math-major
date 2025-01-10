### Производная сложной функции – вывести.
---
$$\displaylines{
\dfrac{dy}{dx} = f'(g(x)) \cdot  g'(x)
}$$
Вывод:
$$\displaylines{ \\
y = f(g(x)), \  u = g(x) \\
\Delta y = f(g(x+\Delta x)) - f(g(x) ), \  \Delta u = g(x+\Delta x) - g(x) \\
\dfrac{dy}{dx} = \lim_{ \Delta x \to 0 } {\frac{f(g(x+\Delta x))-f(g(x) )}{\Delta x} } = \lim_{ \Delta x \to 0 } {\left( \frac{f(g(x+\Delta x))-f(g(x) )}{\Delta u} \cdot  \frac{\Delta u}{\Delta x}  \right)} = \\
= \begin{cases}
\displaystyle\lim_{ \Delta u  \to 0 } {\left( \frac{f(g(x+\Delta x)) - f(g(x) )}{\Delta y}  \right)} = f'(u)= f'(d(x))  \\ \\

\displaystyle\lim_{ \Delta x \to 0 } {\frac{\Delta u}{\Delta x}} = g'(x)
\end{cases} \\ \\
\dfrac{d}{dx} f(g(x) ) = f'(g(x) ) \cdot  g'(x)
}$$

