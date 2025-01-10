### Объект ${\displaystyle \lim_{ x \to a } {f(x) = b}}$ определить по Коши. Написать отрицание. То же по Гейне. Всё с геометрическими интерпретациями. Доказать теорему об эквивалентности определений пределов.

**Определение предела функции по Коши.**
$$\displaylines{
\lim_{ x \to a }f(x) = b \iff  \bigg [\forall \varepsilon > 0 \ \ \exists \delta > 0 : \forall x \in D(f) \ \ 0 < |x - a| < \delta  \implies |f(x) - b| < \varepsilon \bigg]
}$$
Эта запись говорит о том, что число ${\displaystyle b}$ является пределом функции ${\displaystyle f: D(f) \to \mathbb{R}}$ при ${\displaystyle x \to a}$, если для любого эпсилон-коридора больше нуля существует такой дельта-коридор больше нуля, образ которого при отображении ${\displaystyle f}$ полностью содержится в эпсилон-коридоре.
![[Pasted image 20250105035429.png | 400]]

*Отрицание предела по Коши:*
$$\displaylines{
\lim_{x \to a} f(x) \neq b \iff \bigg[\exists \varepsilon > 0 \ \forall \delta > 0 \ \exists x \in D(f) \ \ (0 < |x - a| < \delta) \ \wedge \ (|f(x) - b| \geq \varepsilon) \bigg]
}$$

**Определение предела функции по Гейне.**
$$\displaylines{
 \lim_{ x \to a } f(x)= b \iff  \bigg[\forall \{ x_{ n } \} :  x_{n} \underset{n \to  \infty}{\longrightarrow} a, \quad x_{ n } \neq a \quad \text{и} \quad \{ f(x_{n}) \} \underset{n \to  \infty}{\longrightarrow} b \bigg]
}$$
*Отрицание определения предела функции по Гейне:*
$$\displaylines{
\lim_{x \to a} f(x) \neq b \iff \bigg[\exists \{x_n\} : x_n \underset{n \to \infty}{\longrightarrow} a, \quad x_n \neq a \quad \text{и} \quad \{f(x_n)\} \underset{n \to \infty}{\cancel{\longrightarrow}} b\bigg]
}$$

**Теорема**. Определения пределов по Коши и по Гейне эквиваленты.
Доказательство:
1. Коши ${\displaystyle  \implies}$ Гейне
Предположим, что ${\displaystyle \lim_{ x \to a } {f(x)} = b}$ по Коши. Докажем, что это определение имплицирует определение по Гейне.
По определению Коши
$$\displaylines{
\forall{\varepsilon>0} \exists \delta > 0: \forall{x \in D(f)} \quad (0<|x-a|<\delta) \implies (|f(x)-b| < \varepsilon)
}$$
Рассмотрим любую последовательность ${\displaystyle \{ x_{n} \}}$, такую что ${\displaystyle x_{n} \to a \wedge x_{n} \neq a}$ ${\displaystyle \forall{n}}$. Поскольку ${\displaystyle x_{n} \to a}$ по определению предела последовательности 
$$\displaylines{
\forall{\delta > 0} \ \exists N \in \mathbb{N} : \forall{n > N} \ |x_{n}-a| < \delta
}$$
Выберем ${\displaystyle \delta > 0}$ из условия Коши. Тогда для всех ${\displaystyle n > N}$ выполнено:
$$\displaylines{
0 < |x_{n} - a | < \delta \implies |f(x_{n})-b| < \varepsilon
}$$
Следовательно, последовательность ${\displaystyle \{ f(x_{n}) \}}$ удовлетворяет определению предела:
$$\displaylines{
\forall{\varepsilon > 0} \ \exists N \in \mathbb{N} : \forall{n > N} \ |f(x_{n})-b| < \varepsilon
}$$
Таким образом, Коши ${\displaystyle \implies}$ Гейне.

2. Гейне ${\displaystyle \implies }$ Коши
Предположим, что ${\displaystyle \lim_{ x \to a } {f(x)} = b}$ по Гейне. Докажем, что это определение имплицирует определение по Коши.
По определению Гейне, для любой последовательности ${\displaystyle \{ x_{n} \}, \ x_{n} \to a \wedge x_{n} \neq a}$ выполнено, что ${\displaystyle \{ f(x_{n}) \}} \to b$.
Предположим, что условие Коши не выполнено, это значит 
$$\displaylines{
\exists \varepsilon > 0 \ \forall \delta > 0 \ \exists x \in D(f) \ \ (0 < |x - a| < \delta) \ \wedge \ (|f(x) - b| \geq \varepsilon)
}$$
Построим последовательность ${\displaystyle \{ x_{n} \}}$, такую что ${\displaystyle x_{n} \to a \wedge \ x_{n} \neq a}$ используя отрицание:
$$\displaylines{
0< |x_{n} - a| < \frac{1}{n} \quad \wedge \quad |\{ f(x_{n}) \} - b| \geq  \varepsilon
}$$
Левое неравенство означает, что ${\displaystyle x_{n} \to a \wedge x_{n} \neq a, \ \forall{n \in \mathbb{N}}}$. Однако, ${\displaystyle |\{ f(x_{n}) \} -b| \geq\varepsilon}$ для всех ${\displaystyle n}$, что противоречит определение по Гейне ${\displaystyle (\{ f(x_{n}) \} \to b)}$, следовательно условие Коши выполнено.

Таким образом, определения предела функции по Коши и по Гейне эквивалентны. 