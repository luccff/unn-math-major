##### Декартово (прямое) произведение множеств. Теорема о мощности декартова произведения. Декартова степень множества. Характеристический вектор подмножества.
---
Декартовым произведением множеств ${\displaystyle A}$ и ${\displaystyle B}$ называется множество всех упорядоченных пар ${\displaystyle (a, \ b)}$, где ${\displaystyle a \in A, \ b \in B}$:
$$\displaylines{
A \times B = \{ (a, \  b) \ | a \in A, \  b \in  B \}
}$$
Множество ${\displaystyle A \times A}$ называется декартовым квадратом множества ${\displaystyle A}$ и обозначается ${\displaystyle A ^{ 2 }}$. ${\displaystyle (A \times B \neq B \times A)}$.

Теорема о мощности декартова произведения.
Если ${\displaystyle A}$ и ${\displaystyle B}$ конечные множества, то мощность их декартова произведения равна произведению их мощностей:
$$\displaylines{
|A \times B| = |A| \cdot |B| 
}$$
Доказательство:
$$\displaylines{
A = \{ x_{1}, \  x_{2}, \  \dots , \  x_{ m } \} \\
B = \{ y_{1}, \  y_{2}, \  \dots , \  y_{n} \}
}$$
$$\displaylines{
\begin{cases}
(x_{1}, \  y_{1})(x_{1}, \  y_{2})\dots (x_{1}, \  y_{n}) - n \text{ пар }  \\
\dots  \\
(x_{ m }, \  y_{1})(x_{ m }, \  y_{2})\dots (x_{ m }, \  y_{n}) - n \text{ пар }
\end{cases} \\ \\
\underbrace{ n+n+\dots +n }_{ m \text{ раз } } = m \cdot  n \\
}$$
Несколько множеств:
$$\displaylines{
A_{ 1 } \times  A_{ 2 } \times \dots \times A_{ n } = \{ (x_{1}, \  x_{2}, \ \dots , \  x_{n}) \ | \ x_{i} \in  A_{ i }, \  i = \overline{1, \  n} \}
}$$

Декартова ${\displaystyle n}$-я степень множества ${\displaystyle A}$: ${\displaystyle A^{ n } = \underbrace{ A\times A \times \dots \times A }_{ n \text{ раз } }}$. Элементы ${\displaystyle A^{ n }}$ - упорядоченные наборы (кортежи) длинны ${\displaystyle n}$.
Теорема. Если ${\displaystyle A_{ 1 }, \ A_{ 2 }, \ \dots, \  A_{ n }}$ - конечные, то ${\displaystyle |A_{ 1 } \times A_{ 2 } \times \dots \times A_{ n }| = |A_{ 1 }| \cdot |A_{ 2 }| \cdot \dots \cdot |A_{ n }|}$.
Доказательство:
${\displaystyle n = 1}$ - верно.
Пусть верна для ${\displaystyle n = k}$.
Докажем для ${\displaystyle n = k+1}$. Обозначим ${\displaystyle |A_{ 1 }| = m_{ 1 }, \ \dots, \ |A_{ k }| = m_{k}}$. По предположению ${\displaystyle |A_{ 1 } \times \dots \times A_{ k }| = m_{1} \cdot \dots \cdot m_{ k }}$. Возьмем какую-нибудь вектор-строку ${\displaystyle (x_{1}, \ x_{2}, \ \dots, \ x_{k})}$ из ${\displaystyle A_{ 1 }\times\dots\times A_{ k }}$ и припишем ${\displaystyle a_{ k+1 } \in A_{ k+1 }}$. Это можно сделать ${\displaystyle m_{ k+1 }}$ раз. Получим ${\displaystyle m_{ k+1 }}$ различных векторов из ${\displaystyle A_{ 1 } \times \dots \times A_{ k+1 }}$. Получим ${\displaystyle m_{1} \cdot \dots \cdot m_{ k+1 }}$ различных векторов ${\displaystyle \implies}$ теорема верна для ${\displaystyle n = k+1}$.


Характеристический вектор подмножества.
Пусть дано множество $S = \{{s_{1}, s_{2}, \dots, s_{n}}\}$. Для любого подмножества ${A \subseteq S}$ можно определить **характеристический вектор** как $n$-битную строку ${\mathbf{b} = (b_{1}, b_{2}, \dots, b_{n})}$, где:
$$\displaylines{
\begin{cases}
b_{i} = 1 & s_{ i } \in  A  \\
b_{i} = 0  & s_{ i } \not\in A
\end{cases}
}$$
