### 1 вариант.
$$\displaylines{
\int_{\frac{\pi}{4}}^{\arctan{(3)}} \frac{1}{(3\tan{(x)} + 5) \sin{(2x)}}  \, dx  = \int_{\frac{\pi}{4}}^{\arctan{3}} \frac{1+\tan{(x)}^{ 2 }}{2\tan{(x)}(3\tan{(x)} + 5)}  \, dx \begin{vmatrix}
t = \tan{(x)} \\
dt = (1+\tan{(x)}^{ 2 })dx \\
dx = \dfrac{dt}{1+t^{ 2 }}
\end{vmatrix} = \int_{1}^{3} \frac{1}{2t(3t + 5)}  \, dt \\
\frac{1}{t(3t+5)} = \frac{A}{t} + \frac{B}{3t + 5}  \\
A(3t + 5) + Bt = 1 \\
(3A + B)t + 5A = 1 \\
A = \frac{1}{5}, \   B = -\frac{3}{5} \\
\frac{1}{2}\left( \frac{1}{5} \int_{1}^{3} \frac{1}{t} \, dt   - \frac{3}{5} \int_{1}^{3} \frac{1}{3t+5} \, dx \right) = \frac{1}{2}\left( \frac{1}{5}\ln(3) - \frac{3}{5} \cdot \frac{1}{3} (\ln(14) - \ln( 8)) \right) = \frac{1}{10}(\ln(3) + \ln(8) - \ln(14)) = \frac{1}{10}\ln\left( \frac{12}{7} \right)
}$$
$$\displaylines{
I = \int_{0}^{1} \frac{4\sqrt{ 1-x } - \sqrt{ 3x + 1 }}{(\sqrt{ 3x+1 } + 4\sqrt{ 1-x })} \cdot \frac{1}{(3x+1)^{ 2 }}   \, dx \\
t = \frac{\sqrt{ 3x+1 }}{4\sqrt{ 1-x }} \\
t^{ 2 } = \frac{3x+1}{16(1-x)} \implies  16t^{ 2 }(1-x) = 3x+1 \implies x(-16t^{ 2 } - 3) = 1-16t^{ 2 } \implies  x = \frac{16t^{ 2 }-1}{16t^{ 2 } + 3} \\
dx = \frac{128t}{(16t^{ 2 } + 3)^{ 2 }}dt \\
x = 0 \hookrightarrow t = \frac{1}{4}, \  x = 1 \hookrightarrow t \to  \infty \\
I = \int_{1/4}^{\infty} \frac{1-t}{t(1+t)} \cdot  \frac{(16t^{ 2 } + 3)^{ 2 }}{(64t^{ 2 })^{ 2 }} \cdot  \frac{128t}{(16t^{ 2 } + 3)^{ 2 }}  \, dt =  \frac{1}{32} \int_{1/4}^{\infty} \frac{1-t}{t^{ 3 }(1+t)}  \, dt = \frac{1}{32} \int_{1/4}^{\infty} \left( \frac{2}{t} - \frac{2}{t^{ 2 } } + \frac{1}{t^{ 3 }} - \frac{2}{1+t} \right)  \, dt \\
= \frac{1}{32}\left[ 2\ln(t) + \frac{2}{t} - \frac{1}{2t^{ 2 }} - 2\ln(1+t) \right]_{ 1/4 }^{ \infty } = \frac{1}{32}(0 + 2\ln(5)) = \frac{\ln(5)}{16}
}$$
$$\displaylines{
D = \{ y = (x-2)^{ 3 } \ \quad y = 4x-8 \}. \ \quad S(D) -? \\
(x-2)^{ 3 } = 4x-8 \\
x^{ 3 } - 6x^{ 2 } + 12x-8 = 4x-8 \implies  x^{ 3 } -6x^{ 2 } + 8x = 0 \\
x = 0; x^{ 2 }-6x + 8 = 0 \\
x = 0, \  x = 2, \   x = 4 - \text{ точки пересечения. } \\
\text{ На [0, 2] при } x = 1 \ \quad (1-2)^{ 3 } = -1, \  4 - 8 = -4 \implies  (x-2)^{ 3 } > 4x-8 \\
\text{ На [2, 4] при } x = 3 \ \quad (3-2)^{ 3 } = 1, \   4 \cdot 3 - 8 = 4 \implies 4x-8 > (x-2)^{ 3 } \\
S(D) = \int_{0}^{2} [(x-2)^{ 3 } - (4x-8)]  \, dx  + \int_{2}^{4} [(4x-8) - (x-2)^{ 3 }] \, dx  \\
\text{ i}. \ \int_{0}^{2} x^{ 3 } - 6x^{ 2 } + 12x - 8 - 4x + 8  \, dx = \int_{0}^{2} x^{ 3 } - 6x^{ 2 } + 8x \, dx  \\ 
= \left[ \frac{x^{ 4 }}{4} - 2x^{ 3 } + 4x^{ 2 } \right]_{ 0 }^{ 2 } = (4-16 + 16) - 0 = 4 \\
\text{ ii}. \ \int_{2}^{4} 4x-8-x^{ 3 }+6x^{ 2 } - 12x + 8 \, dx = \int_{2}^{4} -x^{ 3 } + 6x^{ 2 } - 8x \, dx   \\ =\left[ -\frac{x^{ 4 }}{4} + 2x^{ 3 } - 4x^{ 2 } \right]_{ 2 }^{ 4 } = (-64+128 - 64) - (-4 + 16 - 16) = 4 \\
S(D) = 4 + 4 = 8.
}$$
$$\displaylines{
\Gamma: \begin{cases}
x = 4\sqrt{ 2 } \cos{(t)}^{ 3 }  \\
y = 2\sqrt{ 2 } \sin{(t)}^{ 3 }
\end{cases} \ \quad x = 2 \ \  (x\geq 2). \ S(D) - ? \\
\text{ Подставим } x = 2: 2 = 4\sqrt{ 2 } \cos{(t)}^{ 3 } \implies  \cos{(t)}^{ 3 } = \frac{1}{2\sqrt{ 2 }} \implies  \cos{(t)} = \frac{1}{\sqrt{ 2 }} \\
t=  \frac{\pi}{4}, \  t = \frac{7\pi}{4}. \text{Рассматриваем часть между } \frac{\pi}{4} \text{ и } \frac{\pi}{2}, \  \text{так как} x\geq 2. \\
S(D) = \int_{t_{ 1 }}^{t_{ 2 }} y \cdot  \frac{dx}{dt} \, dt = \int_{\frac{\pi}{4}}^{\pi/2} 2\sqrt{ 2 }\sin{(t)}^{ 3 } (-12\sqrt{ 2 }\cos{(t)}^{ 2 } \sin{(t)}) \, dt \\
 = \left|   -48 \int_{}^{} \sin{(t)}^{ 4 }\cos{(t)}^{ 2 } \, dt \right| = 48 \int_{}^{} \left( \frac{1-2\cos{(2t)} + \cos{(2t)}^{ 2 }}{4}  \right) \left(  \frac{1+ \cos{(2t)}}{2}  \right) \, dt \\
 = 48 \int_{}^{} \frac{(1-\cos{(2t)} - \cos{(2t)^{ 2 }} + \cos{(2t)}^{ 3 })}{8}  \, dt =  48 \int_{}^{} \frac{1 - \cos{(2t)} - \cos{(4t)} + \cos{(2t)} \cos{(4t)}}{16}  \, dx  \\ 
 = 48 \int_{}^{} \frac{2-\cos{(2t)}-2\cos{(4t)} + \cos{(6t)}}{32}  \, dx  = 48 \int_{}^{} \left( \frac{1}{16} - \frac{\cos{(2t)}}{32} - \frac{\cos{(4t)}}{16} + \frac{\cos{(6t)}}{32} \right) \, dx \\
 = 48 \left[\frac{t}{16} - \frac{\sin{(2t)}}{64} - \frac{\sin{(4t)}}{64} + \frac{\sin{(6t)}}{192}\right] + C \\
 = 48 \left[  \left(\frac{\pi/2}{16} - \frac{\sin{(\pi)}}{64} - \frac{\sin{(2\pi)}}{64} + \frac{\sin{(3\pi)}}{192} \right) - \left( \frac{\pi/4}{16} - \frac{\sin{(\pi/2)}}{64} - \frac{\sin{(\pi)}}{64} + \frac{\sin{(3\pi/2)}}{192} \right)\right] 
 = 48\left[ \frac{\pi}{32} - \left( \frac{\pi}{64} - \frac{1}{64} - \frac{1}{192} \right) \right] = 48\left[ \frac{\pi}{64} + \frac{1}{64} + \frac{1}{192} \right] 
}$$