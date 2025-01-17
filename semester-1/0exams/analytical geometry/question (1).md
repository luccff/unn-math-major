#### Вещественное векторное пространство. Аксиомы. Примеры.
---
Вещественное векторное пространство — это множество, элементы которого называются **векторами**, на котором определены операции **сложения** и **умножения на число** (скаляр), подчиняющиеся определённым аксиомам.

### Аксиомы вещественного векторного пространства
Пусть ${\displaystyle V}$ - множество векторов, а ${\displaystyle \mathbb{R}}$ - множество вещественных чисел. На ${\displaystyle V}$ определены операции:
1. Сложение ${\displaystyle +: \ V \times V \to V}$
2. Умножение на число ${\displaystyle \cdot:}$ ${\displaystyle \mathbb{R} \times V \to V}$ 
Операции удовлетворяют следующим аксиомам:
1. Ассоциативность сложения:
$$\displaylines{
\forall{\vec{a}, \  \vec{b}, \   \vec{c} \in V: \ \vec{a}+(\vec{b}+\vec{c}) = (\vec{a}+\vec{b}) + \vec{c}}
}$$
2. Коммутативность сложения:
$$\displaylines{
\forall{\vec{a}, \  \vec{b} \in  V: \vec{a} + \vec{b} = \vec{b} + \vec{a}}
}$$
3. Нулевой элемент: ${\displaystyle \exists \vec{0} \in V: \forall{\vec{a} \in V: \vec{a} + \vec{0}} = \vec{a}}$
4. Обратный элемент: ${\displaystyle \forall{\vec{a}} \in V \ \exists -\vec{a}: \ \vec{a} + (-\vec{a}) = 0}$
5. Дистрибутивность умножения относительно сложения скаляров: 
$$\displaylines{
\forall{\alpha, \  \beta \in  \mathbb{R} }; \ \forall{\vec{a} \in  V \implies } (\alpha+\beta)\vec{a} = \alpha\vec{a} + \beta\vec{a}
}$$
6. Дистрибутивность умножения относительно сложения векторов:
$$\displaylines{
\forall{\gamma \in  \mathbb{R}}; \forall{\vec{a}, \  \vec{b} \in  V}: \gamma(\vec{a}+ \vec{b}) = \gamma\vec{a} + \gamma\vec{b}
}$$
7. Ассоциативность умножения скаляров:
$$\displaylines{
\forall{\alpha, \  \beta} \in  \mathbb{R} ; \ \forall \vec{a} \in  V: \ \alpha(\beta\vec{a}) = (\alpha\beta)\vec{a}
}$$
8. Умножение на единицу:
$$\displaylines{
\forall{\vec{a}} \in  V : 1 \cdot  \vec{a} = \vec{a}
}$$
Пусть ${\displaystyle V}$ - множество, для которого заданы два отображения ${\displaystyle f: X \to Y}$
Первое называется сложением и сопоставляет упорядоченной паре элементов из ${\displaystyle V}$ снова элемент из ${\displaystyle V}$:
$$\displaylines{
(\vec{a}, \  \vec{b}) \to \vec{a} + \vec{b}
}$$
Второе называется умножением вектора на число:
$$\displaylines{
(\alpha, \   \vec{a}) \to  \alpha\vec{a}, \   \ \alpha \in  \mathbb{R} ; \quad  \vec{a} \in  V
}$$Если отображения удовлетворяют аксиомам 1-8, то ${\displaystyle V}$ называется вещественным векторным пространством.

### Примеры

1. ${\displaystyle E ^{  n }}$, ${\displaystyle n = 2, \ 3}$ - множество векторов, построенное на аксиомах школьной геометрии.
2. Пространство ${\displaystyle \mathbb{R}^{ n }}$. Элементы - векторы-столбцы из ${\displaystyle n}$ вещественных чисел ${\displaystyle (x_{1}, \ x_{2}, \ \dots \ , \ x_{n})}$
        Операции: 
        1. Сложение: ${\displaystyle (x_{1}, \ \dots, \ x_{n})+ (y_{1}, \ \dots, \ y_{n}) = (x_{1}+y_{1}+\dots+x_{n}+y_{n})}$
        2. Умножение на число: ${\displaystyle a \cdot ( x_{1}, \ \dots, \ x_{n}) = (ax_{1}, \dots, \ ax_{n})}$
3.  Пространство матриц:
        Операции:
        1. Покомпонентное сложение матриц
        2. Умножение всех элементов матрицы на число
4. Пространство функций:
        Элементы - функции вида ${\displaystyle f: \mathbb{R} \to \mathbb{R}}$, для которых определены сложение ${\displaystyle (f+g)(x) = f(x) + g(x) }$ и умножение на число ${\displaystyle (a \cdot f)(x) = a \cdot f(x)}$