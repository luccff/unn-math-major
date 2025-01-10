### Первый замечательный предел и все следствия из него. Доказать.

$$\displaylines{
\lim_{ x \to 0 } {\frac{\sin{(x)}}{x}} = \lim_{ x \to 0 } {\frac{x}{\sin{(x)}}} = 1
}$$
Доказательство через геометрию:
Рассмотрим единичную окружность с центром в начале координат. Пусть угол $x$ (в радианах) соответствует дуге $AB$ на этой окружности. Тогда:
1. Площадь сектора ${\displaystyle OAB = \frac{x}{2}}$
2. Площадь треугольника ${\displaystyle OAB = \frac{1}{2} \sin{(x)}}$
3. Площадь треугольника ${\displaystyle OAC = \frac{1}{2} \tan{(x)}}$
$$\displaylines{
\frac{1}{2}\sin{(x)}< \frac{x}{2} < \frac{1}{2} \tan{(x)} \\
\sin{(x)}< x < \tan{(x)} \ |:\sin{(x)}\cdot \cos{(x)}\\
\cos{(x)}< \frac{\sin{(x)}}{x} < \frac{1}{\cos{(x)}} \\
\text{ при } x \to  0 \text{ получаем } 1 < \frac{\sin{(x)}}{x} < 1 \\
\text{ По теореме о двух миллиционерах получаем } \lim_{ x \to 0 } {\frac{\sin{(x)}}{x} = 1}
}$$
Доказательство через разложение в окрестности нуля:
$$\displaylines{
\lim_{ x \to 0 } {\frac{\sin{(x)}}{x}} 
}$$
Разложим в ряд Тейлора ${\displaystyle \sin{(x)}}$:
$$\displaylines{
\sin{(x)} = x - \frac{x^{ 3 }}{3!} + \frac{x^{ 5 }}{5!} - \dots
}$$
Тогда
$$\displaylines{
\lim_{ x \to 0 } {\frac{x - \cfrac{x^{ 3 }}{3!} + \cfrac{x^{ 5 }}{5!} - \dots }{x} } = \lim_{ x \to 0 } {1- \frac{x^{ 2 }}{6} + \frac{x^{ 4 }}{120} - \dots } = \lim_{ x \to 0 } {1 - 0 + 0 - \dots } = 1
}$$
**Следствия из первого замечательного предела:**
1. 
$$\displaylines{
\lim_{ x \to 0 } {\frac{\tan{(x)}}{x}} = 1
}$$
Доказательство:
$$\displaylines{
\frac{\tan{(x)}}{x} = \frac{\sin{(x)}}{x \cdot  \cos{(x)}} = \frac{\sin{(x)}}{x} \cdot  \frac{1}{\cos{(x)}} \\
\lim_{ x \to 0 } {\frac{\sin{(x)}}{x} \cdot  \frac{1}{\cos{(x)}}} = 1 \cdot  1 = 1
}$$
2. 
$$\displaylines{
\lim_{ x \to 0 } {\frac{\arcsin{(x)}}{x} = 1}
}$$
Доказательство:
$$\displaylines{
\text{ Пусть  } y = \arcsin{(x)}, \  x = \sin{(y)} \\
\lim_{ x \to 0 } {\frac{\arcsin{(x)}}{x} } = \lim_{ x \to 0 } {\frac{y}{\sin{(y)}}} = \left( \lim_{ x \to 0 } {\frac{\sin{(y)}}{y}} \right)^{ -1 } = 1^{ -1 } = 1
}$$
3. 
$$\displaylines{
\lim_{ x \to 0 } {\frac{\arctan{(x)}}{x} = 1}
}$$
Доказательство:
$$\displaylines{
\text{ Пусть } y = \arctan{(x)}, \ x = \tan{(y)} \\
\lim_{ x \to 0 } {\frac{\arctan{(x)}}{x}} = \lim_{ x \to 0 } {\frac{y}{\tan{(y)}}} = 1
}$$
