### Доказать, что ${ \cancel\exists \displaystyle\lim_{ x \to 0 } {\sin{\left( \frac{1}{x} \right)}}}$
---
Доказательство:
Рассмотрим две последовательности, где ${\displaystyle n \in \mathbb{Z}}$:
$$\displaylines{
x_{n} = \frac{1}{\cfrac{\pi}{2} + 2\pi n} & \frac{1}{x_{n}} = \frac{\pi}{2} + 2\pi n \implies  \sin{\left( \frac{1}{x_{n}} \right)} = \sin{\left( \frac{\pi}{2}+ 2\pi n \right)} = 1\\
y_{n} = \frac{1}{-\cfrac{\pi}{2} + 2\pi n} & \frac{1}{y_{n}} = -\frac{\pi}{2} + 2\pi n \implies  \sin{\left( \frac{1}{y_{n}} \right)} = \sin{\left( -\frac{\pi}{2} + 2 \pi n \right)} = -1
}$$
Следовательно: ${\displaystyle f(x_{n}) = 1, \ f(y_{n}) = -1.}$
Обе последовательности ${\displaystyle  \{ x_{n} \}, \ \{ y_{n} \} \to 0 \text{ при } n \to \infty}$, но соответствующие последовательности значения функции ${\displaystyle f(x_{n}), \ f(y_{n})}$ стремятся к разным пределам, значит, что общий предел функции ${\displaystyle f(x), \ x \to 0}$ не существует, так как противоречие условию единственности предела функции по Гейне.

