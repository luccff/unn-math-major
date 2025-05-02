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
$$\displaylines{
|x_{n}| = \left| \dfrac{(-1)^{ n }n+10}{\sqrt{ n^{ 2 }+3 }} \right| \leq \frac{n+10}{\sqrt{ n^{ 2 } +3}} = \frac{1+\frac{10}{n}}{\sqrt{ 1+\dfrac{3}{n^{ 2 }}  }} = \frac{1}{1} =  1
}$$



Доказать неограниченность: ${x_{n} = 2^{ n }+3}$ 
$$\displaylines{
x_{n}=2^{ n } + 3 > 2^{ n } \\
2^{ n }>C \quad n>\log_{2}(C)\\
n(C) =  \lceil\log_{2}(C) \rceil 
}$$



Пусть ${A=[0, 2)}$. Найти, если они существуют ${\sup A, \ \inf A}$. Результат обосновать.
$$\displaylines{
\sup A - \text{ наименьшая верхняя граница. } \\
x \leq  s \quad\forall{x \in A} \\ 
s'<s - \text{ то } s' \text{ не } \sup A\\
\forall{x \in A} \text{ удовл. } x<2 \implies 2 = \sup A\\ \\
\inf A - \text{ наибольшая нижняя граница. } \\
x \geq t \quad \forall{x \in A} \\
t'>t \text{ то } t' \text{ не } \inf A \\
\forall{x} \in A \text{ удовл. } x\geq 0 \implies  0 = \inf A
}$$



Пусть ${A=\{2n \ | \ n\in\mathbb{N}\}}$. Найти, если они существуют ${\sup A, \ \inf A}$. Результат обосновать.
$$\displaylines{
2 = \inf A \\
+\infty = \sup A
}$$
---
### 3) Сходимость и расходимость.
 - Доказать по определению: ${\displaystyle \lim_{ n \to \infty } {\dfrac{n^{ 2 }+1}{n^{ 2 }+2}} = 1}$
$$\displaylines{
\forall{\varepsilon > 0} \quad \exists N \in \mathbb{N} \quad \forall{n > N} : |a_{n} - L| < \varepsilon\\
\left| \frac{n^{ 2 }+1}{n^{ 2 }+2}-1  \right| = \left| \frac{(n^{ 2 }+1)-(n^{ 2 }+2)}{n^{ 2 }+2}  \right| = \left| \frac{-1}{n^{ 2 }+2}  \right| = \frac{1}{n^{ 2 }+2} \\
\frac{1}{n^{ 2 }+2}<\varepsilon \\
n^{ 2 }+2> \frac{1}{\varepsilon} \\ 
n^{ 2 }< \frac{1}{\epsilon}-2 \\
N = \lceil \sqrt{ \frac{1}{\varepsilon} -2}\rceil 
}$$
---


- Доказать расходимость последовательности ${x_{n} = (-1)^{ n }\cdot2}$
Критерий Коши:
$$\displaylines{
\forall{\varepsilon}>0 \quad \exists N \in \mathbb{N} \quad \forall{n, \ m>N}: |x_{n}-x_{ m }|<\varepsilon
}$$
Отрицание критерия Коши:
$$\displaylines{
\exists{\varepsilon}>0 \quad \forall{} N \in \mathbb{N} \quad \exists{n, \ m>N}: |x_{n}-x_{ m }|\geq \varepsilon
}$$
Пусть ${\varepsilon = 4}$
Возьмем ${n = 2k, \ m = 2k+1}$
$$\displaylines{
x_{n}=2, \ x_{ m } = -2
}$$
$$\displaylines{
|x_{n}-x_{ m }| = |2-(-2)| = 4 \geq \varepsilon = 4
}$$
Это противоречит Критерию Коши ${\implies}$ последовательность расходится.

---

- Доказать сходимость по К.К. ${x_{n} = \dfrac{\sin{(1)}}{2}+\dots+\dfrac{\sin{(n)}}{2^{ n }} = \displaystyle\sum_{k=1}^{n} \dfrac{\sin{(k)}}{2^{ k }}}$
$$\displaylines{
\forall{\varepsilon}>0 \quad \exists N \in \mathbb{N} \quad \forall{n, \ m>N}: |x_{n}-x_{ m }|<\varepsilon
}$$
$$\displaylines{
|x_{n}-x_{ m }| < \varepsilon \\
\left| x_{n}-x_{ m } \right| =  \left| \sum_{k=m+1}^{n} \frac{\sin{(k)}}{2^{ k }} \right| \leq \sum_{k=m+1}^{n} \frac{1}{2^{ k }} \leq \frac{1}{2^{ m }} \\
m>\log_{2}\left( \frac{1}{\varepsilon} \right)
}$$
---

