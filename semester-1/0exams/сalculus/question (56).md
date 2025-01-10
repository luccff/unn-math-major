### Правила Лопиталя. Доказать любые два.
---
**Теорема 1.** Пусть функции ${\displaystyle f(x)}$ и ${\displaystyle g(x)}$ определенные на ${\displaystyle [a, \ b]}$, таковы, что:
$$\displaylines{
\begin{aligned}
& 1) \ f(a) = g(a) = 0 \\
& 2) \ \exists f'(a) \text{ и } g'(a) \neq 0 
\end{aligned}
}$$
Тогда существует предел:
$$\displaylines{
\lim_{ x \to a+0 } {\frac{f(x)}{g(x) }} = \frac{f'(a)}{g'(a)}
}$$

Доказательство: применим метод выделения главной части. В силу условия 2 имеем:
$$\displaylines{
f(x) = f(a) + f'(a)(x-a) + o(x-a)\\
g(x) = g(a) + g'(a)(x-a) + o(x-a)
}$$
Отсюда, согласно условию 1 получим:
$$\displaylines{
f(x) = f'(a)(x-a) + o(x-a), \  \quad g(x) = g'(a)(x-a) + o(x-a)
}$$
а поэтому
$$\displaylines{
\lim_{ x \to a+0 } {\frac{f(x)}{g(x) }} = \lim_{ x \to a+0 } {\frac{f'(a) + \cfrac{o(x-a)}{x-a} }{g'(a) + \cfrac{o(x-a)}{x-a} } } = \frac{f'(a)}{g'(a)}
}$$

**Теорема 2**. Пусть функции ${\displaystyle f(x)}$ и ${\displaystyle g(x)}$:
$$\displaylines{
\begin{aligned}
& 1) \text{ Дифференцируемы на } (a, \  b) \\
& 2) \ \lim_{ x \to a+0 } {f(x)} = \lim_{ x \to a+0 } {g(x)} = 0 \\
& 3) \ g'(x)\neq 0 \ \forall{x \in (a, \  b)} \\
& 4) \ \exists \lim_{ x \to a+0 } {\frac{f'(x)}{g'(x)}} = L \in \overline{\mathbb{R} }
\end{aligned}
}$$
Тогда существует предел
$$\displaylines{
\lim_{ x \to a+0 } {\frac{f(x)}{g(x)}} = \lim_{ x \to a+0 } \frac{f'(x)}{g'(x)}
}$$

Доказательство: доопределим функции ${\displaystyle f, \ g}$ в точке ${\displaystyle a}$.
$$\displaylines{
f(a) = g(a) = 0
}$$
Теперь функции непрерывны в точке ${\displaystyle a}$ и удовлетворяют условиям теоремы Коши о среднем значении на любом отрезке ${\displaystyle [a, \ x]}$, где ${\displaystyle a<x<b}$. Поэтому для каждого ${\displaystyle x, \ a<x<b}$ существует такое ${\displaystyle \xi = \xi(x) \in (a, \ x)}$:
$$\displaylines{
\frac{f(x)}{g(x) } = \frac{f(x) - f(a)}{g(x) - g(a)}= \frac{f'(\xi)}{g'(\xi)}   \quad (*)
}$$
причем ${\displaystyle \lim_{ x \to a+0 } {\xi(a)} = a}$. 
Поэтому, если существует ${\displaystyle \lim_{ x \to a+0 } {\frac{f'(x)}{g'(x)} = L}}$, то из правила замены переменного для пределов функции следует, что существует ${\displaystyle \lim_{ x \to a+0 } {\frac{f'(\xi)}{g'(\xi)} = L}}$. Поэтому из ${\displaystyle (*)}$ получаем:
$$\displaylines{
\lim_{ x \to a+0 } {\frac{f(x)}{g(x)}} = \lim_{ x \to a+0 } {\frac{f'(\xi)}{g'(\xi)}} = L
}$$
