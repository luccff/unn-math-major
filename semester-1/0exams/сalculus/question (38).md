### Производные всех элементарных функций – вывести.
---
Производная постоянной функции:
$$\displaylines{
f(x) = C \\
f'(x) = \lim_{ \Delta x \to 0} {\frac{C-C}{\Delta x} } = 0
}$$
Производная линейной функции:
$$\displaylines{
f(x) = x\\
f'(x) = \lim_{ \Delta x \to 0} {\frac{x + \Delta x - x}{\Delta x} } = 1
}$$
Производная степенной функции:
$$\displaylines{
f(x) = x^{ n }, \  n \in  \mathbb{R} \\
f'(x) = \lim_{ \Delta x \to 0 } {\frac{(x+\Delta x)^{ n }-x^{ n }}{\Delta x} } \\\\
(x+\Delta x)^{ n } = x^{ n }+ nx^{ n -1}\Delta x + \dots \\ \\
f'(x) = \lim_{ \Delta x \to 0 } {\frac{nx^{ n-1 }\Delta x+\dots }{\Delta x} } = nx^{ n-1 } \\\\
f'(x) = nx^{ n-1 }
}$$
Производная показательной функции:
$$\displaylines{
f(x) = a^{ x }, \   a>0 \\
f'(x) = \lim_{ \Delta x \to 0 } {\frac{a^{ x+\Delta x }+a^{ x }}{\Delta x} } = a^{ x }\lim_{ \Delta x \to 0 } {\frac{a^{ \Delta x }-1}{\Delta x} } = a^{ x }\ln(a)
}$$
Производная логарифмической функции:
$$\displaylines{
f(x) = \ln(x), \  x>0 \\
f'(x) = \lim_{ \Delta x \to 0 } {\frac{\ln(x+\Delta x)-\ln(x)}{\Delta x} } = \lim_{ \Delta x \to 0 } {\frac{\ln\left( 1+\cfrac{\Delta x}{x} \right)}{\Delta x} } = \\ = \frac{1}{x}\lim_{ \Delta x \to 0 } {\frac{\ln\left( 1+\cfrac{\Delta x}{x} \right)}{\cfrac{\Delta x}{x}} } = \frac{1}{x} 
}$$
Производная синусоиды:
$$\displaylines{
f(x) = \sin{(x)} \\
f'(x) = \lim_{ \Delta x \to 0 } {\frac{\sin{(x + \Delta x)}- \sin{(x)}}{\Delta x} } = \lim_{ \Delta x \to 0 } {\frac{\cos{\left( x + \cfrac{\Delta x}{2}  \right) \cdot \sin{\left( \cfrac{\Delta x}{2}  \right)}}}{\cfrac{\Delta x}{2}} } = \\
= \lim_{ \Delta x \to 0 } {\cos{\left( x+ \cfrac{\Delta x}{2}  \right)} } = \cos{(x)}
}$$
Производная косинусоиды:
$$\displaylines{
f(x) = \cos{(x)} \\
\text{ Аналогично, только будет } -\sin{(x)}
}$$
Производная тангенса:
$$\displaylines{
f(x) = \tan{(x)} = \frac{\sin{(x)}}{\cos{(x)}} \\
f'(x) = \frac{\sin{(x)'\cdot \cos{(x)}-\sin{(x)}\cdot \cos{(x)}'}}{\cos{(x)}^{ 2 }} = \frac{\cos{(x)}^{ 2 }+\sin{(x^{ 2 })}}{\cos{(x)}^{ 2 }} = \frac{1}{\cos{(x)^{ 2 }}}  
}$$
Производная котангенса:
$$\displaylines{
f(x) = \cot{(x)} = \frac{\cos{(x)}}{\sin{(x)}} \\
f'(x) = \frac{\cos{(x)}'\sin{(x)}-\cos{(x)}\sin{(x)}'}{\sin{(x)}^{ 2 }} = \frac{-\sin{(x)}^{ 2 }-\cos{(x)^{ 2 }}}{\sin{(x)}^{ 2 }} = -\frac{1}{\sin{(x)}^{ 2 }}  
}$$
Производная арксинуса:
$$\displaylines{
f(x) = \arcsin{(x)} \\
x = \sin{(f(x) )} \\
1 = \cos{(f(x) )} \cdot f'(x)  \\
f'(x)  = \frac{1}{\cos{(f(x))}} \\
\sin{(f(x))}^{ 2 } + \cos{(f(x) )}^{ 2 } = 1 \\
\cos{(f(x))} = \sqrt{ 1-x^{ 2 } } \\
f'(x) = \frac{1}{\sqrt{ 1-x^{ 2 } }}
}$$
Производная арккосинуса:
$$\displaylines{
f(x) = \arccos{(x)} \\
x = \cos{(f(x))} \\
1 = -\sin{(f(x))} \cdot  f'(x) \\
f'(x) = -\frac{1}{\sin{(f(x))}} \\
\sin{(f(x))} = \sqrt{ 1 - x^{ 2 }} \\
f'(x) = -\frac{1}{\sqrt{ 1-x^{ 2 } }}
}$$
Производная арктангенса:
$$\displaylines{
f(x) = \arctan{(x)} \\
x = \tan{(f(x))} \\
1 = \frac{1}{\cos{(f(x) )}^{ 2 }} \cdot  f'(x) \\
f'(x) = \cos{(f(x) )}^{ 2 } \\
f'(x) = \frac{1}{1+x^{ 2 }}
}$$