- Доказать расходимость по К.К. ${x_{n} = \dfrac{1}{2} + \dots+ \dfrac{1}{n+1}}$
$$\displaylines{
\forall{\varepsilon>0} \quad \exists N \in \mathbb{N} \quad \forall{n, \ m} > N \hookrightarrow |x_{n}-x_{ m }| < \varepsilon \\
\exists{\varepsilon>0} \quad \forall{} N \in \mathbb{N} \quad \exists{n, \ m} > N \hookrightarrow |x_{n}-x_{ m }| \geq  \varepsilon \\
\text{ Пусть } n = 2N, \  m = N \\
|x_{n}-x_{ m }| = \left( 1+\frac{1}{2}+\dots +\frac{1}{2N+1} \right) - \left( 1 + \frac{1}{2}+\dots +\frac{1}{N+1} \right) = \\
= \frac{1}{N+2}+\frac{1}{N+3}+\dots +\frac{1}{2N+1} \geq  \frac{1}{2N+1} \cdot (N+1) = \frac{1}{2} = \varepsilon 
\\ \text{ Расходится }
}$$
---

- Доказать сходимость по теореме Вейерштрасса и найти предел ${x_{n} = \dfrac{100^{ n }}{(n+2)!}}$ 
$$\displaylines{
\frac{x_{n+1}}{x_{n}} = \frac{100^{ n+1 }}{100^{ n }} \cdot  \frac{(n+2)!}{(n+3)!} = 100\cdot \frac{1}{n+3} \\
\lim_{ n \to \infty } {\frac{100}{n+3}} = 0\\
\text{ последовательность сходится к нулю. }
}$$
---

- Доказать сходимость по теореме Вейерштрасса ${x_{n} = \dfrac{n!}{(n+2)!}}$
$$\displaylines{
x_{n} = \frac{1}{(n+2)(n+1)} \\
\text{ Ограничена снизу нулём, } x_{n+1}<x_{n} \implies  \text{ монотонно убывает } \\
\implies \text{ сходится к нулю и предел равен } \lim_{ n \to \infty } {x_{n}} = 0
}$$
---
### 4) Раскрытие неопределенностей
$$\displaylines{
\lim_{ n \to \infty } {\frac{\sqrt{ 4n^{ 3 }-n }-\sqrt[3]{ 8n^{ 6 }+n }}{\sqrt{ 4n^{ 4 }+n }-3n^{ 2 }} } = \lim_{ n \to \infty } {\frac{2n^{ 3/2 }-2n^{ 2 }}{-n^{ 2 }} } = \lim_{ n \to \infty } {\left( \frac{2n^{ 3/2 }}{-n^{ 3 }}- \frac{2n^{ 2 }}{-n^{ 2 }}  \right) } = \\
\lim_{ n \to \infty } {\left( -\frac{2}{n^{ 1/2 }} +2  \right)} = 2
}$$
$$\displaylines{
\lim_{ n \to \infty } \frac{{n^{ 4 }-(n^{ 2 }+n+1)\cdot n^{ 2 }-3n^{ 3 }}}{n-4n^{ 3 }+n^{ 2 }} = \lim_{ n \to \infty } {\frac{n^{ 4 }-n^{ 4 }-n^{ 3 }-n^{ 2 }-3n^{ 3 }}{n-4n^{ 3 }+n^{ 2 }} } = \lim_{ n \to \infty } {\frac{-4n^{ 3 }-n^{ 2 }}{n-4n^{ 3 }+n^{ 2 }} } = \lim_{ n \to \infty } {\frac{4n^{ 3 }}{4n^{ 3 }}} = 1
}$$
$$\displaylines{
\lim_{ n \to \infty } \left( {\sqrt{ n^{ 2 }+4n }-\sqrt{ n^{ 2 }+n }} \right) = \lim_{ n \to \infty } {\left( \frac{({\sqrt{ n^{ 2 }+4n }-\sqrt{ n^{ 2 }+n }})({\sqrt{ n^{ 2 }+4n }+\sqrt{ n^{ 2 }+n }})}{{\sqrt{ n^{ 2 }+4n }+\sqrt{ n^{ 2 }+n }}}  \right)} = \\
= \lim_{ n \to \infty } {\frac{n^{ 2 }+4n-n^{ 2 }-n}{{\sqrt{ n^{ 2 }+4n }+\sqrt{ n^{ 2 }+n }}} } = \lim_{ n \to \infty } {\frac{3n}{\sqrt{ n^{ 2 }\left( 1+\dfrac{4}{n} \right) } + \sqrt{ n^{ 2 }\left( 1+\dfrac{1}{n} \right) }}  } = \lim_{ n \to \infty } {\frac{3}{\left( \sqrt{ 1+\dfrac{4}{n} } + \sqrt{ 1+\dfrac{1}{n} } \right)} } = \frac{3}{\sqrt{ 1 } + \sqrt{ 1 }} = \frac{3}{2} 
}$$
$$\displaylines{
\lim_{ n \to \infty } {\frac{2n^{ n }+3n^{ 122 }+9^{ n }}{\ln(n)^{ 3 }+n^{ n }} } = \lim_{ n \to \infty } {\frac{2n^{ n }}{n^{ n }} } = 2
}$$
$$\displaylines{
\lim_{ n \to \infty } {\frac{2n-\ln(n)}{\log_{3}(9^{ n }+4)} } = \lim_{ n \to \infty } {\frac{2n}{2n} } = 1
}$$
$$\displaylines{
\lim_{ n \to \infty } {\left( \frac{2n-3}{2n+1}  \right)^{ 4n-5 }} \\
\exp\left( 4n-5\ln\left( \frac{2n-3}{2n+1}  \right) \right) \\
\ln\left( 1-\frac{4}{2n+1}  \right) \sim -\frac{4}{2n+1}\\
\exp\left( -\frac{16n-20}{2n+1}  \right) = \exp\left( - \frac{16\left( 1-\dfrac{5}{4n}  \right)}{2\left( 1+\dfrac{1}{2n}  \right)}  \right) = \exp(-8)\\
\implies \lim_{ n \to \infty } {\left( \frac{2n-3}{2n+1}  \right)^{ 4n-5 }} = e^{ -8 }
}$$
---
### 5) Предел функции.
1) Написать определение ${\displaystyle\lim_{ x \to x_{ 0 } }f(x) =A}$ и дать геометрическую интерпретацию
Рассмотрим функцию ${y = f(x)}$, которая определена на некотором промежутке ${\mathcal{X}}$, за исключением, возможно, точки ${x_{ 0 }}$
$$\displaylines{
\lim_{ x \to x_{ 0 } } {f(x) = A} \quad \forall{\varepsilon>0} \quad \exists\delta>0 \quad \forall{x \in \mathcal{X}}: (0<|x-x_{ 0 }|<\delta \implies |f(x)-A| < \varepsilon)
}$$
![[Pasted image 20241223120632.png|600]]


