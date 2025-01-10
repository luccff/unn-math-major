### Критерий Коши существования предела функции. Доказать.
---
**Условие Коши существования предела функции в точке:**
$$\displaylines{
 \lim_{ x \to a } f(x) =b \iff  \forall \varepsilon > 0 \ \ \exists \delta > 0 : \forall x', x'' \in D(f(x)), \ \ x',  x'' \in \stackrel{ \circ }{ U }_{ \delta }(a) \implies |f(x') - f(x'')| < \varepsilon 
}$$
**Теорема**. Для того чтобы ${\displaystyle \exists\lim_{ x \to a } {f(x)<\infty}}$, необходимо и достаточно, чтобы ${\displaystyle f}$ удовлетворяла условию Коши выше в этой точке.
*Доказательство*:
1. ${\displaystyle \implies}$. Пусть ${\displaystyle \exists \lim_{ x \to a } {f(x)} = b}$, тогда 
$$\displaylines{
\forall{\varepsilon>0 \ \exists\delta(\varepsilon): \forall{x \in D(f), \ 0<|x-a|<\delta \implies |f(x)- b|< \frac{\varepsilon}{2}}}
}$$
Пусть ${\displaystyle x', \ x'' \in \stackrel{ \circ }{ U }_{ \delta }(a) \cap D(f) \implies |f(x')-b| < \frac{\varepsilon}{2}, |f(x'')-b| < \frac{\varepsilon}{2}}$
Тогда
$$\displaylines{
|f(x')-f(x'')| \leq |f(x')-b| + |b-f(x'')|< \frac{\varepsilon}{2}+\frac{\varepsilon}{2}= \varepsilon
}$$
2. ${\displaystyle \impliedby}$. Пусть ${\displaystyle f}$ удовлетворяет условию Коши в точке ${\displaystyle a}$. Возьмем ${\displaystyle \forall{x_{n} \in D(f), \ x_{n} \ne a, \ x_{n} \to a}}$. Зафиксируем ${\displaystyle \forall{\varepsilon>0}}$ ${\displaystyle \exists U_{ \delta }(a)}$ (из условия Коши). По определению предела числовой последовательности по ${\displaystyle U_{ \delta }(a) \ \exists N(\delta) \ \forall{n \geq N(\delta)} \implies x \in \stackrel{ \circ }{ U }_{ \delta }(a)}$. Тогда 
$$\displaylines{
\forall{m, \ n \geq N(\delta)} \implies |f(x_{n})- f(x_{ m })| < \varepsilon \implies f(x_{n}) - \text{ фундаментальна } \implies  \exists\lim_{ n \to \infty } {f(x_{n})} < \infty
}$$
Следовательно ${\displaystyle \exists\lim_{ x \to a } {f(x)}}$. Доказательство окончено.

