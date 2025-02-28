Уткин Никита 3824Б1МА1.
I.
$$\displaylines{
1) \ \int \frac{dx}{(2x+3)^{ 2 } - 36} = \begin{vmatrix}
t = 2x+3 \\
dt = 2dx \\
dx = \frac{dt}{2}
\end{vmatrix} = \frac{1}{2}\int \frac{dx}{t^{ 2 }-6^{ 2 }} = \frac{1}{24}\ln\left| \frac{2x-3}{2x+9} \right| + C
}$$
$$\displaylines{
2)\int \frac{(\sqrt{ x }+2)^{ 3 }}{x}dx = \int \frac{x\sqrt{ x }+6x+12\sqrt{ x }+8}{x}dx = \int \left( \frac{x^{ 3/2 }}{x}+\frac{6x}{x}+\frac{12x^{ 1/2 }}{x} + \frac{8}{x} \right)dx = \\ =\int x^{ 1/2 }dx + \int 6dx + \int  12x^{ -1/2 }dx + \int \frac{8}{x}dx = \frac{x^{ 3/2 }}{\frac{3}{2} }+ 6x + \frac{12x^{ 1/2 }}{\frac{1}{2}} + 8\ln|x| + C   
}$$
$$\displaylines{
3)\int (2\sin{(5x)^{ 2 }} + 3)dx = \int 2 \cdot \frac{1-\cos{(10x)}}{2} + 3 dx = \int 4-\cos{(10x)} = 4x -\frac{\sin{(10x)}}{10} + C
}$$

II.
$$\displaylines{
1)\int \frac{x^{ 2 }}{\sqrt[4]{ 2x^{ 3 }+1 }}dx = \begin{vmatrix}
u = 2x^{ 3 }+1 \\
du = 6x^{ 2 }dx \\
\dfrac{du}{6} = x^{ 2 }
\end{vmatrix} = \frac{1}{6}\int u ^{ -1/4 }du = \frac{1}{6} \frac{u^{ 3/4 }}{\frac{3}{4}} + C = \frac{2}{9}(2x^{ 3 }+1)^{ 3/4 } + C
}$$
$$\displaylines{
2)\int \frac{4x+5}{x^{ 2 }+4x+8} dx = \int \frac{4x+5}{(x+2)^{ 2 } + 4} dx = \begin{vmatrix}
u = x+2  \\
du = dx \\
x = u-2 
\end{vmatrix} = \int \frac{4(u-2)+5}{u^{ 2 } + 4}du = \int \frac{4u-3}{u^{ 2 }+3}du = \\
= \int \frac{4u}{u ^{ 2 } + 3}du - \int \frac{3}{u ^{ 2 } + 4}du = \begin{vmatrix}
w = u ^{ 2 } + 4 \\
dw = 2udu \\
du = \frac{dw}{2u} \\
4udu = 2dw
\end{vmatrix} = \int \frac{2dw}{w} - \frac{3}{2}\arctan{\left( \frac{u}{2} \right)} + C \\
=2\ln(u ^{  2 } + 4) - \frac{3}{2}\arctan{\left( \frac{u}{2} \right)} + C = 2\ln((x+2)^{ 2 }+4) - \frac{3}{2}\arctan{\left( \frac{x+2}{2} \right)} + C
}$$
$$\displaylines{
3)\int \frac{\sin{(\sqrt[3]{ x })}}{\sqrt[3]{ x }}dx = \int \frac{\sin{(t)}}{t} 3t^{ 2 }dt = 3\int t\sin{(t)}dx = -3(t\cos{(t)} + \sin{(t)}) + C = -3\sqrt[3]{ x }\cos{(\sqrt[3]{ x })} + 3\sin{(\sqrt[3]{ x })} + C\\-e^{ x }\cos{(x)} +e^{ x }\sin{(x)}
\begin{array}{|c|c|}
\hline 
D & I \\
\hline 
t & \sin{(t)} \\
\hline 
1 & -\cos{(t)} \\
\hline 
0 & -\sin{(t)} \\
\hline 
\end{array}
}$$
III.
$$\displaylines{
1) \int \frac{dx}{2+\sqrt{ x+3 }} = \begin{vmatrix}
t = \sqrt{ x+3 }
\end{vmatrix}  = \int \frac{2tdt}{2+t} = 2\int \left( 1- \frac{2}{t+2} \right)dt = 2\sqrt{ x+3 } -4\ln|2+\sqrt{ x+3 }| + C 
}$$
$$\displaylines{
2)\int \frac{dx}{\sqrt{ e^{ x }+10 }} = \begin{vmatrix}
t = \sqrt{ e^{ x }+10 }
\end{vmatrix} = \frac{1}{\sqrt{ 10 }}\ln\left| \frac{t-\sqrt{ 10 }}{t+\sqrt{ 10 }}  \right| + C = \frac{1}{\sqrt{ 10 }}\int \ln\left| \frac{\sqrt{ e^{ x }+10 } - \sqrt{ 10 }}{\sqrt{ e^{ x }-10 } + \sqrt{ 10 }}  \right| + C  
}$$
$$\displaylines{
3)\int \frac{dx}{x\sqrt{ 4-x^{ 2 } }} = \dots 
}$$
IV.
$$\displaylines{
1) \int = (x^{ 2 }+2x)\sin{(4x)}dx = -\frac{1}{4}(x^{ 2 }+2x)\cos{(4x)} + \frac{1}{16}(2x+2)\sin{(4x)} + \frac{\cos{(4x)}}{32} \\
\begin{array}{|c|c|c|}
\hline 
D & I \\
\hline 
x^{ 2 }+2x & \sin{(4x)} \\
\hline 
2x+2 & -\cfrac{\cos{(4x)}}{4} \\
\hline 
2 & -\cfrac{\sin{(4x)}}{16} \\
\hline 
0 & \cfrac{\cos{(4x)}}{64} \\
\hline 
\end{array}
}$$
$$\displaylines{
2)\int x^{ 3 }\ln(x)dx =  \frac{1}{4}\ln(x)x^{ 4 } - \int \frac{1}{x} \frac{1}{4}x^{ 4 }dx = \frac{1}{4}\ln(x)x^{ 4 } -\frac{1}{16}x^{ 4 } + C\\
\begin{array}{|c|c|}
\hline 
D & I \\
\hline 
\ln(x) & x^{ 3 } \\
\hline 
\dfrac{1}{x} & \cfrac{1}{4}x^{ 4 } \\
\hline 
\end{array} 
}$$
$$\displaylines{
3)\int e^{ x }\sin{(x)}dx = -e^{ x }\cos{(x)} +e^{ x }\sin{(x)} - \int e^{ x }\sin{(x)}dx = \frac{-e^{ x }\cos{(x)} +e^{ x }\sin{(x)}}{2} + C \\
\begin{array}{|c|c|}
\hline 
D & I \\
\hline 
e^{ x } & \sin{(x)} \\ \hline 
e^{ x }  & -\cos{(x)} \\
\hline 
e^{ x } & -\sin{(x)} \\
\hline 

\end{array}
}$$