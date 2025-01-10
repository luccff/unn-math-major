### Сформулировать определения по Коши и по Гейне и дать геометрические интерпретации следующих объектов: односторонние пределы, бесконечные пределы, предел при ${\displaystyle x \to \infty, \ x \to + \infty, \ x \to - \infty}$.
---
**Односторонние пределы по Коши:**
1. Стремление слева:
$$\displaylines{
\lim_{ x \to a^{ - } }f(x) = L \iff  \bigg [\forall \varepsilon > 0 \ \ \exists \delta > 0 : \forall x \quad a-\delta < x < a \implies |f(x) - L| < \varepsilon \bigg]
}$$
2. Стремление справа:
$$\displaylines{
\lim_{ x \to a^{ + } }f(x) = L \iff  \bigg [\forall \varepsilon > 0 \ \ \exists \delta > 0 : \forall x \quad a<x<a+\delta \implies |f(x) - L| < \varepsilon \bigg]
}$$

**Односторонние пределы по Гейне:**
1. Стремление слева:
$$\displaylines{
 \lim_{ x \to a^{ - } } f(x)= L \iff  \bigg[\forall \{ x_{ n } \} :  x_{n} \underset{n \to  \infty}{\longrightarrow} a, \ x_{n} < a, \quad x_{ n } \neq a \quad \text{и} \quad \{ f(x_{n}) \} \underset{n \to  \infty}{\longrightarrow} L \bigg]
}$$
2. Стремление справа:
$$\displaylines{
\lim_{ x \to a^{ + } } f(x)= L \iff  \bigg[\forall \{ x_{ n } \} :  x_{n} \underset{n \to  \infty}{\longrightarrow} a, \ x_{n} > a, \quad x_{ n } \neq a \quad \text{и} \quad \{ f(x_{n}) \} \underset{n \to  \infty}{\longrightarrow} L \bigg]
}$$
**Бесконечные пределы**:
1. Определение по Коши:
$$\displaylines{
\lim_{ x \to a } {f(x)} = + \infty \iff \forall\varepsilon>0 \ \exists\delta>0: \forall{x \in \stackrel{ \circ }{ U }(a) \implies  f(x)>M} \\
\lim_{ x \to a } {f(x)} = - \infty \iff \forall\varepsilon<0 \ \exists\delta>0: \forall{x \in \stackrel{ \circ }{ U }(a) \implies  f(x)<M}
}$$
2. Определение по Гейне:
$$\displaylines{
\lim_{ x \to a } {f(x)} = + \infty \iff  \forall{\{ x_{n} \} \to  a, \  x_{n} \neq  a} \implies \{ f(x_{n}) \} \to  + \infty \\
\lim_{ x \to a } {f(x)} = - \infty \iff  \forall{\{ x_{n} \} \to  a, \  x_{n} \neq  a} \implies \{ f(x_{n}) \} \to  - \infty
}$$
**Пределы при** ${\displaystyle x \to \pm \infty}$:
1. Определение по Коши
$$\displaylines{
\lim_{ x \to +\infty } {f(x)} = L \iff  \forall{\varepsilon>0} \ \exists N>0: \forall{x > N} \implies  |f(x) - L| < \varepsilon \\
\lim_{ x \to -\infty } {f(x)} = L \iff  \forall{\varepsilon>0} \ \exists N>0: \forall{x < N} \implies  |f(x) - L| < \varepsilon \\
}$$
2. Определение по Гейне
$$\displaylines{
\lim_{ x \to +\infty } {f(x)} = L \iff \forall{\{ x_{n} \}} \to  + \infty \implies \{ f(x_{n}) \} \to  L\\
\lim_{ x \to -\infty } {f(x)} = L \iff \forall{\{ x_{n} \}} \to  - \infty \implies \{ f(x_{n}) \} \to  L
}$$
