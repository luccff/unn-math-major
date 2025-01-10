### Найти производную функции ${\displaystyle y = \begin{cases} x^{ 2 }\sin{\left( \frac{1}{x} \right)}, \ & x\neq0 \\ 0, \ & x = 0\end{cases}}$
---
$$\displaylines{
y = \begin{cases} x^{ 2 }\sin{\left( \cfrac{1}{x} \right)}, \  & x\neq0 \\ 0, \ &  x = 0\end{cases}
}$$
Для ${\displaystyle x\neq0}$:
$$\displaylines{
y'(x) =2x\sin{\left( \frac{1}{x} \right)} + x^{ 2 }\cdot \cos{\left( \frac{1}{x} \right)} \cdot \left( -\frac{1}{x^{ 2 }} \right) =  2x\sin{\left( \frac{1}{x} \right)} - \cos{\left( \frac{1}{x} \right)}
}$$
Для ${\displaystyle x = 0}$:
$$\displaylines{
y'(0) = \lim_{ x \to 0 } {\frac{y(x)-y(0)}{x-0} } = \lim_{ x \to 0 } {\frac{x^{ 2 }\sin{\left( \cfrac{1}{x} \right)}}{x} } = \lim_{ x \to 0 } {x\sin{\left( \frac{1}{x} \right)}} \\
-1\leq \sin{\left( \frac{1}{x} \right)}\leq 1 \\
-x\leq x\sin{\left( \frac{1}{x} \right)}\leq x\\
\text{ При } x \to  0: 0\leq x\sin{\left( \frac{1}{x} \right)}\leq 0 \\
\text{ По т. о двух миллиционерах }: \lim_{ x \to 0 } {x\sin{\left( \frac{1}{x} \right)}} = 0
}$$
Ответ: $$\displaylines{
y'(x) = \begin{cases}
2x\sin{\left( \cfrac{1}{x} \right)}-\cos{\left( \cfrac{1}{x} \right)}, \   &  x\neq 0 \\
0, \   & x = 0
\end{cases}
}$$
