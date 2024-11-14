Страница 175.
**Exercise 21**
$$\displaylines{
2) \ \lim_{  x \to 7 } {\frac{2x^{ 2 }-11x-21}{x^{ 2 }-9x+14}} = \lim_{ x \to 7 } {\frac{2(x-7)\left( x+\frac{3}{2} \right)}{(x-7)(x-2)}} = \lim_{ x \to 7 } {\frac{2x+3}{x-2}} = \frac{17}{5}
\\
3) \lim_{ x \to 1 } {\frac{x^{ 4 }-x^{ 3 }+ x^{ 2 }-3x+2}{x^{ 3 }-x^{ 2 }-x+1}} = \lim_{ x \to 1 } {\frac{(x-1)^{ 2 }(x^{ 2 }-x+1)}{(x-1)^{ 2 }(x+1)}} = \lim_{ x \to 1 } {\frac{x^{ 2 }-x+1}{x+1}} = \frac{4}{2} = 2 \\
4) \lim_{ x \to 1 } {\frac{x^{ 4 }-2x+1}{x^{ 8 }-2x+1}} = \lim_{ x \to 1 }{\frac{4x^{ 3 }-2}{8x^{ 7 }-2}} = \frac{4-2}{8-2} = \frac{1}{3} \text{ (по Лопиталю) }\\
5) \lim_{ x \to 1 } {\frac{x^{ 101 }-101x+100}{x^{ 2 }-2x+1}} = \lim_{ x \to 1 } {\frac{101x^{ 100 }-101}{2x-2}} = \lim_{ x \to 1 } {\frac{10100x^{ 90 }}{2}} = 5050 \text{ (по Лопиталю) } \\
}$$
**Exercise 24**
$$\displaylines{
4) \ \lim_{ x \to 1 } {\left( \frac{n}{1-x^{ n }} - \frac{k}{1-x^{ k }} \right)}, \  n, \  k \in \mathbb{N} = 
\begin{bmatrix}
t = 1-x, \ t \to 0, \ x\to0  \\
x = 1-t
\end{bmatrix} \\
x^{ n } = (1-t)^{ n }= 1-nt + \frac{n(n-1)}{2}t^{ 2 } - \dots \\
1-x^{ n } = 1-(1-t)^{ n } = nt-\frac{n(n-1)}{2}t^{ 2 }+\dots \\
1-x^{ k } = kt-\frac{k(k-1)}{2}t^{ 2 } + \dots \\
\lim_{ x \to 1 } {\left( \frac{n}{nt-\frac{n(n-1)}{2}t^{2 }+\dots} - \frac{k}{kt-\frac{k(k-1)}{2}t^{ 2 }+\dots}\right) } = \lim_{ x \to 1 } {\left( \frac{1}{t-\frac{n-1}{2}t^{ 2 }+\dots} - \frac{1}{t-\frac{k-1}{2}t^{ 2 }+ \dots} \right)} \\

\frac{1}{t-at^{ 2 }+\dots} \approx \frac{1}{t}(1+at+\dots) \\
\frac{1}{t-\frac{n-1}{2}t^{ 2 }} \approx \frac{1}{t}\left( 1+\frac{(n-1)}{2}t \right) \\
\frac{1}{t-\frac{k-1}{2}t^{ 2 }} \approx \frac{1}{t}\left( 1+\frac{(k-1)}{2}t \right) \\
\implies\left( \frac{1}{t} + \frac{n-1}{2} \right) - \left( \frac{1}{t} + \frac{k-1}{2} \right) = \frac{n-1}{2} - \frac{k-1}{2} = \frac{n-k}{2}\\
\boxed{\lim_{ x \to 1 } {\left( \frac{n}{1-x^{ n }} - \frac{k}{1-x^{ k }} \right)} = \frac{n-k}{2}}
}$$
 
**Exercise 25**

$$\displaylines{
2) \lim_{ x \to 0 } {\frac{x}{\sqrt[3]{ 1+x }-1}} = \begin{bmatrix}
y = \sqrt[3]{ 1+x } \\
y^{ 3 } = 1+x  \\
x = y^{ 3 } - 1
\end{bmatrix} = \lim_{ x \to 0 } {\frac{y^{ 3 }-1}{y-1}} = \lim_{ x \to 0 } {y^{ 2 }+y+1} = 3
}$$
$$\displaylines{
 5) \lim_{ x \to 5 } {\frac{\sqrt{ 6-x }-1}{3-\sqrt{ 4+x }}} = 3 \\
 f'(x) = (\sqrt{ 6-x }-1)' = -\frac{1}{2\sqrt{ 6-x }} \\
 g'(x) = (3-\sqrt{ 4+x })' = -\frac{1}{2\sqrt{ 4+x }} \\ 
 \implies \lim_{ x \to 5 } {\frac{\sqrt{ 4+x }}{\sqrt{ 6-x }}} = \frac{\sqrt{ 4+5 }}{\sqrt{ 6-5 }} = 3
 }$$

$$\displaylines{
  7) \lim_{ x \to 3 } {\frac{\sqrt{ x^{ 2 }-2x+6 } - \sqrt{ x^{ 2 }+2x-6 }}{x^{ 2 }-4x+3}} = -\frac{1}{3} \\
  f'(x) = \frac{2x-2}{2\sqrt{ x^{ 2 }-2x+6 }} - \frac{2x+2}{2\sqrt{ x^{ 2 }+2x-6 }} = \frac{x-1}{\sqrt{ x^{ 2 }-2x+6 }} - \frac{x+1}{\sqrt{ x^{ 2 } +2x - 6 }} \\
  g'(x) = 2x-4 \\
  f'(3) = \frac{3-1}{3} - \frac{3+1}{3} = -\frac{2}{3} \\
  g'(3) = 2 \\
  \implies \lim_{ x \to 3 } {\frac{-\frac{2}{3}}{2}} = -\frac{1}{3}
  }$$
  
$$\displaylines{
8) \lim_{ x \to 0 } {\frac{\sqrt[3]{ x+8 }-2}{\sqrt{ 1+2x  }-1}} = \frac{1}{12} \\
f'(x) = \left( (x+8)^{\frac{1}{3} } - 2\right)' = \frac{1}{3}(x+8)^{ -\frac{2}{3} } \\
g'(x) = \left( (1+2x)^{ \frac{1}{2} } - 1\right) = \frac{1}{2}(1+2x)^{ -\frac{1}{2} } \cdot 2 = (1+2x)^{ -\frac{1}{2} } \\
\implies \lim_{ x \to 0 } {\frac{\frac{1}{3}(x+8)^{ -\frac{2}{3} }}{(1+2x)^{ -\frac{1}{2} }}} = \lim_{ x \to 0 } {\frac{1}{3}\cdot(x+8)^{ -\frac{2}{3} }\cdot (1+2x)^{ \frac{1}{2}} } = \frac{1}{3}\cdot \frac{1}{4} = \frac{1}{12}


}$$
 
 
  
 
 
 
 
 