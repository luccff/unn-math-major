### Определение непрерывности функции в точке. Записать через символику Коши и Гейне. Теоремы о непрерывных функциях. Доказать.
---
*Определение*. Пусть функция ${\displaystyle f}$ определена в некоторой окрестности ${\displaystyle U(a)}$, ${\displaystyle  a \in \mathbb{R}}$. Функция ${\displaystyle f}$ называется **непрерывной в точке** ${\displaystyle a}$ если ${\displaystyle \lim_{ x \to a } {f(x)} = f(a)}$.
Через символику Коши это выглядит так:
$$\displaylines{
\forall{\varepsilon>0} \ \exists\delta = \delta(\varepsilon) > 0: \forall{x}: |x-x_{ 0 }| < \delta \implies  |f(x)- f(a)| < \varepsilon
}$$
По Гейне:
$$\displaylines{
\forall{\{ x_{n} \}}: x_{n} \in  U(a), \  \lim_{ n \to \infty } {x_{n}} = a \implies  \lim_{ n \to \infty } {f(x_{n})} = f(a)
}$$
Лемма о сохранении знака функции:
Пусть функция ${\displaystyle f}$ непрерывна в точке ${\displaystyle x_{ 0 }, \ f(x_{0})>0}$. Тогда
$$\displaylines{
\exists U(x_{ 0 }): \forall{x \in  U(x_{ 0 })} \implies f(x)>0
}$$
Доказательство:
Пусть ${\displaystyle f(x_{ 0 }) = d>0}$. Возьмем ${\displaystyle \varepsilon = \frac{d}{2}>0}$. Тогда
$$\displaylines{
\exists\delta>0: \forall{x}:|x-x_{ 0 }| < \delta \implies  |f(x)-f(x_{ 0 })| < \frac{d}{2}
}$$
Откуда следует, что 
$$\displaylines{
\forall{x \in  U_{ \delta }(x_{ 0 }) \implies  f(x) = f(x_{ 0 }) +(f(x) - f(x_{ 0 })) > d- \frac{d}{2}= \frac{d}{2}>0}
}$$

Теорема (арифметические свойства непрерывных функций).
Пусть функции ${\displaystyle f, \ g }$ непрерывны в точке ${\displaystyle x_{ 0 }}$. Тогда функции ${\displaystyle f\pm g, \ f\cdot g, \frac{f}{g} \text{ при } g(x_{ 0 })\neq0}$ непрерывны в точке ${\displaystyle x_{0}}$.
Доказательство:
$$\displaylines{
\lim_{ x \to x_{0} } {(f(x)\pm g(x))} = \lim_{ x \to x_{0} } {f(x) \pm \lim_{ x \to x_{0} } {}g(x) = f(x_{ 0 }) \pm  g(x_{0})}
}$$
$$\displaylines{
\lim_{ x \to x_{0} } {(f(x) \cdot  g(x))} = \lim_{ x \to x_{0} } {f(x)} \cdot  \lim_{ x \to x_{0} } {g(x)} = f(x_{0})\cdot g(x_{0})
}$$
Частное можно доказать по лемме сохранения знака 
$$\displaylines{
\exists U(x_{0}): \forall{x} \in  U(x_{ 0 }) \implies g(x) \neq 0
}$$
Так что частное ${\displaystyle \frac{f}{g}}$ определено на ${\displaystyle U(x_{ 0 })}$. Поэтому
$$\displaylines{
\lim_{ x \to x_{ 0 } } {\frac{f(x)}{g(x)}} = \cfrac{\displaystyle\lim_{ x \to x_{0} } {f(x)}}{\displaystyle\lim_{ x \to x_{0} } {g(x)}} = \frac{f(x_{0})}{g(x_{0})} 
}$$