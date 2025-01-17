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
3. Дистрибутивность: ${\displaystyle \vec{a} \cdot (\vec{b} + \vec{c}) = \vec{a} \cdot \vec{ b} + \vec{a} \cdot \vec{ c}}$
Доказательство:
$$\displaylines{
\vec{a} = (a_{1}, \  a_{2}, \  a_{3}), \  \vec{b} = (b_{1}, \  b_{2}, \  b_{3}), \  \vec{c} = (c_{1}, \  c_{2}, \  c_{3}) \\
\vec{a} \cdot  ( \vec{b} + \vec{c}) = a_{1}(b_{1}+c_{1}) + a_{2}(b_{2}+c_{2}) + a_{3}(b_{3}+c_{3}) = \\
= a_{1}b_{1} + a_{1}c_{1} + a_{2}b_{2} + a_{2}c_{2} + a_{3}b_{3} + a_{3}c_{3} = \\
= (a_{1}b_{1} + a_{2} b_{2} + a_{3} b_{3}) + ( a_{1} c_{1} + a_{2}c_{2} + a_{3}c_{3}) = \vec{a} \cdot  \vec{b} + \vec{a} \cdot  \vec{ c}
}$$
4. Умножение на скаляр: ${\displaystyle (k\vec{a}) \cdot \vec{b} = k(\vec{a}\cdot\vec{b})}$, ${\displaystyle k \in \mathbb{R}}$.
Доказательство:
$$\displaylines{
\vec{a} = (a_{1}, \  a_{2}, \  a_{3}), \  \vec{b} = (b_{1}, \  b_{2}, \  b_{3}), \  k\vec{a} = (ka_{1}, \  ka_{2}, \  ka_{3}) \\
(k\vec{a}) \cdot  \vec{b} = (ka_{1})b_{1} + (ka_{2})b_{2} + (ka_{3})b_{3} =  \\
= k(a_{1}b_{1} + a_{2}b_{2} + a_{3}b_{3}) = k(\vec{a} \cdot  \vec{ b})
}$$
5. Связь с длинной вектора: ${\displaystyle \vec{a} \cdot \vec{a} = |\vec{a}| ^{  2 }}$
Доказательство:
$$\displaylines{
\vec{a} \cdot  \vec{a} = a_{1}^{ 2 }+a_{2}^{ 2 } + a_{3}^{ 2 } 
}$$
Сумма квадратов координат равна квадрату длины вектора:
$$\displaylines{
|\vec{a}|^{ 2 } = a_{1}^{ 2 }+a_{2}^{ 2 }+a_{3}^{ 2 } \\
\vec{a} \cdot  \vec{a} = |\vec{a}|^{ 2 }
}$$
6. ${\displaystyle (\vec{a}, \vec{b} + \vec{c}) = (\vec{a}, \vec{b}) + (\vec{a}, \vec{c}), \ \ \forall \vec{a}, \vec{b}, \vec{c} \in \overline{E}^{ 3 }}$

Длинна вектора ${\displaystyle \vec{a} = (a_{1}, \ a_{2})}$ равна:
$$\displaylines{
|\vec{a}| = \sqrt{ \vec{a} \cdot  \vec{a} } = \sqrt{ {a}_{ 1 }^{ 2 } + {a}_{ 2 }^{ 2 } }
}$$
Косинусом угла между векторами называется:
$$\displaylines{
\cos{(\vec{a}, \  \vec{b})} = \frac{\vec{a} \cdot  \vec{b}}{|\vec{a}| \cdot  | \vec{b}|} 
}$$

Вещественное векторное пространство $V$ называется Евклидовым векторным пространством, если каждой упорядоченной паре векторов $\vec{a}, \vec{b}$ поставлено в соответствие число $(\vec{a}, \vec{b})$, которое называется скалярным произведением. При этом должны выполнены свойства скалярного произведения. 
$$\displaylines{
\vec{a}, \vec{b} \to (\vec{a}, \vec{b})
}$$