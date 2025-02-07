### Производная от функции, заданной неявно. Уметь вычислять для конкретных приме ров.
---
Определение. Если функция задана неявна, то есть уравнением вида:
$$\displaylines{
F(x, \  y) = 0, \  
}$$
то для нахождения производной производной ${\displaystyle y'(x)}$ используют неявное дифференцирование.

$$\displaylines{
\frac{d}{dx}[F(x, \  y)] = \frac{\partial F}{\partial x} + \frac{\partial F}{\partial y}\cdot \dfrac{dy}{dx}  
}$$
И производная ${\displaystyle y'(x)}$ будет равна:
$$\displaylines{
\dfrac{dy}{dx} = -\frac{\cfrac{\partial F}{\partial x} }{\cfrac{\partial F}{\partial y} } 
}$$
Пример:
$$\displaylines{
F(x, \  y) = x^{ 2 }+y^{ 2 }-1 = 0 \\
\frac{\partial{F}}{\partial x} = 2x, \   \quad \frac{\partial F}{\partial y} = 2y \\
y'(x) = -\frac{2x}{2y} = -\frac{x}{y} 
}$$
Пример:
$$\displaylines{
F(x, \  y) = x^{ 3 }+y^{ 3 }-3xy = 0 \\
\frac{\partial F}{\partial x} = 3x^{ 2 }-3y, \   \quad \frac{\partial F}{\partial y} = 3y^{ 2 }-3x \\
y'(x) = -\frac{3x^{ 2 }-3y}{3y^{ 2 }-3x} 
}$$

$$\displaylines{
f(x, \  y) = \begin{cases}
\dfrac{2xy}{\sqrt{ x^{ 2 } + y^{ 2 } }}  & (x, \  y) \neq (0, \  0) \\
0  & (x, \  y) = (0, \  0) 
\end{cases}
}$$