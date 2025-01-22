#### Дистрибутивность скалярного произведения относительно сложения векторов.
---
Дистрибутивность: ${\displaystyle (\vec{a}, \ \vec{b}+ \vec{c}) = (\vec{a}, \ \vec{b}) + (\vec{a}, \ \vec{c}), \  \quad \forall{ \vec{a}, \ \vec{b}, \ \vec{c} \in \overline{E}^{ 3 }}}$.
Доказательство: cвойство косинусов эквивалентно свойству дистрибутивности. 
$$\displaylines{
\vec{AC} + \vec{CB} = \vec{AB} \\ 
\vec{CB} = \vec{AB} - \vec{AC} = \vec{c} - \vec{b} \\
\vec{CB}^{ 2 } = |\vec{c}-\vec{b}|^{ 2 } = |\vec{c}|^{ 2 } + |\vec{b}|^{ 2 } - 2\cos{(\alpha)} \cdot |\vec{c}| \cdot |\vec{b}| = |\vec{c}|^{ 2 } + |\vec{b}|^{ 2 } - 2(\vec{c}, \  \vec{b})
}$$
Пусть ${\displaystyle \vec{b} \to - \vec{b}}$:
$$\displaylines{
|\vec{c}+\vec{b}| ^{ 2 } = (\vec{c}, \  \vec{c}) + (\vec{b}, \  \vec{b}) + 2 (\vec{c}, \  \vec{b})
}$$
Пусть ${\displaystyle \vec{b} \to (\vec{x} + \vec{y})}$:
$$\displaylines{
|\vec{c}+ (\vec{x}+ \vec{y})| ^{ 2 } = (\vec{c}, \  \vec{c}) + |(\vec{x}+\vec{y})|^{ 2 } + 2(\vec{c}, \   \vec{x}+\vec{y}) \\
\text{ Где } |(\vec{x}+\vec{y})|^{ 2 } = (\vec{x}, \  \vec{x}) + (\vec{y}, \  \vec{y}) + 2(\vec{x}, \  \vec{y}) \\
\text{ Тогда } |\vec{c}+ (\vec{x}+ \vec{y})| ^{ 2 } = (\vec{c}, \  \vec{c}) + (\vec{x}, \  \vec{x}) + (\vec{y}, \  \vec{y}) + 2(\vec{x}, \  \vec{y}) + 2(\vec{c}, \   \vec{x}+\vec{y}) \\
}$$
Рассмотрим переход
$$\displaylines{
 (\vec{c}+(\vec{x}+\vec{y}))^{ 2 } = \vec{c}^{ 2 } + \vec{x}^{ 2 } + \vec{y}^{ 2 } + 2(\vec{x}, \  \vec{y}) + 2(\vec{c}, \  \vec{x}+ \vec{y})  \quad (1) \\
 ((\vec{c}+\vec{x}) + \vec{y})^{ 2 } = \vec{c}^{ 2 } + \vec{x}^{ 2 } + \vec{y}^{ 2 }+ 2(\vec{c}, \  \vec{x}) + 2(\vec{c}+\vec{x}, \  \vec{y})  \quad (2) \\
 (1)-(2) \implies (\vec{x}, \  \vec{y}) + (\vec{c}, \   \vec{x} + \vec{y}) -  (\vec{c}, \  \vec{x}) -(\vec{c} + \vec{x}, \   \vec{y}) = 0  \\
 \vec{y} \to  -\vec{y}  \\
 -(\vec{x}, \  \vec{y}) + (\vec{c}, \  \vec{x} - \vec{y}) - (\vec{c}, \  \vec{x}) + (\vec{c}+ \vec{x}, \  \vec{y}) = 0  \quad ( 3) \\ \\
 (1) - (2) + (3) = (\vec{c} , \  \vec{x} + \vec{y}) + (\vec{c}, \  \vec{x} - \vec{y}) - 2(\vec{c}, \  \vec{x}) = 0 
}$$
Пусть ${\displaystyle \vec{x} + \vec{y} = \vec{a}}$ и ${\displaystyle \vec{x} - \vec{y} = \vec{b}}$:
$$\displaylines{
(\vec{c}, \   \vec{a}) + (\vec{c}, \  \vec{b}) = 2(\vec{c}, \   \vec{x}) \\
\vec{x} = \frac{\vec{a} + \vec{b}}{2} \\
(\vec{c}, \   \vec{a}) + (\vec{c}, \  \vec{b}) = 2\left( \vec{c}, \ \frac{\vec{a} + \vec{b}}{2}   \right) = (\vec{c}, \  \vec{a}+ \vec{b}) \\
}$$
Доказано.
