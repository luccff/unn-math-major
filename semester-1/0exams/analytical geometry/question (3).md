#### Базис. Свойства координат вектора. Базисы в ${\displaystyle \overline{E}^{ 2 }}$ и в ${\displaystyle \overline{E}^{ 3 }}$
---
Базис векторного пространства ${\displaystyle V}$ - это упорядоченная система линейно независимых векторов ${\displaystyle \{ e_{ 1 }, \ e_{ 2 }, \ \dots, \ \vec{e}_{ n } \}}$, которая порождает всё пространство ${\displaystyle V.}$ Это значит, что:
1. Любой вектор пространства ${\displaystyle V}$ может быть представлен как линейная комбинация остальных. 
$$\displaylines{
\vec{v} = \sum_{i=1}^{n} \alpha_{ i } \cdot \vec{e}_{ i } 
}$$
где ${\displaystyle \alpha_{ 1 }, \ \alpha_{ 2 }, \ \dots}$ - скаляры, называемые координатами вектора ${\displaystyle \vec{v}}$ в данном базисе.
2. Базис должен быть линейно независимым
$$\displaylines{
\sum_{i=1}^{n} \alpha_{ i } \cdot \vec{e}_{ i } = \vec{0} \implies \alpha_{ 1 }=\dots =a_{n} = 0
}$$
3. Число векторов в базисе равно размерности пространства ${\displaystyle V}$.
Если в векторном пространстве существует базис из конечно числа векторов, то он называется конечно мерным. Число векторов базиса называется размерностью пространства. 

Коэффициенты разложения вектора по векторам базиса называется координатами вектора относительно данного базиса.
### Свойства координат вектора
1. Единственность представления:
    В любом базисе каждый вектор ${\displaystyle \vec{v} \in V}$ имеет единственное разложение по векторам:
$$\displaylines{
\vec{v} = \sum_{i=1}^{n} c_{ i } \cdot \vec{e}_{ i } 
}$$
    Координаты ${\displaystyle c_{ 1 }, \ \dots , \ c_{n}}$ - уникальны.
    Доказательство:
    Предположим, что есть два разложения ${\displaystyle \vec{x} = x^{ 1 }\vec{e}_{ 1 } + \dots + x^{ n }\vec{e}_{ n }}$ и ${\displaystyle \vec{x} = y^{ 1 }\vec{e}_{ 1 }+\dots+y^{ n }\vec{e}_{ n }}$. Вычтем один вектор из другого и получаем:
$$\displaylines{
\vec{0} = (x^{ 1 }-y^{ 1 }) \vec{e}_{ 1 } + \dots  + (x^{ n }-y^{ n })\vec{e}_{ n }
}$$
    Что представляет собой линейную комбинацию базисных векторов равную нулевому вектору. Так как базисные вектора линейно независимы, то получаем, что линейная комбинация обязана быть тривиальной, следовательно: ${\displaystyle x^{ 1 } = y^{  1 } , \ \dots, \ x^{ n } = y^{ n }}$. 
2. Пусть есть базис ${\displaystyle B = \{ \vec{e}_{ 1 }, \ \dots, \ \vec{e}_{ n } \}}$.  ${\displaystyle \vec{a} = (a_{1}, \ \dots a_{n})_{ B }}$ и ${\displaystyle \vec{b} = (b_{ 1 }, \ \dots, \ b_{n})_{ B }}$.
Сумма и разность: 
$$\displaylines{
\vec{a} \pm  \vec{b} = (a_{1}\pm b_{1}, \   a_{2}\pm b_{2}, \  \dots , \  a_{n}\pm b_{n} )_{ B }
}$$
Доказательство:
$$\displaylines{
\vec{a} + \vec{b} \implies \sum_{ i = 1 }^{ n } a_{ i } \cdot \vec{e_{ 1 }} = \sum_{ i = 1 }^{ n } (a_{ i } + b_{ i }) \cdot \vec{e_{ i }} = \vec{a} + \vec{b} = (a_{ 1 } + b_{ 1 }, \dots, a_{ n } + b_{ n })_{ B }
}$$
Умножение на скаляр:
$$\displaylines{
\alpha\vec{a} = (\alpha a_{1}, \   \alpha a_{ 2 }, \  \dots , \  \alpha a_{n})_{ B }
}$$

