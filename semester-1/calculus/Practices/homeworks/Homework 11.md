# Exercise 143
**Exercise 143.4:**
$$\displaylines{
x_{ n } = \frac{1}{1 \cdot 2} - \frac{1}{2 \cdot 3} + \dots + \frac{(-1)^{ n - 1 }}{n \cdot (n + 1)} \\ 
|x_{ n + p } - x_{ n }| = \frac{(-1)^{ n }}{(n + 1) \cdot (n + 2)} + \frac{(-1)^{ n + 1 }}{(n + 2) \cdot (n + 3)} + \dots + \frac{(-1)^{ n + p - 1}}{(n + p) \cdot (n + p + 1)} \leq \\
\leq | \frac{1}{(n + 1) \cdot (n + 2)} + \dots + \frac{1}{(n + p) \cdot (n + p + 1) } | \leq  \frac{1}{(n + 1)^{2}} + \dots + \frac{1}{(n + p)^{2}}  \leq \frac{1}{n} \\ 
\frac{1}{n} < \epsilon \\ 
n > \frac{1}{\epsilon} \\ 
n(\epsilon) = \left[ \frac{1}{\epsilon} \right] + 1
}$$

# Exercise 149
**Exercise 149.1:**
$$\displaylines{
\sum_{ k = 1 }^{ n } \frac{\sin k \alpha}{k \cdot (k + 1)}, \ \ \alpha \in \mathbb{R} \\ 
|x_{ n + p } - x_{ n }| = | \frac{\sin ((n + 1) \cdot \alpha)}{(n + 1) \cdot (n + 2)} + \dots + \frac{\sin((n + p) \cdot \alpha)}{(n + p) \cdot (n + p + 1)} | \leq \frac{1}{(n + 1)^{2}} + \dots + \frac{1}{(n + p)^{2}} < \frac{1}{n} \\ 
\frac{1}{n} < \epsilon \\ 
n > \frac{1}{\epsilon} \\ 
n(\epsilon) = \left[ \frac{1}{\epsilon} \right] + 1
}$$

**Exercise 149.2:**
$$\displaylines{
\sum_{ k = 1 }^{ n } \frac{a_{ k }}{k^{2}} \text{, где } |a_{ k }| \leq C \\ 
|x_{ n + p } - x_{ n }| = | \frac{a_{ n + 1 }}{(n + 1)^{2}} + \dots + \frac{a_{ n + p }}{(n + p)^{2}} | \leq \frac{C}{(n + 1)^{2}} + \dots + \frac{C}{(n + p)^{2}} = C \cdot \left( \frac{1}{(n + 1)^{2}} + \dots \frac{1}{(n + p)^{2}} \right) < \frac{C}{n} \\ 
\frac{C}{n} < \epsilon \\ 
n > \frac{C}{\epsilon} \\ 
n(\epsilon) = \left[ \frac{C}{\epsilon} \right] + 1
}$$

# Exercise 147
**Exercise 147.1:**
$$\displaylines{
 \text{Anti Criterion: } \exists \epsilon > 0 : \forall N \in \mathbb{N} \ \ \exists n > N, \ \ \exists p \in \mathbb{N} \implies |x_{ n + p } + x_{ n }| \geq \epsilon \\ 
x_{ n } = 0.2^{ (-1)^{ n } \cdot n } = 
\begin{cases}
0.2^{ n }, \ \ \text{n is even} \\
5^{ n }, \ \ \text{n is odd}
\end{cases} \\ 
\text{When n is even: } \underset{ n \to \infty }{ 0.2^{ n } \to 0 } \\ 
\text{When n is odd: } \underset{ n \to \infty }{ 5^{ n } \to \infty } \\ 
\text{Therefore, the sequence alternates between values that grow very large and values that shrink to zero.} \\ 
|x_{ n + 1} - x_{ n }| = 5^{ n + 1 } - \frac{1}{5^{ n }} \geq 5^{ n } - \frac{1}{5^{ n }} \geq n - \frac{1}{n} > \epsilon \\ 
n - \frac{1}{n} \geq \epsilon = 0 \\ 
n - \frac{1}{n} \geq 0 \\ 
\frac{n^{2} - 1}{n} \geq 0 \text{ – always} \\ 
n(N) = N + 1 \\ 
p(n) = n + 1
}$$
\

