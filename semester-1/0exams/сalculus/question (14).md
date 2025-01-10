### Критерий Коши существования предела последовательности. Формулировка, геометрическая интерпретация, доказательство.
---
**Теорема (Критерий Коши для сходимости последовательности)**. Для того, чтобы последовательность ${\displaystyle \{ x_{n} \}}$ была сходящейся, необходимо и достаточно, чтобы она была фундаментальной.

$$\displaylines{
\forall{\varepsilon>0} \ \exists N \in  \mathbb{N} \ \forall{n, \ m > N}: \ |x_{ n } - x_{ m }| < \varepsilon
}$$
![[Pasted image 20250104195653.png | 500]]

*Доказательство*:
1. Необходимость:
Пусть последовательность ${\displaystyle x_{n} \in \mathbb{R}}$ сходится к ${\displaystyle  a \in \mathbb{R}}$. Запишем определение предела:
$$\displaylines{
\forall{\varepsilon >0} \ \exists N \in  \mathbb{N} \ \forall{n >N} : \ |x_{n} - a| < \frac{\varepsilon}{2}
}$$
Фиксируем ${\displaystyle \varepsilon}$ и берем соответствующие ${\displaystyle N}$. Возьмем произвольные ${\displaystyle m, \ n > N}$:
$$\displaylines{
|x_{n} - x_{ m }| \leq |x_{n} - a| + |a - x_{ m }| < \frac{\varepsilon}{2} + \frac{\varepsilon}{2} = \varepsilon
}$$
2. Достаточность:
Поскольку ${\displaystyle \{ x_{n} \}}$ является последовательностью Коши, то она ограничена, так как начиная с ${\displaystyle N+1}$ вся последовательность лежит в ${\displaystyle  \varepsilon}$ окрестности ${\displaystyle x_{ m }}$, ${\displaystyle m>N}$. 
По теореме Больцано-Вейерштрасса из ограниченной последовательности можно выделить сходящуюся подпоследовательность ${\displaystyle \{ x_{n_{ k }} \}}$, причем ${\displaystyle \lim_{ n \to \infty } {x_{n_{ k }}} = a}$.
Запишем условие Коши:
$$\displaylines{
\forall{\epsilon>0} \ \exists N_{ 1 } \in  \mathbb{N}  \ \forall{n, \ m > N_{ 1 }}: \ |x_{n} - x_{ m }| < \frac{\varepsilon}{2}
}$$
Запишем определение предела подпоследовательности:
$$\displaylines{
\forall{\varepsilon>0} \ \exists N_{ 2 } \in  \mathbb{N} \ \forall{k> N_{ 2 }}: \ |x_{ n_{ k } } - a| < \frac{\varepsilon}{2}
}$$
Фиксируем ${\displaystyle \varepsilon}$. Берем ${\displaystyle N_{ 1 }, \ N_{ 2 }}$. Возьмем ${\displaystyle  n> N_{ 1 }, \ k > N_{ 2 }}$, такую, что ${\displaystyle n_{ k }>N_{ 1 }}$. Тогда
$$\displaylines{
|x_{ n }- a| \leq |x_{n} - x_{n_{ k }}| + | x_{n_{ k }} - a| < \frac{\varepsilon}{2} + \frac{\varepsilon}{2} = \varepsilon
}$$
