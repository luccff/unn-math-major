17.11.2024

---
### о-малое

Определение.
$$\displaylines{
f(x) = o(g(x)), \  \text{ при  } x \to  a  \iff f(x) \text{ является бесконечно малой по сравнению с }g(x), \  \text{ при } x \to  a\\
\boxed{\lim_{ x \to a } {\frac{f(x)}{g(x)} =0 }}
}$$
Пример. 
$$\displaylines{
x^{ 2 } = o(x), \  \text{ при } x \to  0 \\
\lim_{ x \to 0 } {\frac{x^{ 2 }}{x} } = \lim_{ x \to 0 } {\frac{x}{1} } = 0 \\
}$$
Обратный пример.
$$\displaylines{
x = o(x^{ 2 }), \ \text{ при } x \to  \infty \\
\lim_{ x \to \infty } {\frac{x}{x^{ 2 }}} = \lim_{ x \to \infty } {\frac{1}{x}} = 0
}$$
$$\displaylines{
o(x)+o(x) = o(x) \\ 
o(x)-o(x) = o(x) \\
\text{ Воспринимаем  }o(x) \text{ как класс функции.  } \\ \\
\text{ непр. ф. + непр. ф. = непр. ф. (не две непр.) } \\
\text{ непр. ф. - непр. ф. = непр. ф (не ноль) }
}$$

$$\displaylines{
\text{ При } x \to  0 & o(x^{ 2 }) + o(x^{ 3 }) = o(x^{ \min(2, \ 3) }) = o(x^{ 2 })\\
\text{ При } x \to \infty & o(x^{ 2 })+o(x^{ 3 }) = o(x^{ \max(2, \ 3) }) = o(x^{ 3 })\\
}$$
$$\displaylines{
\text{ На бесконечности } x^{ 3 } \gg x^{ 2 } \\
x^{ 2,5 } = o(x^{ 2 }), \ \text{ при } x \to  0? -\text{ Да,}\text{ т.к. } \lim_{ x \to 0 } {\frac{x^{ 2,5 }}{x^{ 2 }} } = \lim_{ x \to 0 } {x^{ 0,5 }} = 0  \ \ \checkmark \\
x^{ 2,5 } = o(x^{ 3 }), \  \text{ при } x \to 0? - \text{ Нет, т.к } \lim_{ x \to 0 } {\frac{x^{ 2, 5 }}{x^{ 3 }} } = \lim_{ x \to 0 } {\frac{1}{x^{ 0,5 }}} = \frac{1}{0} \neq 0  \ \ \times 
}$$
---
### O-большое

