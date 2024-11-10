**Уткин Никита МА1, 2 вариант**

### I. Вычислить
$$\displaylines{
\lim_{ x \to -\infty } {\frac{x+\sqrt{ x^{ 2 } + x }}{2x+ \sqrt{ 4x^{ 2 } +1 }}} = \lim_{ x \to -\infty } {\frac{x\left( 1+\sqrt{ 1+\frac{1}{x} } \right)}{x\left( 2+\sqrt{ 4+\frac{1}{x^{ 2 }} } \right)}} = \lim_{ x \to -\infty } {\frac{2x}{4x}} = \boxed{\frac{1}{2}}\\
\lim_{ x \to \infty } {\frac{4^{ x }+3x}{2^{ 2x }-x}} = \lim_{ x \to \infty } {\frac{4^{ x }}{2^{ 2x }}} = \lim_{ x \to \infty } {\frac{2^{ 2x }}{2^{ 2x } }} = \boxed{1}
}$$
### II. Доказать
$$\displaylines{
\cancel\exists \lim_{ x \to 0  } {\tan{\left( \frac{2}{x} \right)}}  \\
\text{ если } x\to0^{ + }, \  \text{ то } \frac{2}{x} \to +\infty \\
\text{ если } x \to 0^{ - }, \  \text{ то } \frac{2}{x} \to -\infty\\
\text{ Из-за бесконечных колебаний между }\pm \infty \ \text{функция не стремится к одному значению } \\
\implies \cancel\exists \lim_{ x \to 0 } {\tan{\left( \frac{2}{x} \right)}} \\
\\
\lim_{ x \to 1 } {\frac{x-1}{x^{ 2 }-1}} = \frac{1}{2} \\
\lim_{ x \to 1 } {\frac{x-1}{(x-1)(x+1)}} = \lim_{ x \to 1 } {\frac{1}{x+1}} = \frac{1}{1+1} = \boxed{\frac{1}{2}}
}$$
### III. Вычислить
$$\displaylines{
\lim_{ x \to -1 } {\frac{x^{ 3 }+2x^{ 2 }+3x+2}{x^{ 3 }+1}} = \lim_{ x \to -1 } {\frac{(x +1)(x^{ 2 }+x+2)}{(x+1)(x^{ 2 }-x+1)}} = \lim_{ x \to -1 } { \frac{x^{ 2 }+x+2}{x^{ 2 }-x+1}} = \frac{1-1+2}{1+1+1} = \boxed{\frac{2}{3}}\\
\lim_{ x \to -3 } {\frac{\sqrt{ 7+x }-2}{x+3}} = \lim_{ x \to -3 } {\frac{(\sqrt{ 7+x }-2)(\sqrt{ 7+x }+2)}{(x+3)(\sqrt{ 7+x }+2)}} = \lim_{ x \to -3 } {\frac{(7+x)-4}{(x+3)(\sqrt{ 7+x }+2)}} = \lim_{ x \to -3 } {\frac{1}{\sqrt{ 7 +x }+2}} = \frac{1}{\sqrt{ 4 }+2} = \boxed{\frac{1}{4}}


}$$

### IV. Вычислить
$$\displaylines{
\lim_{ x \to 0 } {\frac{\cos{(x)}\cdot \ln(1+3x^{ 2 })\ln(1+\cos{(x)})}{(e^{ 3x }-1)(\cos{(4x-5x^{ 2 })-1})}} = \lim_{ x \to 0 } {\frac{\left( 1-\frac{x^{ 2 }}{2} \right)\cdot3x^{ 2 }\cdot \ln\left( 2-\frac{x^{ 2 }}{2} \right)}{3x \cdot \left( -\frac{(4x - 5x^{ 2 })^{ 2 }}{2} \right)}} = \lim_{ x \to 0 } {\frac{3x^{ 2 }\cdot \ln(2)}{3x \cdot (-8x^{ 2 })}} = \lim_{ x \to 0 } {\frac{3x^{ 2 }\ln(2)}{-24x^{ 3 }}} = \lim_{ x \to 0 } {-\frac{\ln(2)}{8x}} = \boxed{-\infty} \\
(4x-5x^{ 2 })^{ 2 } = (16x^{ 2 }-40x^{ 3 }+25x^{ 4 }) \approx 16x^{ 2 }, \  \text{ при } x \to 0
}$$

$$\displaylines{
\lim_{ x \to 0 } {\frac{\cos{(3x)}-\cos{(x)}}{\cos{\left( \frac{\pi}{2} -x^{ 2 } \right) - \arcsin{(2x^{ 3 })}}}} = \lim_{ x \to 0 } {\frac{-2\sin{\left( \frac{3x+x}{2} \right)\sin{\left( \frac{3x-x}{2} \right)}}}{x^{ 2 } - 2x^{ 3 }}} = \lim_{ x \to 0 } {\frac{-2\sin{(2x)}\sin{(x)}}{x^{ 2 }-2x^{ 3 }}} = \lim_{ x \to 0 } {\frac{-2\cdot 2x \cdot x}{x^{ 2 }(1-2x)}} = \lim_{ x \to 0 } {\frac{-4x^{ 2 }}{x^{ 2 }(1-2x)}} = \\
= \lim_{ x \to 0 } {-\frac{4}{1-2x}} = -\frac{4}{1-2\cdot0} = \boxed{-4}
}$$

$$\displaylines{
\lim_{ x \to 1 } {(x)^{ \frac{1}{\sin{(x-1)}^{ 2 }} }} = \lim_{ x \to 1 } {\frac{\ln(x)}{\sin{(x-1)}^{ 2 }}} = \begin{bmatrix}
t = x-1, \  t \underset{ x\to1 }{ \to 0 }
\end{bmatrix} = \lim_{ t \to 0 } {\frac{\ln(1+t)}{\sin{(t)}^{ 2 }}} = \lim_{ t \to 0 } {\frac{t}{t^{ 2 }}} = \lim_{ t \to 0 } {\frac{1}{t}} = \boxed{\infty}
}$$
