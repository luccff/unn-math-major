Ex. 37 (1)
$$\displaylines{
\lim_{ x \to 0 } {\frac{e^{ \sin{(x)} } - e^{ x }}{\sin{(x)}-x} } = \left[ \frac{0}{0} \right] = \lim_{ x \to 0 } {\frac{\cos{(x)}e^{ \sin{(x)} } - e^{ x }}{\cos{(x)} - 1} } = \lim_{ x \to 0 } {\frac{(-\sin{(x)}e^{ \sin{(x)}  }+ \cos{(x)}^{ 2 }e^{ \sin{(x)} }) - e^{ x }}{-\sin{(x)}} } = \\
= \lim_{ x \to 0 } {\frac{(-\cos{(x)}e^{ \sin{(x)} } -\sin{(x)}\cos{(x)}e^{ \sin{(x)} } + 2\cos{(x)}(-\sin{(x)}) e^{ \sin{(x)}  } + \cos{(x)}^{ 3 }e^{ \sin{(x)} }) - e^{ x }}{-\cos{(x)}} } = \\ =\frac{-1\cdot 1 + 0 \cdot  1 \cdot  1 + 2 \cdot  1 \cdot - \cdot  1 + 1 \cdot  1 \cdot  1 - 1}{-1} = \frac{-1+0+0+1-1}{-1} = 1 
}$$
Ex. 43 (-1/3)
$$\displaylines{
\lim_{ x \to +0 } {\frac{3+\ln(x)}{2-3\ln(\sin{(x)})} } = \lim_{ x \to +0 } {\frac{\frac{1}{x}}{-3 \cdot  \frac{\cos{(x)}}{\sin{(x)}}} } = \lim_{ x \to +0 } {\frac{-\sin{(x)}}{3x\cos{(x)}} } = -\frac{1}{3} \cdot  1 \cdot  \frac{1}{1} = -\frac{1}{3}
}$$
Ex. 48 (-2/pi)
$$\displaylines{
\lim_{ x \to +\infty } {x\ln\left( \frac{2}{\pi} \arctan{(x)} \right)} = \lim_{ x \to +\infty } {\frac{\ln\left( \frac{2}{\pi}\arctan{(x)} \right)}{\frac{1}{x}} } = \lim_{ x \to +\infty } {\frac{\frac{1}{\frac{2}{\pi}\arctan{(x)}}\cdot \frac{2}{\pi}\cdot \frac{1}{1+x^{ 2 }} }{-\frac{1}{x^{ 2 }}} } = \lim_{ x \to +\infty } {\frac{\frac{1}{\arctan{(x)}(1+x^{ 2 })}}{-\frac{1}{x^{ 2 }}} } = \lim_{ x \to +\infty } {-\frac{x^{ 2 }}{\arctan{(x)}(1+x^{ 2 })} } = \\
= \lim_{ x \to +\infty } {-\frac{x^{ 2 }}{\frac{\pi}{2}(1+x^{ 2 })} } = \lim_{ x \to +\infty } {-\frac{2x^{ 2 }}{\pi(1+x^{ 2 })} } = \lim_{ x \to +\infty } {-\frac{2x^{ 2 }}{\pi x^{ 2 }} } = -\frac{2}{\pi}
}$$
Ex. 49 (0)
$$\displaylines{
\lim_{ x \to +\infty } {x^{ n }e^{ -x^{ 3 } }} = \lim_{ x \to +\infty } {\frac{x^{ n }}{e^{ x^{ 3 } }} } = \lim_{ x \to +\infty } {\frac{nx^{ n-1 }}{e^{ x^{ 3 } }3x^{ 2 }} } = \dots = 0 \\
\text{ Т.к. степень в числителе уменьшается, а в знаменателе остается в той же форме и стремтся к нулю. }
}$$
Ex. 50 (2)
$$\displaylines{
\lim_{ x \to +\infty } {(\pi-2\arctan{(\sqrt{ x })})\sqrt{ x }} = \lim_{ x \to +\infty }\frac{2}{\sqrt{ x }} \cdot  \sqrt{ x } = 2\\
\pi-2\arctan{(\sqrt{ x })} \sim  \pi-2\left( \frac{\pi}{2} - \frac{1}{\sqrt{ x }} \right) = \frac{2}{\sqrt{ x }}
}$$
Ex. 56 (0)
$$\displaylines{
\lim_{ x \to 0 } {\left( \frac{1}{x} - \frac{1}{\arcsin{(x)}} \right)} = \lim_{ x \to 0 } {\frac{\arcsin{(x)}-x}{x\arcsin{(x)}} } = \lim_{ x \to 0 } {\frac{\frac{1}{\sqrt{ 1-x^{ 2 } }} - 1}{\arcsin{(x)}\cdot \frac{x}{\sqrt{ 1-x^{ 2 } }}} } = \lim_{ x \to 0 } {\frac{\frac{x}{(1-x^{ 2 })^{ 3/2 }}}{\frac{2}{\sqrt{ 1-x^{ 2 } }}+ \frac{x^{ 2 }}{(1-x^{ 2 })^{ 3/2 }} } } = \lim_{ x \to 0 } {\frac{x}{2-2x^{ 2 }+x^{ 2 }} } = \frac{0}{2} = 0
}$$
Ex. 59 (1/3)
$$\displaylines{
\lim_{ x \to 0 } {\left( \frac{1}{x\arctan{(x)}} - \frac{1}{x^{ 2 }} \right)} = \lim_{ x \to 0 } {\frac{x^{ 2 }-x\arctan{(x)}}{x^{ 3 }\arctan{(x)}} } = \lim_{ x \to 0 } {\frac{x(x-\arctan{(x)})}{x^{ 3 }\arctan{(x)}} } = \lim_{ x \to 0 } {\frac{x-\arctan{(x)}}{x^{ 2 }\arctan{(x)}} } = \lim_{ x \to 0 } {\frac{1-\frac{1}{1+x^{ 2 }}}{2x\arctan{(x)}+\frac{x^{ 2 }}{1+x^{ 2 }}} } = \lim_{ x \to 0 } {\frac{x^{ 2 }}{x(2\arctan{(x)}+2x^{ 2 }\cdot \arctan{(x)}+x)} } = \\
= \lim_{ x \to 0 } {\frac{x}{2\arctan{(x)}+2x^{ 2 }\cdot \arctan{(x)}+x} } = \lim_{ x \to 0 } {\frac{1}{3+4x \cdot  \arctan{(x)}}} =\frac{1}{3 + 4\cdot 0\cdot \arctan{(0)}} = \frac{1}{3}
}$$
 