Определение.
$$\displaylines{
f(x) = O(g(x)), \  \text{ при } x \to  a, \  \text{ если } \lim_{ x \to a } {\frac{f(x)}{f(x)} } = const \neq 0
}$$
Пример.
$$\displaylines{
\sin{(2x)} = O(x), \  \text{ при  } x \to  0 \\
\lim_{ x \to 0 } {\frac{\sin{(2x)}}{x}} = 2 = const\neq 0 
}$$
---
### Формула Тейлора.
![[image_2024-11-17_20-52-34.png | 500]]
$$\displaylines{

o(x) - \text{ погрешность при приблеженных вычислениях } \\
f(x) \sim a_{ 0 } + a_{ 1 }x + a_{ 2 }x^{ 2 }+a_{ 3 }x^{ 3 } + \dots + a_{ n-1 }x^{ n-1 } + a_{n}x^{ n } = P_{ n }(x) \\
f(0) = P_{ n }(0) \hookrightarrow \boxed{f(0) = a_{ 0 }}  = 0!a_{ 0 } \hookrightarrow a_{ 0 } = \frac{f(0)}{0!} \\ \\
P_{ n }'(x) = a_{ 1 } + 2a_{ 2 }x^{ 1 }+3a_{ 3 }x^{ 2 }+4a_{ 4 }x^{ 3 }+\dots +na_{ n }x^{ n-1 } \\
f'(0) = P_{ n }'(0) \hookrightarrow \boxed{f'(0) = a_{ 1 }} = 1!a_{ 1 }  \hookrightarrow a_{ 1 } = \frac{f'(0)}{1!} \\ \\
P_{ n }''(x) = 2 \cdot 1a_{ 2 }+3\cdot 2a_{ 3 }x^{ 1 }+4\cdot 3a_{ 4 }x^{ 3 } + \dots + n(n-1)a_{ n }x^{ n-2 } \\
f''(0) = P_{ n }''(0) \hookrightarrow \boxed{f''(0) = 2\cdot  1 \cdot a_{ 2 }} = 2!a_{ 2 } \hookrightarrow a_{ 2 } = \frac{f''(0)}{2!} \\ \\
P'''_{ n }(x) = 3 \cdot 2\cdot 1 a_{ 3 } + 4 \cdot  3 \cdot  2 a_{ 4 } x^{ 1 } + \dots + n(n-1)(n-2)a_{n}x^{ n-3 } \\
f'''(0) = P_{ n }'''(o) \hookrightarrow \boxed{f'''(0) = 3 \cdot  2 \cdot  1 a_{ 3 }} = 3! a_{ 3 } \hookrightarrow a_{ 3 } = \frac{f'''(0)}{3!}\\
\vdots \\
\boxed{f^{ (n) } = n! a_{ n } }\hookrightarrow a_{ n } = \frac{f^{ (n) }(0)}{n!} 
}$$

$$\displaylines{
\boxed{
f(x) \sim \frac{f(0)}{0!}x^{ 0 } + \frac{f'(0)}{1!} x^{ 1 } + \frac{f''(0)}{2!}x^{ 2 } + \frac{f'''(0)}{3!}x^{ 3 } + \dots +\frac{f^{ (n) }(0)}{n!} x^{ n }
} \\ || \\
\boxed{
f(x) \sim \sum_{k=0}^{n} \frac{f^{ (k) }(0)}{k!}x^{ k }
} \\\\
}$$
$$\displaylines{
\boxed{
f(x) \sim \sum_{k=0}^{n} \frac{f^{ (k) }(0)}{k!}x^{ k } +o(x^{ n })
} - \text{формула Маклорена}
}$$
$$\displaylines{
\boxed{
f(x) = \sum_{k=0}^{n} \frac{f^{ (k) }(a)}{k!}(x-a)^{ k } + o((x-a)^{ n }) 
} - \text{ формула Тейлора }
}$$
---
Выведем формулу Маклорена для ${f(x) = e^{ x }}$
$$\displaylines{
f(x)  = \frac{f(0)}{0!}x^{ 0 } + \frac{f'(0)}{1!} x^{ 1 } + \frac{f''(0)}{2!}x^{ 2 } + \frac{f'''(0)}{3!}x^{ 3 } + \dots +\frac{f^{ (n) }(0)}{n!} x^{ n } + o(x^{ n })
}$$
$$\displaylines{
\begin{array}{|c|c|} \hline
k  & f^{ (k) }(x) & f^{ (k) }(0) \\
\hline 
0  & e^{ x }  & 1 \\
1  & e^{ x } & 1  \\
2 & e^{ x }  & 1 \\
\vdots  & \vdots  &  \vdots\\
n & e^{ x } & 1  \\
\hline 
\end{array} \implies \begin{matrix}
e^{ x } = \frac{1}{0!}x^{ 0 } + \frac{1}{1!}x^{ 1 } +\frac{1}{2!}x^{ 2 } +\frac{1}{3!}x^{ 3 } + \dots +\frac{1}{n!}x^{ n } + o(x^{ n }) \\
 \\
\boxed{e^{ x } = 1+x+\frac{x^{ 2 }}{2!} + \frac{x^{ 3 }}{3!} + \dots + \frac{x^{ n }}{n!}+o(x^{ n })} \\

e^{ 1 } = 1+1+ \frac{1}{2!} + \frac{1}{3!} + \dots \frac{1}{n!} + \dots  \\
e^{ 1 } = 2,718\dots 
\end{matrix}
}$$
---
### Таблица Тейлора при ${x \to 0}$
$$\displaylines{
\text{ Быстрая часть }\begin{cases}
e^x = 1 + x + \frac{x^2}{2!} + \frac{x^3}{3!} + \frac{x^4}{4!} + \dots + \frac{x^n}{n!} + o(x^n) \\ \\
\sin(x) = x - \frac{x^3}{3!} + \frac{x^5}{5!} - \dots + (-1)^n \frac{x^{2n+1}}{(2n+1)!} + o(x^{2n+1}) \\ \\
\cos(x) = 1 - \frac{x^2}{2!} + \frac{x^4}{4!} - \dots + (-1)^n \frac{x^{2n}}{(2n)!} + o(x^{2n}) \\
\end{cases} \\ \\ \text{ Медленная часть }
\begin{cases}
\ln(1+x) = x - \frac{x^2}{2} + \frac{x^3}{3} - \frac{x^4}{4} + \dots + (-1)^{n+1} \frac{x^n}{n} + o(x^n) \\ \\
\arctan(x) = x - \frac{x^3}{3} + \frac{x^5}{5} - \dots + (-1)^n \frac{x^{2n+1}}{2n+1} + o(x^{2n+1}) \\
\end{cases} \\ \\
\frac{1}{1-x} = 1 + x + x^2 + x^3 + \dots + x^n + o(x^n) \\
\frac{1}{1+x} = 1 - x + x^2 - x^3 + \dots + (-1)^n x^n + o(x^n) \\
(1+x)^a = 1 + ax + \frac{a(a-1)}{2}x^2 + \frac{a(a-1)(a-2)}{6}x^3 + \dots + \frac{a(a-1)\dots(a-n+1)}{n!}x^n + o(x^n) \\
\sinh(x) = x + \frac{x^3}{3!} + \frac{x^5}{5!} + \dots + \frac{x^{2n+1}}{(2n+1)!} + o(x^{2n+1}) \\
\cosh(x) = 1 + \frac{x^2}{2!} + \frac{x^4}{4!} + \dots + \frac{x^{2n}}{(2n)!} + o(x^{2n})
}$$
---
### Примеры.
$$\displaylines{
1) \ \lim_{ x \to 0 } {\frac{e^{ x }-1-x}{x^{ 2 }} } = \lim_{ x \to 0 } {\frac{1+x+\frac{x^{ 2 }}{2!}+o(x^{ 2 })-1-x}{x^{ 2 }} } = \lim_{ x \to 0 } \left( {\frac{1}{2!} + \cancel{\frac{o(x)}{x^{ 2 }}}^{ \ 0 } }\right) = \boxed{\frac{1}{2}} \\
e^{ x }\sim 1+x + \frac{x^{ 2 }}{2!} + o(x^{ 2 }) - \text{ разложение 1-й несокр. степени. }
}$$
$$\displaylines{
2) \ \lim_{ x \to 0 } {\frac{\sin{(x)}-x}{x^{ 3 }} } = \lim_{ x \to 0 } {\frac{x-\frac{x^{ 3 }}{6} + o(x^{ 3 }) - x}{x^{ 3 }} } = \lim_{ x \to 0 } {\frac{-\frac{x^{ 3 }}{6}}{x^{ 3 }} } = \boxed{-\frac{1}{6}}\\
\sin{(x)} = x - \frac{x^{ 3 }}{3!} + o(x^{ 3 })
}$$
$$\displaylines{
3) \ \lim_{ x \to 0 } {\frac{\cos{(x)} - 1 + \frac{x^{ 2 }}{2}}{x^{ 4 }} } = \lim_{ x \to 0 } {\frac{1-\frac{x^{ 2 }}{2} + \frac{x^{ 4 }}{24} + o(x^{ 4 }) -1 + \frac{x^{ 2 }}{2}}{x^{ 4 }} } = \lim_{ x \to 0 } {\frac{\frac{x^{ 4 }}{24}}{x^{ 4 }} } = \boxed{\frac{1}{24}}\\
\cos{(x)} = 1 - \frac{x^{ 2 }}{2!} + \frac{x^{ 4 }}{4!} + o(x^{ 4 })
}$$
$$\displaylines{
4) \ \lim_{ x \to 0 } {\frac{1 + x\cos{(x)} - \sqrt{ 1+2x }}{\ln(1+x)-x} } = \lim_{ x \to 0 } {\frac{1+x-\frac{x^{ 3 }}{2} + o(x^{ 3 }) - 1 - x + \frac{x^{ 2 }}{2}+o(x^{ 2 })}{-\frac{x^{ 2 }}{2}+o(x^{ 2 })} } = \\ \\= \lim_{ x \to 0 } {\frac{\frac{x^{ 2 }}{2}-\frac{x^{ 3 }}{2}+ o(x^{ 2 } )+o(x^{ 3 })}{-\frac{x^{ 2 }}{2} + o(x^{ 2 })} } = \lim_{ x \to \infty } {\frac{\frac{x^{ 2 }}{2}-\frac{x^{ 3}}{2}^{ =o(x^{ 2 }) } + o(x^{ 2 })}{-\frac{x^{ 2 }}{2}+o(x^{ 2 })} }  = \lim_{ x \to 0 } {\frac{\frac{x^{ 2 }}{2} + o(x^{ 2 })}{-\frac{x^{ 2 }}{2}+o(x^{ 2 })} } = \boxed{-1}\\ \\
\ln(1+x) = x - \frac{x^{ 2 }}{2} + o(x^{ 2 }) \\
\ln(1+x) - x = -\frac{x^{ 2 }}{2} + o(x^{ 2 }) \\
\cos{(x)} = 1-\frac{x^{ 2 }}{2} + o(x^{ 2 }) , \  x\cos{(x)} = x-\frac{x^{ 3 }}{2} + o(x^{ 3 })\\
\sqrt{ 1+2x } = (1+2x)^{ 1/2 } = 1+ \frac{1}{2}2x+\frac{\frac{1}{2}\left( \frac{1}{2}-1 \right)}{2!}(2x)^{ 2 } + o(x^{ 2 }) = 1+x-\frac{x^{ 2 }}{2} + o(x^{ 2 })
}$$
$$\displaylines{
5) \ \boxed{\lim_{ x \to 0 } {\frac{e^{ x }-\sqrt[3]{ 1+3x+\frac{9x^{ 2 }}{2} }}{x^{ 3 }} }}\\ 
e^{ x } = 1+ x + \frac{x^{ 2 }}{2!} + \frac{x^{ 3 }}{3!} + o(x^{ 3 }) \\
\sqrt[3]{ 1+3x + \frac{9x^{ 2 }}{2} } = \left( 1+ \left( 3x+\frac{9x^{ 2 }}{2} \right) \right)^{ 1/3 } = \\ = 1+ \frac{1}{3}\left( 3x+\frac{9x^{ 2 }}{2} \right) + \frac{\frac{1}{3}\left( \frac{1}{3}-1 \right)}{2}\left( 3x+\frac{9x^{ 2 }}{2} \right)^{ 2 } + \frac{\frac{1}{3}\left( \frac{1}{3-1} \right)\left( \frac{1}{3}-2 \right)}{3!} \left( 3x + \frac{9x^{ 2 }}{2} \right)^{ 3 } + o(x^{ 3 })  \ \boxed{=}  \\
\left( 3x + \frac{9x^{ 2 }}{2} \right)^{ 2 } = \left( 3x+\frac{9x^{ 2 }}{2} \right) \cdot \left( 3x+\frac{9x^{ 2 }}{2} \right) = 9x^{ 2 } + \frac{27x^{ 3 }}{2} + \frac{27x^{ 3 }}{2} + \underset{ \hookrightarrow o(x^{ 3 })}{ \frac{81x^{ 4 }}{4} } + o(x^{ 3 })  = 9x^{ 2 } + 27x^{ 3 } + o(x^{ 3 }) \\
\left( 3x + \frac{9x^{ 2 }}{2} \right)^{ 3 } = \left( 3x+\frac{9x^{ 2 }}{2} \right) \cdot \left( 3x+\frac{9x^{ 2 }}{2} \right) \cdot \left( 3x+\frac{9x^{ 2 }}{2} \right) = \dots = 27x^{ 3 } + o(x^{ 3 }) \\
\boxed{=} \ 1+ x + \frac{3x^{ 2 }}{2} - x^{ 2 } - 3x^{ 3 } + \frac{5}{3}x^{ 3 } + o(x^{ 3 }) = 1+x + \frac{x^{ 2 }}{2} -\frac{4x^{ 3 }}{3} + o(x^{ 3 })
}$$
$$\displaylines{
\boxed{\lim_{ x \to 0 } {\frac{e^{ x }-\sqrt[3]{ 1+3x+\frac{9x^{ 2 }}{2} }}{x^{ 3 }} }} = \lim_{ x \to 0 } {\frac{1+ x + \frac{x^{ 2 }}{2!} + \frac{x^{ 3 }}{3!} + o(x^{ 3 }) - \left( 1+x + \frac{x^{ 2 }}{2} -\frac{4x^{ 3 }}{3} + o(x^{ 3 }) \right)}{x^{ 3 }} } = \\
= \lim_{ x \to 0 } {\frac{\frac{x^{ 3 }}{6}+ \frac{8x^{ 3 }}{6} + o(x^{ 3 })}{x^{ 3 }} } = \boxed{\frac{3}{2}}
}$$
---


