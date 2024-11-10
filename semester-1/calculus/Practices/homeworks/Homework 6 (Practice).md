# Part 1 
## Exercise 299 
### Point 2 
$$\displaylines{
x_{ n } = \frac{3n + 4 \nearrow}{n + 2 \nearrow} \\ 
\begin{aligned}
x_{ n + 1 } - x_{ n } &\vee 0 \\
\frac{3n + 7}{n + 3} - \frac{3n + 4}{n + 2} &\vee 0 \\ 
\frac{2}{(n + 3) \cdot (n + 2)} &\vee 0 \\ 
2 &\vee 0 \\
2 &> 0 \\ 
x_{ n + 1 } - x_{ n } &> 0 \implies x_{ n } \nearrow
\end{aligned} 
}$$

### Point 4 
$$\displaylines{
x_{ n } = n^{ 3 } - 6n^{2} \\ 
\begin{aligned}
x_{ n + 1 } - x_{ n } &\vee 0 \\ 
(n + 1)^{ 3 } - 6 \cdot (n + 1)^{2} - n^{ 3 } + 6n^{2} &\vee 0 \\ 
3n^{2} - 9n - 5 &\vee 0 \\ 
\end{aligned} \\ 
3x^{2} - 9x - 5 = 0 \\
x_{ 1 } = \frac{9 - \sqrt{ 141 }}{6} < 0, \ \ x_{ 2 } = \frac{9 + \sqrt{ 141 }}{6} \\ 
3 < x_{ 2 } < 4 \implies x_{ n } \nearrow \ \ (n \geq 4)
}$$

## Exercise 300, Point 2 
$$\displaylines{
x_{ n } = \sqrt{ n + 2 } - \sqrt{ n + 1 } \\ 
\begin{aligned}
x_{ n + 1 } - x_{ n } &\vee 0 \\ 
(\sqrt{ n + 3 } - \sqrt{ n + 2 }) - (\sqrt{ n + 2 } - \sqrt{ n + 1 }) &\vee 0 \\ 
\frac{(n + 3) - (n + 2)}{\sqrt{ n + 3 } + \sqrt{ n + 2 }} - \frac{(n + 2) - (n + 1)}{\sqrt{ n + 2 } + \sqrt{ n + 1 }} &\vee 0 \\ 
\frac{1}{\sqrt{ n + 3 } + \sqrt{ n + 2 }} - \frac{1}{\sqrt{ n + 2 } + \sqrt{ n + 1 }} &\vee 0 \\ 
\sqrt{ n + 3 } > \sqrt{ n + 2 } > \sqrt{ n + 1 } \\ 
\frac{1}{\sqrt{ n + 3 } + \sqrt{ n + 2 }} - \frac{1}{\sqrt{ n + 2 } + \sqrt{ n + 1 }} &< 0 \\ 
x_{ n + 1 } - x_{ n } &< 0 \implies x_{ n } \searrow 
\end{aligned} 
}$$

## Exercise 301, Point 7 
$$\displaylines{
x_{ n } = \frac{2^{ n } \nearrow}{n \nearrow} \\ 
x_{ 1 } = \frac{2}{1} = 2 \\ 
x_{ 2 } = \frac{4}{2} = 2 \\ 
x_{ 3 } = \frac{8}{3} \\ 
\dots \\ 
\begin{matrix}
\text{Первые члены последовательности увеливаются} \\
\text{Порядок роста степенной функции выше, чем у линейной}
\end{matrix} \implies x_{ n } \nearrow
}$$

# Part 2 
## Limit 
$$\displaylines{
\lim_{ n \to \infty } A \Leftrightarrow \forall \epsilon > 0 \ \ \exists N \in \mathbb{N} \ \ \forall n > N \ \ |x_{ n } - A| < \epsilon
}$$
## Exercise 1 
### Point 3
$$\displaylines{
x_{ n } = \frac{(-1)^{ n + 1 }}{n} \\ 
\lim_{ n \to \infty } x_{ n } = 0 \\ 
|x_{ n } - 0| = |x_{ n }| = \frac{|(-1)^{ n + 1 }|}{n} = \frac{1}{n} \\ 
\frac{1}{n} < \epsilon \\ 
n  > \frac{1}{\epsilon} \\ 
N(\epsilon) = \left[ \frac{1}{\epsilon} \right] + 1 
}$$

### Point 4
$$\displaylines{
x_{ n } = \frac{2 + (-1)^{ n }}{n} \\ 
\lim_{ n \to \infty } x_{ n } = 0 \\ 
|x_{ n } - 0| = |x_{ n }| = \frac{2 + (-1)^{ n }}{n} < \frac{3}{n}< \epsilon \\ 
\frac{3}{n} < \epsilon \\ 
n > \frac{3}{\epsilon} \\ 
N(\epsilon) = \left[ \frac{3}{\epsilon} \right] + 1
}$$
### Point 6
$$\displaylines{
x_{ n } = \frac{1}{n} \cdot \sin \frac{\pi n}{2} \\ 
\lim_{ n \to \infty } x_{ n } = 0 \\ 
|x_{ n } - 0| = |x_{ n }| = | \frac{1}{n} \cdot \sin \frac{\pi n}{2} | = \frac{1}{n} \cdot | \sin \frac{\pi n}{2} | < \frac{1}{n} \cdot 1 < \epsilon \\ 
\frac{1}{n} < \epsilon \\ 
n > \frac{1}{\epsilon} \\ 
N(\epsilon) = \left[ \frac{1}{\epsilon} \right]  + 1
}$$

## Exercise 2 
### Point 2 
$$\displaylines{
\lim_{ n \to \infty } \frac{n}{2n + 1} = \frac{1}{2} \\ 
\lim_{ n \to \infty } \frac{n}{2n + 1} = \lim_{ n \to \infty } \frac{1}{2 + \frac{1}{n}^{ \to 0 }} = \frac{1}{2}
}$$

### Point 3
$$\displaylines{
\lim_{ n \to \infty } \frac{3n}{2n - 1} = \frac{3}{2} \\ 
\lim_{ n \to \infty } \frac{3n}{2n - 1} = \lim_{ n \to \infty } \frac{3}{2 - \frac{1}{n}^{ \to 0 }} = \frac{3}{2}
}$$

## Exercise 8 
### Point 1
$$\displaylines{
x_{ n } = \frac{n^{2} - 1}{n^{ 3 }} \\ 
\lim_{ n \to \infty } \frac{n^{2} - 1}{n^{ 3 }} = \lim_{ n \to \infty } \left( \frac{1}{n}^{ \to 0 } - \frac{1}{n^{ 3 }}^{  \to 0 } \right) = 0 
}$$

### Point 2 
$$\displaylines{
x_{ n } = \frac{2n + 3}{n^{2}} \\ 
\lim_{ n \to \infty } \frac{2n + 3}{n^{2}} = \lim_{ n \to \infty } \frac{2 + \frac{3}{n}^{ \to0 }}{n} = 0
}$$