3. Коллинеарность в ${\displaystyle \overline{E}^{ 2 }}$:
$$\displaylines{
\vec{a} = (a_{ 1 }, a_{ 2 })_{ B } \\ 
\vec{b} = (b_{ 1 }, b_{ 2 })_{ B } \\ 
\vec{a} || \vec{b} \iff  \begin{vmatrix}a_{ 1 } & a_{ 2 } \\ b_{ 1 } & b_{ 2 }\end{vmatrix} = 0 \\ 
\underset{ \vec{a} \neq 0 }{ \vec{a} || \vec{b} } \implies \exists \alpha \mid \vec{b} = \alpha \cdot \vec{a} \\ 
(b_{ 1 }, b_{ 2 }) = (\alpha \cdot a_{ 1 }, \alpha \cdot a_{ 2 }) \\ 
\begin{vmatrix}a_{ 1 } & a_{ 2 } \\ \alpha \cdot a_{ 1 } & \alpha \cdot a_{ 2 }\end{vmatrix} = 0 \\ 
\det= a_{1} \cdot  (\alpha \cdot  a_{ 2 }) - a_{2} \cdot  (\alpha \cdot  a_{ 1 }) = 0
}$$
В обратную сторону:
$$\displaylines{
\begin{vmatrix}
a_{1} & a_{2} \\
b_{1} & b_{2}
\end{vmatrix} = 0 \implies \vec{a}||\vec{b} \\
\text{Пусть } a_{ 1 } \neq 0 \\ 
a_{ 1 } \cdot b_{ 2 } - a_{ 2 } \cdot b_{ 1 } = 0 \implies b_{ 2 }= \frac{a_{ 2 }}{a_{ 1 }} \cdot b_{ 1 } \implies \vec{b} = (b_{1}, \  b_{2}) = \left( b_{1}, \  \frac{a_{2}}{a_{1}} \cdot  b_{1} \right) = b_{1} \cdot  \left( 1, \  \frac{a_{2}}{a_{1}} \right)
}$$
Это показывает, что ${\displaystyle \vec{b}}$ является линейной комбинацией ${\displaystyle \vec{a} \implies \vec{b}||\vec{a}}$. 
Если ${\displaystyle a_{1} = 0}$, то ${\displaystyle a_{2} \neq 0 (\text{иначе } \vec{ a} = \vec{0})}$. Тогда из уравнения:
$$\displaylines{
0 \cdot  \vec{b_{2}} - a_{2} \cdot  b_{1} = 0 \implies  b_{1} = 0
}$$
Значит ${\displaystyle \vec{b } = (0, \ b_{2})}$ и ${\displaystyle \vec{b}||\vec{a}}$. Это доказывает, что координаты векторов пропорциональны, а значит, векторы коллинеарны.

### Базисы в ${\displaystyle \overline{E}^{ 2 }}$ и ${\displaystyle \overline{E}^{ 3 }}$
Базис в ${\displaystyle \overline{E}^{ 2 }}$:
1. ${\displaystyle \dim \overline{E}^{ 2 } = 2}$.
2. Базис состоит из двух линейно независимых векторов, например:
$$\displaylines{
e_{ 1 } = (1, \  0), \  e_{ 2 } = (0, \  1)
}$$
3. Любой вектор ${\displaystyle \vec{v} = ( x, \ y)}$ представим в виде:
$$\displaylines{
\vec{v} = x \cdot  e_{ 1 } + y \cdot  e_{ 2 }
}$$

Базис в ${\displaystyle \overline{E}^{ 3 }}$:
1. ${\displaystyle \dim \overline{E}^{ 3 } = 3}$.
2. Базис состоит из трех линейно независимых векторов, например:
$$\displaylines{
e_{ 1 } = (1, \  0, \  0), \  e_{ 2 } = (0, \  1, \  0), \  e_{ 3 } = ( 0, \  0, \  1)
}$$
3. Любой вектор ${\displaystyle \vec{v} = ( x, \ y, \ x)}$ представим в виде:
$$\displaylines{
\vec{v} = x \cdot  e_{ 1 } + y \cdot  e_{ 2 } + z \cdot  e_{ 3 }
}$$
