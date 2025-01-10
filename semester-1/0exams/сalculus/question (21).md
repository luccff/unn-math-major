### Предел композиции (сложной функции). Доказать.
---
**Теорема**. Пусть функции ${\displaystyle g \wedge f}$ определены в окрестностях точек ${\displaystyle a \wedge L}$ соответственно, и выполняется следующее:
$$\displaylines{
\begin{aligned}
&\exists \lim_{ x \to a } {g(x)} = L \\
&\exists \lim_{ y \to L } {f(y)} = M \\
&\exists \stackrel{ \circ }{ U }(a): g(x) \neq  L
\end{aligned}
}$$
Тогда существует ${\displaystyle \lim_{ x \to a } {f(g(x))} = M}$

*Доказательство*:
1. ${\displaystyle \lim_{ x \to a } {g(x)} = L}$
По определению:
$$\displaylines{
\forall{\varepsilon' > 0} \exists \delta'>0: \forall{x} (0<|x-a|<\delta') \implies  |g(x)-L| < \varepsilon'
}$$
2. ${\displaystyle \lim_{ y \to L } {f(y)} = M}$
По определению:
$$\displaylines{
\forall{\varepsilon > 0} \exists \delta>0: \forall{x} (0<|y - L|<\delta) \implies  |f(y) - M| < \varepsilon
}$$
3. Пусть ${\displaystyle \varepsilon > 0}$ задано, тогда по пункту 2 ${\displaystyle \exists \delta > 0: |y - L| < \delta \implies |f(y) - M| < \varepsilon}$
4. Положим ${\displaystyle \varepsilon' = \delta}$, тогда по пункту 1 ${\displaystyle \exists \delta'>0: 0<|x-a|<\delta' \implies |g(x)- L|<\varepsilon' = \delta}$
5. Тогда ${\displaystyle \forall{x}}$ удовлетворяющих условию ${\displaystyle 0<|x-a|<\delta'}$ имеем ${\displaystyle |g(x)-L| < \delta}$, по определению предела функции ${\displaystyle f}$ это означает, что ${\displaystyle (|f(g(x))-M| < \varepsilon)}$
Таким образом:
$$\displaylines{
\forall{\varepsilon>0} \ \exists \delta' > 0: \forall{x} \ ( 0< |x-a| < \delta') \implies  ( |f(g(x)- M)| < \varepsilon ) \implies  \lim_{ x \to a } {f(g(x))} = M
}$$
