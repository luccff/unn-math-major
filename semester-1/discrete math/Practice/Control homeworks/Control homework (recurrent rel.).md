Task: ${x_{n} = 5x_{n-1}+14x_{n-2}, \quad x_{ 0 } = 2, \quad x_{ 1 } = 2}$
Solution: 
$$\displaylines{
x_{n} = d_{1}x_{n-1}+d_{ 2 }x_{n-2} \\
\lambda^{ 2 } = 5\lambda+14 \\
\lambda^{ 2 } - 5\lambda-14 = 0 \\
(\lambda-7)(\lambda+2) = 0 \\
\lambda_{ 1 }\neq \lambda_{ 2 } \implies  x_{n} = C_{ 1 }\lambda^{ n }_{ 1 } + C_{ 2 }\lambda^{ n }_{ 2 } \\
x_{n} = C_{ 1 }7^{ n } + C_{ 2 }(-2)^{ n }
}$$
${x_{ 0 } = 2:}$
$$\displaylines{
x_{ 0 } = C_{ 1 }+C_{ 2 } = 2
}$$
${x_{ 1 } = 2:}$
$$\displaylines{
x_{ 1 } = 7\cdot C_{ 1 } -2C_{ 2 } = 2
}$$
$$\displaylines{
\begin{cases}
C_{ 1 }+C_{ 2 } = 2 \\
7C_{ 1 }-2C_{ 2 } = 2
\end{cases} \quad \quad
\begin{matrix}
C_{ 2 } = 2-C_{ 1 } \\
7C_{ 1 } - 2(2-C_{ 1 }) = 2
\end{matrix} \\
7C_{ 1 }-4+2C_{ 1 } = 2 \\
9C_{ 1 }= 6 \\
C_{ 1 } = \frac{2}{3} \implies C_{ 2 } = 2-\frac{2}{3} = \frac{4}{3}
}$$
Answer:
$$\displaylines{
x_{n} = \frac{2}{3}\cdot 7^{ n } + \frac{4}{3}\cdot (-2)^{ n }
}$$