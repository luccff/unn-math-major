Ex. 1 Найти ${f'(x_{ 0 })}$, если:
$$\displaylines{
1) \ f = x^{ 2 }, \  x_{ 0 } = 0,1 \\
f'(x)\frac{d}{dx}(x^{ 2 }) = 2x \\
f'(0,1) = 2 \times 0,1 = \boxed{0,2} 
}$$
$$\displaylines{
2) \ f = 2\sin{(3x)}, \ x_{ 0 } = \frac{\pi}{6} \\
f'(x) = 2\cdot \frac{d}{dx}\sin{(3x)} = 6\cos{(3x)} \\
f'(x_{ 0 }) = 6\cdot \cos{\left( 3 \cdot \frac{\pi}{6} \right)} = 6 \cdot  0 = \boxed{0}
}$$
$$\displaylines{
3) \ f = 1+ \ln(2x), \  x_{ 0 } = 1 \\
f'(x) = \frac{d}{dx} 1+\ln(2x) = \frac{1}{2x} \cdot 2 = \frac{1}{x} \\
f'(x_{ 0 }) = \frac{1}{1} = \boxed{1}
}$$
Ex. 213(3,5,7,9) Найти дифференциал:
$$\displaylines{
3) \ d(2\sqrt{ x^{ 3 } }(3\ln(x)-2)) = d(2x^{ 3/2 }(3\ln(x)-2)) = \left( 3x^{ 1/2 }\cdot (3\ln(x)-2) + 2x^{ 3/2 }\cdot \frac{3}{x} \right)dx = \\
= \left( \frac{6x^{ 3/2 }}{x}  \right)dx + (3x^{ 1/2 }(3\ln(x) -2))dx= 6x^{ 1/2 }dx+ 3x^{ 1/2 }(3\ln(x)-2)dx = \\
= x^{ 1/2 }(6+3(3\ln(x)-2))dx = \boxed{9\sqrt{ x } \ \ln(x)dx}
}$$
$$\displaylines{
5) \ d\ln\left(\sqrt{ 1+2\sin{(x)} }+ \sqrt{ 2\sin{(x)}-1 }\right) = \left( \frac{1}{\sqrt{ 1+2\sin{(x)} }+ \sqrt{ 2\sin{(x)}-1}} \right)\cdot \left( \frac{\cos{(x)}}{\sqrt{ 1+2\sin{(x)} }} + \frac{\cos{(x)}}{\sqrt{ 2\sin{(x)-1}}}  \right)dx =  \\
= \frac{1}{\sqrt{ 1+2\sin{(x)} }+ \sqrt{ 2\sin{(x)}-1}} \cdot  \left(\frac{\cos{(x)}}{\sqrt{ 1+2\sin{(x)}  }} + \frac{\cos{(x)}}{\sqrt{ 2\sin{(x)}-1 }}\right) dx =\\
= \frac{1}{\sqrt{ 1+2\sin{(x)} } + \sqrt{ 2\sin{(x)}-1 }} \cdot \frac{\cos{(x)}(\sqrt{ 2\sin{(x)}-1 }+\sqrt{ 1+2\sin{(x)} })}{\sqrt{ (1+2\sin{(x)})\cdot (2\sin{(x)}-1) }}dx = \\ = \frac{\cos{(x)}}{\sqrt{ (1+2\sin{(x)}) \cdot  (2\sin{(x)}-1) }}dx = \boxed{\frac{\cos{(x)}}{\sqrt{ 4\sin{(x)}^{ 2 } -1}}dx}

}$$
$$\displaylines{
7) \ d\left( \frac{\arcsin{(x)}}{\sqrt{ 1-x^{ 2 } }} + \ln\left( \sqrt{ \frac{1-x}{1+x}  } \right)  \right) = \frac{ 1+  \frac{x\arcsin{(x)}}{\sqrt{ 1-x^{ 2 } }}}{1-x^{ 2 }}  - \frac{1}{2} \cdot \frac{1+x}{1-x} \cdot \frac{-2}{(1+x)^{ 2 }} = \frac{\sqrt{ 1-x^{ 2 } } + x\arcsin{(x)}}{\sqrt{ 1-x^{ 2 }(1-x^{ 2 }) }} -\frac{1}{1-x^{ 2 }} = \\
= \boxed{\frac{x\arcsin{(x)}}{\sqrt{ 1-x^{ 2 }(1-x^{ 2 }) }}} 
}$$
$$\displaylines{
9) \ d(x^{ x^{ 2 } }) \\
\ln(y) = \ln(x^{ x^{ 2 } })\\
\frac{1}{y} \cdot \frac{dy}{dx} = \frac{d}{dx} x^{ 2 }\ln(x) \\
\boxed{\frac{dy}{dx} = x^{ x^{ 2 } } \cdot  (2x\ln(x)+x)}


}$$
Ex. 214(2,4) Найти дифференциал в указанных точках:
$$\displaylines{
2) \ d\left( \arctan{\left( \frac{\ln(x)}{x} \right)} \right), \  x_{ 1 } = \frac{1}{e}, \  x_{ 2 } = e \\
\frac{dy}{dx} = \frac{1}{1+ \left( \frac{\ln(x)}{x} \right)^{ 2 }} \cdot  \frac{1-\ln(x)}{x^{ 2 }} \\
\text{ Для } x_{ 1 } = \frac{1}{e} \quad dy = \frac{1}{1+e^{ 2 }} \cdot  \frac{1-(-1)}{\left( \frac{1}{e} \right)^{ 2 }}dx = \frac{1}{1+e^{ 2 }} \cdot  2e^{ 2 }dx = \boxed{\frac{2e^{ 2 }}{1+e^{ 2 }}dx} \\
\text{ Для }x_{ 2 } = e \quad dy = \frac{1}{1+ \left( \frac{1}{e} \right)^{ 2 }} \cdot  \frac{1-1}{e^{ 2 }}dx = \frac{1}{1+\frac{1}{e^{ 2 }}} \cdot  0dx = \boxed{0}\\

}$$
$$\displaylines{
4) \ d\left( \frac{x^{ 2 }2^{ x }}{x^{ x }}  \right), \  x_{ 1 } = 1, \ x_{ 2 } = 2 \\
\frac{dy}{dx} = \frac{2x2^{ x }}{x^{ x }} + \frac{x^{ 2 }\cdot 2^{ x }(\ln(2)-\ln(x)-1)}{x^{ x }} \\
\text{ Для } x_{ 1 } = \frac{2\cdot 1\cdot 2}{1} + \frac{1^{ 2 }\cdot 2\cdot \ln(2)-\ln(1)-1}{1} = 4 + 2 \cdot (\ln(2)-1) = \boxed{2+2\ln(2)} \\
\text{ Для  } x_{ 2 } = \frac{2\cdot 2\cdot 4}{4} + \frac{2^{ 2 }\cdot 4\cdot (\ln(2)-\ln(2)-1)}{4} = 4-4 = \boxed{0}  
}$$
Ex 830.
$$\displaylines{
f'(2) - ? \quad f(x) = x^{ 2 }\sin{(x-2)} \\
f'(x) = 2x\sin{(x-2)} + x^{ 2 }\cos{(x-2)} \\
f'(2) = 2\cdot 2\cdot \sin{(0)} + 2^{ 2 }\cdot  \cos{(0)} = \boxed{4}
}$$
Ex 831.
$$\displaylines{
f'(1) - ? \quad f(x) = x+ (x-1) \arcsin{\left( \sqrt{ \frac{x}{x+1}  } \right)} \\
f'(x) = 1 + \arcsin{\left( \sqrt{ \frac{x}{x+1}  } \right)} +(x-1)\cdot \frac{1}{2\sqrt{ x  }(x+1)} \\
f'(1) = 1+ \arcsin{\left( \frac{\sqrt{ 2 }}{2}  \right)} = \boxed{1+ \frac{\pi}{4}}
}$$