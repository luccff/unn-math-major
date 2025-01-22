#### Определение скалярного произведения векторов в ${\displaystyle E^{ 3 }}$. Нахождение длины вектора и угла между векторами с помощью скалярного произведения. Связь скалярного произведения и умножение вектора на число.
---
Для двух векторов ${\displaystyle \vec{a} = ( a_{1}, \ a_{2}, \ a_{3})}$ и ${\displaystyle \vec{b} = ( b_{1}, \ b_{2}, \ b_{3})}$ в пространстве ${\displaystyle \overline{E}^{ 3 }}$ скалярное произведение определяется как:
$$\displaylines{
\vec{a} \cdot  \vec{b} = a_{1}b_{1} + a_{2}b_{2} + a_{3}b_{3}
}$$
Скалярным произведением ненулевых векторов ${\displaystyle \vec{a}}$ и ${\displaystyle \vec{b}}$ называется число, равное произведению длин векторов на косинус угла между ними.
$$\displaylines{
\vec{a} \cdot  \vec{b} = |\vec{a}| \cdot  |\vec{b}| \cdot  \cos{(\vec{a}, \  \vec{b})}
}$$

Пусть ${\displaystyle \vec{a}, \ \vec{b}}$ отложены от одной точки ${\displaystyle O}$: ${\displaystyle \overline{OA} = \vec{a}, \  \overline{OB} = \vec{ b}}$. Тогда углом между векторами называется наименьший из углов, образованных лучами ${\displaystyle OA}$ и ${\displaystyle OB}$.
Если ${\displaystyle \vec{a}\uparrow\uparrow\vec{b}}$, то ${\displaystyle \hat{(\vec{a}, \ \vec{b})}}$ = 0.
Если ${\displaystyle \vec{a}\uparrow\downarrow\vec{b}}$, то ${\displaystyle \hat{(\vec{a}, \ \vec{b})}}$ = ${\displaystyle \pi}$.
Если один из векторов равен нулевому, тогда угол между векторами не определен. 

Свойства скалярного произведения:
1. Положительная определенность скалярного произведения $(\vec{a}, \vec{a}) \stackrel{ \text{def} }{ = } \vec{a}^{2} \geq 0 \ \ \forall \overline{a} \in \overline{E}^{ 3 }$.
2. Коммутативность: ${\displaystyle \vec{a} \cdot \vec{ b} = \vec{b} \cdot \vec{a}}$.
3. Дистрибутивность: ${\displaystyle (\vec{a}, \ \vec{b}+ \vec{c}) = (\vec{a}, \ \vec{b}) + (\vec{a}, \ \vec{c}), \  \quad \forall{ \vec{a}, \ \vec{b}, \ \vec{c} \in \overline{E}^{ 3 }}}$.
Доказательство:
Свойство косинусов эквивалентно свойству дистрибутивности. 
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

4. Умножение на скаляр: ${\displaystyle (k\vec{a}) \cdot \vec{b} = k(\vec{a}\cdot\vec{b})}$, ${\displaystyle k \in \mathbb{R}}$.
Доказательство:
$$\displaylines{
\vec{a} = (a_{1}, \  a_{2}, \  a_{3}), \  \vec{b} = (b_{1}, \  b_{2}, \  b_{3}), \  k\vec{a} = (ka_{1}, \  ka_{2}, \  ka_{3}) \\
(k\vec{a}) \cdot  \vec{b} = (ka_{1})b_{1} + (ka_{2})b_{2} + (ka_{3})b_{3} =  \\
= k(a_{1}b_{1} + a_{2}b_{2} + a_{3}b_{3}) = k(\vec{a} \cdot  \vec{ b})
}$$


Связь с длинной вектора: ${\displaystyle \vec{a} \cdot \vec{a} = |\vec{a}| ^{  2 }}$
Доказательство:
$$\displaylines{
\vec{a} \cdot  \vec{a} = a_{1}^{ 2 }+a_{2}^{ 2 } + a_{3}^{ 2 } 
}$$
Сумма квадратов координат равна квадрату длины вектора:
$$\displaylines{
|\vec{a}|^{ 2 } = a_{1}^{ 2 }+a_{2}^{ 2 }+a_{3}^{ 2 } \\
\vec{a} \cdot  \vec{a} = |\vec{a}|^{ 2 }
}$$
Длинна вектора ${\displaystyle \vec{a} = (a_{1}, \ a_{2})}$ равна:
$$\displaylines{
|\vec{a}| = \sqrt{ \vec{a} \cdot  \vec{a} } = \sqrt{ {a}_{ 1 }^{ 2 } + {a}_{ 2 }^{ 2 } }
}$$
Косинусом угла между векторами называется:
$$\displaylines{
\cos{(\vec{a}, \  \vec{b})} = \frac{\vec{a} \cdot  \vec{b}}{|\vec{a}| \cdot  | \vec{b}|} 
}$$

Связь скалярного произведения и умножение вектора на число.
Умножение вектора на число изменяет длину вектора, а скалярное произведение пропорционально произведению длин векторов. Если вектор ${\displaystyle \vec{a}}$ удлиняется в ${\displaystyle \lambda}$ раз, то его "вклад" в скалярное произведение также увеличивается в ${\displaystyle \lambda}$ раз.
