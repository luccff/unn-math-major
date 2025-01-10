### Бесконечно малая функция. Операции над бесконечно малыми функциями. Доказать.
---
*Определение*. Функция ${\displaystyle f(x)}$ называется **бесконечно малой** при ${\displaystyle x \to a}$, если её предел в этой точке равен нулю (${\displaystyle \lim_{ x \to a } {f(x)} = 0}$)
$$\displaylines{
\forall{\varepsilon>0} \ \exists\delta>0: \forall{x \in  \stackrel{ \circ }{ U }_{ \delta }(a)} \implies  |f(x)| < \varepsilon
}$$
Теорема 1. Алгебраическая сумма конечного числа бесконечно малых функций есть бесконечно малая функция.
Доказательство: пусть ${\displaystyle \alpha(x) \wedge \beta(x)}$ - бесконечно малые функции при ${\displaystyle  x \to a}$
$$\displaylines{
\begin{aligned}
& 1) \ \lim_{ x \to a } {\alpha(x)} = 0 \iff  \forall{\varepsilon} > 0  \ \exists \delta_{ 1 } > 0 \ \forall{x} \in \stackrel{ \circ }{ U }_{ \delta_{ 1 } }(a) \implies  |\alpha(x)| < \frac{\varepsilon}{2} \\
& 2) \ \lim_{ x \to a } {\beta(x)} = 0 \iff  \forall{\varepsilon} > 0  \ \exists \delta_{ 2 } > 0 \ \forall{x} \in \stackrel{ \circ }{ U }_{ \delta_{ 2 } }(a) \implies  |\beta(x)| < \frac{\varepsilon}{2}
\end{aligned}
}$$
Обозначим ${\displaystyle \delta = \min(\delta_{ 1 }, \ \delta_{ 2 })}$. Тогда ${\displaystyle \forall{x \in \stackrel{ \circ }{ U }}_{ \delta }(a) \implies 1, \ 2}$
$$\displaylines{
|\alpha(x)+ \beta(x)| \leq |\alpha(x)| + |\beta(x)| < \frac{\varepsilon}{2} + \frac{\varepsilon}{2} = \varepsilon
}$$
Следовательно ${\displaystyle \lim_{ x \to a } {(\alpha(x) + \beta(x)) = 0 \implies \alpha(x) + \beta(x)}}$ бесконечно малая при ${\displaystyle x \to a}$

Теорема 2. Произведение ограниченной функции на бесконечно малую функцию есть бесконечно малая функция.
Доказательство: пусть ${\displaystyle \alpha(x)}$ бесконечно малая функция при ${\displaystyle x \to a}$:
$$\displaylines{
\forall{\varepsilon> 0} \ \exists\delta_{ 1 } \ \forall{x} \in  \stackrel{ \circ }{ U }_{ \delta_{ 1 } }(a) \implies |\alpha(x)| < \frac{\varepsilon}{m} \ (*)
}$$
Пусть ${\displaystyle f(x)}$ ограниченная функция при ${\displaystyle x \to a}$:
$$\displaylines{
\forall{\varepsilon>0} \ \exists\delta_{ 2 } > 0 \ \forall{x \in \stackrel{ \circ }{ U }_{ \delta_{ 2 } }} \ \exists M>0: \ |f(x)| \leq M (**)
}$$
Обозначим ${\displaystyle \delta = \min(\delta_{ 1 }, \ \delta_{ 2 })}$, тогда
$$\displaylines{
\forall{x \in \ \stackrel{ \circ }{ U }}_{ \delta }(a) \ \implies  (*)(**) \\
|f(x) \cdot  \alpha(x)| = |f(x)| \cdot  |\alpha(x)| < M \cdot  \frac{\varepsilon}{M} = \varepsilon
}$$
Следовательно ${\displaystyle \lim_{ x \to a } {(f(x) \cdot \alpha(x)) = 0}}$ и ${\displaystyle f(x)\cdot\alpha(x) }$ бесконечно малая при ${\displaystyle x \to a}$

Следствие 1 теоремы 2. Произведение двух бесконечно малых функций есть бесконечно малая функция, потому что любая бесконечно малая функция также будет являться ограниченной.

Следствие 2. Произведение бесконечно малой функции на бесконечно малую есть бесконечно малая функция.