2) Написать определение ${\displaystyle\lim_{ x \to x_{ 0 } }f(x) =A\pm 0}$ и дать геометрическую интерпретацию
$$\displaylines{
\lim_{ x \to x_{ 0 }} {f(x)} = A \pm 0 \iff \begin{matrix}
\displaystyle\lim_{ x \to x_{ 0 }+0 } {f(x)} = A \\
\text{ или } \\
\displaystyle\lim_{ x \to x_{ 0 }-0 } {f(x)} = A
\end{matrix}
}$$
![[Pasted image 20241223121305.png]] 
![[Pasted image 20241223121316.png]] 
![[Pasted image 20241223121331.png]]
3) Доказать по определению ${\displaystyle\lim_{ x \to 1 }\dfrac{x-3}{x+1} = - 1}$
$$\displaylines{
\lim_{ x \to x_{ 0 } } {f(x) = A} \quad \forall{\varepsilon>0} \quad \exists\delta>0 \quad \forall{x \in \mathcal{X}}: (0<|x-x_{ 0 }|<\delta \implies |f(x)-A| < \varepsilon) \\
0<|x-1|<\delta \implies  \left| \frac{x-3}{x+1}-1  \right| <\varepsilon \\
\left| \frac{x-3}{x+1}  -1\right| = \left| \frac{2x-2}{x+1}  \right| =  \frac{2|x-1|}{|x+1|}  \leq 2|x-1| <\varepsilon \\
|x-1|< \frac{\varepsilon}{2} \\
\delta = \frac{\varepsilon}{2}
}$$
$$\displaylines{
\ln(1 + e^{ 2x }) = 2x + \ln(1 + e^{ -2x }) \\
\text{ при } x \to \infty\ \implies  e^{ -2x } \to 0  \hookrightarrow\ln(1+e^{ -2x }) \sim e^{ -2x } \text{ по тейлору около } e^{ -2x } \\
\lim_{ x \to \infty } {(\ln(1 + e^{ 2x })-2x)} = \lim_{ x \to \infty } ({(2x + e^{ -2x }) -2x}) = \lim_{ x \to \infty } {e^{ -2x }} = 0
}$$