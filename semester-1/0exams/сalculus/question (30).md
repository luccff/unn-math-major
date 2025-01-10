### Непрерывность сложной функции. Непрерывность элементарных функций. Всё с доказательствами.
---
Пусть функция ${\displaystyle f(x)}$ имеет предел в точке ${\displaystyle y_{0}}$ при ${\displaystyle  x \to x_{0}}$, и ${\displaystyle f(x_{ 0 }) = y_{ 0 }}$ функция ${\displaystyle g}$ непрерывна в точке ${\displaystyle y_{0}}$, тогда существует ${\displaystyle \lim_{ x \to x_{0} } {g(f(x))} = g(y_{0})}$.
Доказательство:
$$\displaylines{ \forall \varepsilon > 0 \, \exists \delta > 0 : |y - y_{0}| < \delta \implies |g(y) - g(y_{0})| < \varepsilon,\\ \forall \varepsilon > 0 \, \exists \delta > 0 \, \exists \gamma > 0 :  |x - x_{0}| < \gamma \implies |f(x) - y_{0}| < \delta,\\ \implies \forall \varepsilon > 0 \, \exists \gamma > 0 : 0 < |x - x_{0}| < \gamma \implies |g(f(x)) - g(y_{0})| < \varepsilon. }$$

Непрерывность элементарных функций.

1. Непрерывность постоянной функции:
$$\displaylines{ 
\begin{aligned}
&\text{Дано: функция } f(x) = C, \text{ где } C \in \mathbb{R}. \text{ Необходимо доказать, что } \lim_{x \to x_0} f(x) = C. \\
&\\
&\text{Определение предела: } \forall \varepsilon > 0 \, \exists \delta > 0 : 0 < |x - x_0| < \delta \implies |f(x) - C| < \varepsilon. \\ 
&\\
&\text{Подставим } f(x) = C:  |f(x) - C| = |C - C| = 0. \\ 
&\\
&\text{Следовательно, } |f(x) - C| < \varepsilon \text{ для любого } \varepsilon > 0, \text{ вне зависимости от } x \text{ и } \delta. \\ 
&\\
&\text{Выбираем любое } \delta > 0. \text{ Тогда условие } 0 < |x - x_0| < \delta \implies |f(x) - C| < \varepsilon \text{ выполняется.} \\ 
&\\
&\text{Следовательно, } \lim_{x \to x_0} f(x) = C. 
\end{aligned}
}$$
2. Непрерывность ${\displaystyle f(x) = x}$

$$\displaylines{
\begin{aligned}
&\text{Дано: функция } f(x) = x. \text{ Необходимо доказать, что } \lim_{x \to x_0} f(x) = x_0. \\
&\\
&\text{Определение предела: } \forall \varepsilon > 0 \, \exists \delta > 0 : 0 < |x - x_0| < \delta \implies |f(x) - x_0| < \varepsilon. \\ 
&\\
&\text{Подставим } f(x) = x:  |f(x) - x_0| = |x - x_0|. \\ 
&\\
&\text{Для любого } \varepsilon > 0 \text{ выберем } \delta = \varepsilon. \\
&\\
&\text{Тогда при } 0 < |x - x_0| < \delta \text{ имеем } |f(x) - x_0| = |x - x_0| < \delta = \varepsilon. \\
&\\
&\text{Следовательно, } \lim_{x \to x_0} f(x) = x_0.
\end{aligned}
}$$

3. Непрерывность многочлена
Многочлен имеет вид:
$$\displaylines{
P(x) = a_{n}x^{ n } + a_{n-1} x^{ n-1 } + \dots + a_{1}x+a_{0} 
}$$
Доказательство:  каждый коэффициент ${\displaystyle a_{k}x^{ k }}$ является произведением непрерывных функций: константы ${\displaystyle a_{k}}$, которая непрерывна в силу пункта 1 и степенной функции ${\displaystyle x^{ k }}$,  которая непрерывна в силу пункта 2 + дополнение, что произведение непрерывных функций будет непрерывная функция. По индукции сумма конечного числа непрерывных функций дает непрерывную функцию. Следовательно многочлены непрерывны на ${\displaystyle \mathbb{R}}$.

4. Непрерывность рациональных функций.
Рациональная функция ${\displaystyle R(x)}$ имеет вид:
$$\displaylines{
R(x) = \frac{P(x)}{Q(x)}, \  
}$$
где ${\displaystyle P(x), \ Q(x)}$ многочлены. В силу того, что многочлены непрерывны на ${\displaystyle \mathbb{R}}$ (пункт 3), частное этих функций непрерывно в тех точках, где ${\displaystyle Q(x) \neq 0}$.

5. Непрерывность показательной функции ${\displaystyle f(x) = a^{ x }}$. 

Доказательство не по индукции: пусть ${\displaystyle a^{ x }}$ имеет вид
$$\displaylines{
a^{ x } = \exp(x\ln(a)) 
}$$
Экспонента непрерывна как предел частичных сумм ряда Тейлора:
$$\displaylines{
\exp(x) = \sum_{n=0}^{\infty} \frac{x^{ n }}{n!}
}$$
Этот ряд сходится равномерно на любом компактном интервале, что доказывает её непрерывность. Поскольку ${\displaystyle a^{ x }}$ является суперпозицией непрерывных функций ${\displaystyle \exp(x)}$ и ${\displaystyle \ln(a)}$, она также непрерывна.

6. Непрерывность логарифмической функции.
${\displaystyle \ln(x)}$ является обратной функцией к ${\displaystyle \exp(x)}$ и определяется как решение уравнения:
$$\displaylines{
\exp(y) = x
}$$
Доказательство: Поскольку ${\displaystyle \exp(x)}$ строго монотонна и непрерывна на ${\displaystyle \mathbb{R}}$, её обратная функция также непрерывна на ${\displaystyle (0;+\infty)}$

7. Непрерывность функций ${\displaystyle \sin{(x)}, \ \cos{(x)}}$
Функции ${\displaystyle \sin{(x)}}$ и ${\displaystyle \cos{(x)}}$ задаются через ряды Тейлора:
$$\displaylines{
\sin{(x)} = \sum_{n=0}^{\infty} \frac{(-1)^{ n }x^{ n+1 }}{(n+1)!}, \quad \cos{(x)} = \sum_{n=0}^{\infty} \frac{(-1)^{ n }x^{ 2n }}{2n!}  
}$$
Доказательство: эти ряды сходятся равномерно на любом конечном интервале. Поскольку частичные суммы рядов являются многочленами (а значит, непрерывными функциями), то предел этих частичных сумм будет также непрерывен. 

8. Обратные тригонометрические функции
Функции ${\displaystyle \arcsin{(x)}, \ \arccos{(x)}, \ \arctan{(x)}, \text{ arccot}{(x)}}$ непрерывны на своих областях определения, так как они являются обратными к функциям ${\displaystyle \sin{(x)}, \ \cos{(x)}, \ \tan{(x)}, \ \cot{(x)}}$, которые строго монотонны и непрерывны на соответствующих интервалах.