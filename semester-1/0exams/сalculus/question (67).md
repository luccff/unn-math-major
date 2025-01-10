### Построение графика функции с полным исследованием.
---
План анализа:
1) Найти область определения ${D(x)}$ (все ${x}$, при которых существует ${f(x)}$) и указать особые точки;
2) Найти ${y}$ при ${x = 0}$ (пересечение ординат). Найти ${x}$ при которых ${y = 0}$ ( корни или пересечение с абсциссой);
3) Проверить знаки ${f(x)}$ методом интервалов;
4) Найти вертикальные асимптоты и исследовать поведение функции в их окрестности (т.е. стремление к ${+}\infty$ или ${- \infty}$);
5) Найти наклонную асимптоту ${y= kx+b}$, где ${\displaystyle k = \lim_{ x \to \pm \infty } {\frac{f(x)}{x}}}$, ${\displaystyle  b = \lim_{ x \to \pm \infty } {(f(x)-kx)}}$;
6) Найти ${y'}$, исследовать на монотонность и найти экстремумы функции;
7) Найти ${y''}$, исследовать на выпуклость и найти точки перегиба функции;
8) Построить график функции. 

Пример 1.
$$\displaylines{
f(x) = \frac{x^{ 2 }+8}{1-x} \\

}$$

1) ${D(x) = \mathbb{R}\backslash\{ 1 \} }$
2) ${x = 0; f(0) = 8 }$
$$\displaylines{
y = 0; \frac{x^{ 2 }+8}{1-x} = 0 \to  x \cancel{\in } \mathbb{R} \\
}$$
3) 
```tikz
\begin{document}
\begin{tikzpicture}[scale=2, baseline=(current bounding box.center)]
  \draw[->] (-3,0) -- (3,0) node[below] {};
  \draw[fill=white, thick] (0, 0) circle (1pt) node[below] {\(1\)};
  \node at (-1, 0.3) { $+$ };
  \node at (1, 0.3) { $-$ };
\end{tikzpicture}
\end{document}
```

4) Вертикальная асимптота: ${ x = 1}$
$$\displaylines{
\lim_{ x \to 1^{ + } } {\frac{x^{ 2 }+8}{1-x} } = \left[ \frac{9}{0^{ - }} \right] = -\infty \\
\lim_{ x \to 1^{ - } } {\frac{x^{ 2 }+8}{1-x} } = \left[ \frac{9}{0^{ + }} \right] = + \infty \\
}$$
5) Наклонные асимптоты: ${y = kx+b}$ 
$$\displaylines{
k = \lim_{ x \to \pm \infty } {\frac{\cfrac{x^{ 2 }+8}{1-x} }{x} } = \lim_{ x \to \pm \infty } {\frac{x^{ 2 }+8}{x-x^{ 2 }} } = -1 \\
b = \lim_{ x \to \pm \infty } {\left( \frac{x^{ 2 }+8}{1-x} +x \right)} = \lim_{ x \to \pm \infty } {\frac{x^{ 2 }+8+x-x^{ 2 }}{1-x} } = -1 \\
}$$
Итого: ${y= -x-1}$ на ${\pm \infty}$ (непонятно с какой стороны прижимаемся к асимптоте, поэтому рассм. другой способ)
Другой способ:
$$\displaylines{
\frac{x^{ 2 }+8}{1-x} = -\left( \frac{x^{ 2 }+8}{x-1}  \right) = \\
\text{ поделим уголком } \\
= -\left( x+1 + \frac{9}{x-1}  \right) = -x-1 - \frac{9}{x-1} \sim -x-1 \\
\text{ Рассмотрим  } -\frac{9}{x-1}: \lim_{ x \to +\infty } {-\frac{9}{x-1} } = 0^{ - } - \text{ ниже асимптоты } \\
\lim_{ x \to -\infty } {-\frac{9}{x-1} } = 0^{ + } - \text{ выше асимптоты }
}$$
6) ${y' = \left( \cfrac{x^{ 2 }+8}{1-x} \right)'}$
$$\displaylines{ 
= \frac{2x(1-x) + (x^{ 2 }+8)}{(1-x)^{ 2 }} = \frac{2x-2x^{ 2 }+x^{ 2 }+8}{(x-1)^{ 2 }} = \frac{-x^{ 2 }+2x+8}{(x-1)^{ 2 }} = \\
= - \frac{x^{ 2 }-2x-8}{(x-1)^{ 2 }} = - \frac{(x-4)(x+2)}{(x-1)^{ 2 }} = 0 \\  
}$$
```tikz
\begin{document}
\begin{tikzpicture}[scale=2, baseline=(current bounding box.center)]

  \draw[->] (-4,0) -- (4,0) node[below] {};

  

  \draw[fill=black, thick] (-2, 0) circle (1pt) node[below] {\(-2\)};

  \draw[fill=white, thick] (0, 0) circle (1pt) node[below] {\(1\)};

  \draw[fill=black, thick] (2, 0) circle (1pt) node[below] {\(4\)};

  

  \node at (-4, 0.3) { $y'$ };

  \node at (-4, -0.3) { $y$ };

  \node at (-3, 0.3) { $-$ };

  \node at (-3, -0.3) { $\searrow$ };

  \node at (-1, 0.3) { $+$ };

  \node at (-1, -0.3) { $\nearrow$ };

  \node at (1, 0.3) { $+$ };

  \node at (1, -0.3) { $\nearrow$ };

  \node at (3, 0.3) { $-$ };

  \node at (3, -0.3) { $\searrow$ };

\end{tikzpicture}
\end{document}
```

$$\displaylines{
x = -2 - \text{ точка минимума } \quad f_{ \min } = f(-2) = 4 \quad (-2; 4) - \text{ т. min }\\
x = 4 - \text{ точка максимума } \quad f_{ \max } = f(4) = -8 \quad (4; -8) - \text{ т. max }
}$$
7) ${y'' = \left( -\cfrac{x^{ 2 }-2x-8}{(x-1)^{ 2 }} \right)'}$
$$\displaylines{
= - \frac{(2x-2)(x-1)^{ 2 }- (x^{ 2 }-2x-1) \cdot 2(x-1)}{(x-1)^{ 3 }} = -\frac{18}{(x-1)^{ 3 }}  
}$$
```tikz
\begin{document}
\begin{tikzpicture}[scale=2, baseline=(current bounding box.center)]

  \draw[->] (-3,0) -- (3,0) node[below] {};

  

  \draw[fill=white, thick] (0, 0) circle (1pt) node[below] {\(1\)};

  

  \node at (-3, 0.3) { $y''$ };

  \node at (-3, -0.3) { $y$ };

  \node at (-1, 0.3) { $+$ };

  \node at (-1, -0.3) { $\bigcup$ };

  \node at (1, 0.3) { $-$ };

  \node at (1, -0.3) { $\bigcap$ };

  

\end{tikzpicture}
\end{document}
```


![[Pasted image 20250109053725.png|600]]
