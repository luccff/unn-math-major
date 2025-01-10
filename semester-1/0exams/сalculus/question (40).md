### Правила дифференцирования – доказать.
---
Производная суммы:
$$\displaylines{
\dfrac{d}{dx} [f(x)+g(x)] = f'(x) + g'(x) \\
\frac{d}{dx}[f(x)+g(x)] = \lim_{ \Delta x \to 0 } {\frac{[f(x+\Delta x)+g(x+\Delta x)] - [f(x) +g(x) ]}{\Delta x} } \\
\lim_{ \Delta x \to 0 } {\frac{f(x+\Delta x)-f(x)}{\Delta x} } = f'(x)  \quad \text{ и }  \quad \lim_{ \Delta x \to 0 } {\frac{g(x+\Delta x)-g(x)}{\Delta x} } = g'(x) 
}$$
Производная произведения:
$$\displaylines{
\frac{d}{dx}[f(x)g(x)] = f'(x)g(x)+f(x)g'(x) \\
\frac{d}{dx}[f(x)g(x)] = \lim_{ \Delta x \to 0 } {\frac{f(x+\Delta x)g(x+\Delta x)-f(x)g(x)}{\Delta x} } = \\
= \lim_{ \Delta x \to 0 } {\frac{[f(x+\Delta x)-f(x)]g(x+\Delta x) + f(x)[g(x+\Delta x)-g(x)]}{\Delta x} } =  \\
= \lim_{ \Delta x \to 0 } {\frac{f(x+\Delta x)-f(x)}{\Delta x} \cdot g(x+\Delta x) } + f(x)\lim_{ \Delta x \to 0 } {\frac{g(x+\Delta x) - g(x)}{\Delta x} } = \\
= f'(x)\cdot g(x) + f(x)\cdot g'(x)
}$$
Производная частного:
$$\displaylines{
\frac{d}{dx}\left[ \frac{f(x)}{g(x) } \right] = \frac{f'(x)g(x)-f(x)g'(x)}{g(x)^{ 2 }} \\
\frac{d}{dx}\left[ \frac{f(x)}{g(x) } \right] = \lim_{ \Delta x \to 0 } {\frac{\cfrac{f(x+\Delta x)}{g(x+\Delta x)} - \cfrac{f(x) }{g(x) } }{\Delta x} } = \lim_{ \Delta x \to 0 } {\frac{f(x+\Delta x)g(x)-f(x)g(x+\Delta x)}{\Delta x \cdot g(x+\Delta x)g(x)} } = \\ 
= \frac{f'(x)g(x)-f(x)g'(x)}{g(x)^{ 2 }} 
}$$
Производная сложной функции:
$$\displaylines{
\displaylines{ \\
y = f(g(x)), \  u = g(x) \\
\Delta y = f(g(x+\Delta x)) - f(g(x) ), \  \Delta u = g(x+\Delta x) - g(x) \\
\dfrac{dy}{dx} = \lim_{ \Delta x \to 0 } {\frac{f(g(x+\Delta x))-f(g(x) )}{\Delta x} } = \lim_{ \Delta x \to 0 } {\left( \frac{f(g(x+\Delta x))-f(g(x) )}{\Delta u} \cdot  \frac{\Delta u}{\Delta x}  \right)} = \\
= \begin{cases}
\displaystyle\lim_{ \Delta u  \to 0 } {\left( \frac{f(g(x+\Delta x)) - f(g(x) )}{\Delta y}  \right)} = f'(u)= f'(d(x))  \\ \\

\displaystyle\lim_{ \Delta x \to 0 } {\frac{\Delta u}{\Delta x}} = g'(x)
\end{cases} \\ \\
\dfrac{d}{dx} f(g(x) ) = f'(g(x) ) \cdot  g'(x)
}
}$$
