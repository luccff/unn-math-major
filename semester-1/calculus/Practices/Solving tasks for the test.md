### 1) Метод математической индукции.

---
Доказать равенство ${1\cdot2 + 2 \cdot 5 + \dots + n(3n-1) = n^{ 2 }(n+1), \quad n \in\mathbb{N}}$

1. База индукции: ${ n = 1}$
$$\displaylines{
1(3\cdot 1 - 1) = 1^{ 2 }(1+1) \\
2 = 2
}$$
2. Индукционное предположение: предположим, что для ${n = k}$ выполняется:
$$\displaylines{
1\cdot2 + 2 \cdot 5 + \dots + k(3k-1) = k^{ 2 }(k+1)
}$$
3. Индукционный переход: докажем, что для ${n = k+1}$ выполняется:
$$\displaylines{
1\cdot2 + 2 \cdot 5 + \dots + (k+1)(3k+2) = (k+1)^{ 2 }(k+2)
}$$
Левая часть: 
$$\displaylines{
S_{ k+1 } = S_{ k } + (k+1)(3k+2) \\
S_{ k+1 } = k^{ 2 }(k+1)+(k+1)(3k+2) = (k+1)(k^{ 2 }+3k+2) \\
S_{ k+1 } = (k+1)(k+1)(k+2) = (k+1)^{ 2 }(k+2)
}$$
Левая часть равна правой части ${\implies}$ равенство доказано:
$$\displaylines{
{1\cdot2 + 2 \cdot 5 + \dots + n(3n-1) = n^{ 2 }(n+1), \quad n \in\mathbb{N}}
}$$
---
Доказать равенство: ${1\cdot2 + 2\cdot3+ \dots+ n(n-1)=\dfrac{n(n-1)(n+1)}{3}, \quad n \in\mathbb{N}}$
1. База индукции:
$$\displaylines{
0 = 0
}$$
2. Предположение:
$$\displaylines{
1\cdot2 + 2\cdot3 + \dots + k(k-1)=\dfrac{k(k-1)(k+1)}{3}
}$$
3. Пусть для ${n = k+1}$ выполняется:
$$\displaylines{
1\cdot2 + 2\cdot3 + \dots + k(k+1)=\dfrac{k(k+1)(k+2)}{3} \\
S_{ k+1 } = \dfrac{k(k-1)(k+1)}{3} + k(k+1) \\
S_{ k+1 } = k(k+1)\cdot \left( \frac{k+2}{3}  \right) = \frac{k(k+1)(k+2)}{3} 
}$$
Левая часть равна правой части ${\implies}$ равенство доказано:
$$\displaylines{
{1\cdot2 + 2\cdot3+ \dots+ n(n-1)=\dfrac{n(n-1)(n+1)}{3}, \quad n \in\mathbb{N}}
}$$
Доказать неравенство: ${(1+x)^{ n } \geq 1+ nx, \ x>-1, \ n \in \mathbb{N}}$
1. База индукции: ${ n = 1}$ 
$$\displaylines{
(1+x)^{ 1 } \geq 1+x \\
1+x\geq  1+x
}$$
2. Предположение: ${n = k}$ 
$$\displaylines{
(1+x)^{ k } \geq 1+kx
}$$
3. Переход: ${n = k+1}$
$$\displaylines{
(1+x)^{ k+1 } \geq 1+ xk+x \\
\text{ Левая часть: } (1+x)^{ k }\cdot (1+x) \\
\text{ по предположению } (1+x)^{ k } \geq  1+kx \implies (1+x)^{ k+1 } \geq (1+kx)(1+x) \\
(1+kx)(1+x) = 1+x+kx+kx^{ 2 } \\
\\
1 + x(k+1)+kx^{ 2 }\geq 1+x(k+1) \\
\text{ Так как  }x\geq -1, \ \text{ то } kx^{ 2 } \geq 0 \implies  \text{ доказано }
}$$
---
### 2) Доказать ограниченность и неограниченность последовательности:

Доказать ограниченность: ${x_{n} = \dfrac{(-1)^{ n }n+10}{\sqrt{ n^{ 2 }+3 }}}$