Ex. 176(1,3) Определить ${\alpha, \ \beta}$ при которых функции всюду непрерывны и всюду дифференцируемы.

$$\displaylines{
1) \ y = \begin{cases}
\alpha x + \beta, & x\leq 1 \\
x^{ 2 }, \  & x>1
\end{cases}\\
\text{ Для непрерывности: }
\lim_{ x \to 1^{ - } } {y(x)} = \lim_{ x \to 1^{ + } } {y(x)} = y(1) \\
y(1) = \alpha \cdot  1 + \beta = \alpha + \beta \\
\lim_{ x \to 1^{ + } } {y(x)} = 1^{ 2 } = 1 \\
\text{ Должно выполнятся } \alpha + \beta = 1 \\
\text{ Условие дифф.: } \lim_{ x \to 1^{ - } } {y'(x)} = \lim_{ x \to 1^{ + } } {y'(x)} \\
x\leq 1: \ y'(x) = \alpha \\
x>1: \ y'(x) = 2x \\
x = 1: \ y'(1) = 2\cdot 1 - 2 \\
\text{ Для дифф. должно выполнятся: } \alpha = 2 \\
\alpha + \beta = 1 \implies 2 + \beta = 1 \implies  \beta = -1 \\
}$$
Ответ: a) ${\alpha + \beta = 1}$; б) ${\alpha = 2, \ \beta = -1}$
$$\displaylines{
3) \ y = \begin{cases}
\alpha x^{ 3 } + \beta x , \  & |x| \leq 2 \\
\left( \frac{1}{\pi} \right)\arcsin{\left( \frac{1}{x} \right)}, \  & |x|>2
\end{cases} \\
\text{ Непрерывность в точке } x = 2: \\
y(2)^{ - } = \alpha \cdot  8 + \beta \cdot 2 = 8\alpha + 2\beta \\
y(2)^{ + } = \frac{1}{\pi}\arcsin{\left( \frac{1}{2} \right)} = \frac{1}{\pi} \cdot  \frac{\pi}{6} = \frac{1}{6} \\
\boxed{8\alpha + 2\beta = \frac{1}{6}} \\
\text{ Непрерывность в точке  } x = -2: \\
y(-2)^{ - } = -8\alpha -2\beta \\
y(-2)^{ + } = -\frac{1}{6} \\
\boxed{-8\alpha - 2\beta = -\frac{1}{6}} \\
\text{ Дифференцируемость в точке } x = 2:\\
y'(x)^{ - } = 3\alpha x^{ 2 } + \beta \\
y'(2) = 3\alpha \cdot  4 + \beta = 12\alpha + \beta \\
y'(x)^{ + } = \frac{1}{\pi} \cdot  \frac{-1}{x^{ 2 }\sqrt{ 1-\left( \frac{1}{x^{ 2 }} \right) }} = \frac{1}{\pi} \cdot  \frac{-1}{x^{ 2 }\sqrt{ \frac{x^{ 2 }-1}{x^{ 2 }}  }} = \frac{1}{\pi} \cdot  \frac{-1}{\sqrt{ x^{ 2 }-1 }}\\
y'(2) = \frac{1}{\pi} \cdot  \frac{-1}{\sqrt{ 3 }} = -\frac{1}{\pi\sqrt{ 3 }}  \\
\boxed{12\alpha + \beta = -\frac{1}{\pi\sqrt{ 3 }}} \\
\text{ Дифференцируемость в точке  } x = -2: \\
y'(-2) = 12\alpha  + \beta \\
y'(-2) = -\frac{1}{\pi\sqrt{ 3 }} \\
\boxed{ 12\alpha + \beta = -\frac{1}{\pi\sqrt{ 3 }}} \\
\text{ Сложна... }
}$$
Ex. 178 Определить значение ${\alpha, \ \beta}$ при которых функция имеет производную в точке ${x = \pm1}$
$$\displaylines{
y = \begin{cases}
\arctan{(\alpha x)}, \  & |x| \leq 1 \\
\beta \text{ sign }x + \frac{x-1}{2}, \  & |x| > 1 
\end{cases} \\
\text{ Для непрерывности: } \\
y(1) = \arctan{(\alpha)} \\
y(1) = \beta \\
\boxed{\arctan{(\alpha)} = \beta} \\
y(-1) = \arctan{(-\alpha)} \\
y(-1) = -\beta-1 \\
\boxed{ \arctan{(-\alpha)} = -\beta-1} \\
\text{ Дифференцируемость: } \\
y'(x) = \frac{\alpha}{1+(\alpha x)^{ 2 }} \\
y(1) = \frac{a}{1+\alpha^{ 2 }} \\
y'(x) = 0+ \frac{1}{2} = \frac{1}{2} \\
\boxed{\frac{\alpha}{1+\alpha^{ 2 }} = \frac{1}{2}} \\
\text{ При }x = -1 \text{ аналогично. } \\
\\
\alpha = \frac{1}{2}(1+\alpha^{ 2 }) \hookrightarrow 2\alpha = 1+\alpha^{ 2 } \hookrightarrow (\alpha-1)^{ 2 } = 0 \implies \alpha = 1 \\
\arctan{(1)} = \beta \\
\beta = \frac{\pi}{4}
}$$
Ответ: ${\alpha = 1, \ \beta = \frac{\pi}{4}}$
Ex. 192(1) Найти ${f_{ \pm }'(0)}$ для функции
$$\displaylines{
f(x) = \begin{cases}
x, \  & x\leq 0 \\
\sqrt[3]{ x^{ 4 } }\ln(x), \   & x > 0
\end{cases} \\
f'_{ - }(0) = \lim_{ x \to 0^{ - } } {\frac{f(x)-f(0)}{x-0} } = \lim_{ x \to 0^{ - } } {\frac{x-0}{x-0} } = 1 \\
f_{ + }'(0) = \lim_{ x \to 0^{ + } } {\frac{f(x)-f(0)}{x-0} } = \lim_{ x \to 0^{ + } } {\frac{\sqrt[3]{ x^{ 4 } }\ln((x))-0}{x} } = \lim_{ x \to 0^{ + } } {x^{ 1/3 }\ln(x)} = 0
}$$
Ответ: ${f'_{ - } = 0; f'_{ + } = 0}$
