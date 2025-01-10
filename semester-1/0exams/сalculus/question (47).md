### Производные высших порядков от явно заданной функции; от функции, заданной параметрически. Производная n-ого порядка от показательной функции, логарифмической функции, ${\displaystyle \sin{(x)}}$, ${\displaystyle \cos{(x)}}$. Формула Лейбница производной n-ого порядка от произведения функции. Вторая производная от функции, заданной параметрически.
---
Определение. Производные высших порядков - это последовательные производные функции. Обозначаются как:
$$\displaylines{
f''(x) = \frac{d^{ 2 }f}{dx^{ 2 }}, \   f^{ (n) } = \frac{d^{ n }f}{dx^{ n }}  
}$$
Производные высших порядков от явно заданных функций:

Показательная функция:
$$\displaylines{
f^{ (n) }(x) = e^{ x }, \  \forall{n}
}$$
Логарифмическая функция:
$$\displaylines{
y = \ln(x)\\
y' = \frac{1}{x} = x^{ -1 }\\
y''=(x^{ -1 })' = -x^{ -2 } \\
y''' = -1(-2)x^{ -3 } \\
y^{ (4) } = -1(-2)(-3)x^{ -4 }\\
\cdots\\
y^{ (n) } = (-1)^{ n+1 }(n-1)! \cdot  x^{ -n }
}$$
Производная синуса:
$$\displaylines{
f(x) = \sin{(x)}, \  f^{ (n) }(x) = \begin{cases}
\sin{(x)}, \   & n = 4k \\
\cos{(x)}, \   & n = 4k+1 \\
-\sin{(x)}, \   & n = 4k+2 \\
-\cos{(x)}, \   & n = 4k+3
\end{cases} \\ \\
\displaylines{
y = \sin{(x)} \\
y' = \cos{(x)} = \sin{\left( x + \frac{\pi}{2} \right)} \\
y'' = -\sin{(x)} = \sin{\left( x+\frac{2\pi}{2} \right)} \\
y''' = -\cos{(x)} = \sin{\left( x+\frac{3\pi}{2} \right)} \\
\dots \\
y^{ (n) } = \sin{\left( x+\frac{n\pi}{2} \right)}
}
}$$
Производная косинуса:
$$\displaylines{
f(x) = \cos{(x)}, \  f^{ (n) }(x) = \begin{cases}
\cos{(x)}, \  &  n = 4k \\
-\sin{(x)}, \  &  n = 4k+1 \\
-\cos{(x)}, \  &  n = 4k+2  \\
\sin{(x)}, \   &  n = 4k+3
\end{cases} \\ \\
y = \cos{(x)} \\ 
y' = -\sin{(x)} = \cos{\left( x+\frac{\pi}{2} \right)} \\
y'' = -\cos{(x)} = \cos{\left( x + \frac{2\pi}{2} \right)} \\
y''' = \sin{(x)} = \cos{\left( x+\frac{3\pi}{2} \right)} \\
\dots \\
y^{ (n) } = \cos{\left( x+\frac{n\pi}{2} \right)}
}$$

Формула Лейбница для ${\displaystyle n}$-ой производной произведения функции:
$$\displaylines{
(f\cdot g)^{ (n) } = \sum_{k=0}^{n} \binom{n}{k} f^{ (n-k) } \cdot g^{ (k) }
}$$

Производная второго порядка для функции, заданной параметрически:
$$\displaylines{
x = x(t), \  y = y(t) \\
\dfrac{dy}{dx} = \cfrac{\dfrac{dy}{dt}}{\dfrac{dx}{dt}} \\
\dfrac{d^{ 2 }y}{dx^{ 2 }} = \cfrac{\dfrac{d}{dt}\left( \cfrac{dy}{dx}  \right)}{\cfrac{dx}{dt} } 
}$$