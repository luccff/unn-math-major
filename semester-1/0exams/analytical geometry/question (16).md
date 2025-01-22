#### Определение и свойства векторного произведения.
---
Пусть ${\displaystyle \vec{a}, \ \vec{b}, \  \vec{c}}$ - упорядоченная тройка некомпланарных векторов. Векторное произведение ${\displaystyle \vec{a}\times\vec{b}}$ определяется как вектор, удовлетворяющим следующим условиям:
1. Направление: ${\displaystyle \vec{a}, \ \vec{b}}$ - перпендикулярно плоскости, содержащей эти вектора, а направление определяется по правилу правой руки: если разместить указательный палец правой руки на первом векторе, а средний на втором, то отогнутый перпендикулярно к ладони большой палец покажет примерное направление произведения векторов. 
![[Pasted image 20250119153935.png]]
    Вектор $\vec{c}$, полученный в результате векторного произведения $\vec{a} \times \vec{b}$ , направлен так, чтобы наименьшее вращение от $\vec{a}$ к $\vec{b}$ вокруг вектора $\vec{c}$ осуществлялось против часовой стрелки, если смотреть с конца вектора $\vec{c}$.
![[Pasted image 20250119154420.png]]
2. Длинна вектора ${\displaystyle \vec{a}\times\vec{b}}$: ${\displaystyle |\vec{a}\times\vec{b}| = |\vec{a}| \cdot |\vec{b}| \cdot \sin{(\vec{a}, \ \vec{b})}}$.
3. Вектор ${\displaystyle \vec{a}\times\vec{b}}$ определяется однозначно, кроме случая ${\displaystyle \vec{a} || \vec{b}}$, где результат равен ${\displaystyle \vec{0}}$.

### Свойства векторного произведения
1. Геометрический смысл длинны векторного произведения - площадь параллелограмма, построенного на этих векторах.
2. Перпендикулярность результата: ${\displaystyle \vec{a} \times \vec{b} \perp \vec{a}, \  \vec{a}\times\vec{b} \perp \vec{b}}$.
3. Антикоммутативность: ${\displaystyle \vec{a}\times\vec{b} = - (\vec{b} \times \vec{a})}$.
4. Ассоциативность по умножению на скаляр: ${\displaystyle k(\vec{a}\times\vec{b}) = (k\vec{a}) \times \vec{b} = \vec{a} \times (k\vec{b}), \ k \in \mathbb{R}}$.
5. Дистрибутивность: ${\displaystyle \vec{a} \times (\vec{b} + \vec{c}) = (\vec{a} \times \vec{b}) + (\vec{a} \times \vec{c})}$.
6. Собственный результат: ${\displaystyle \vec{a} \times \vec{a} = \vec{0}}$.
7. ${\displaystyle \vec{a} \times \vec{b} = \vec{0} \iff |\vec{a}\times\vec{b}| = 0 \iff |\vec{a}| \cdot |\vec{b}| \cdot \sin{(\vec{a}, \ \vec{b})}}$ если ${\displaystyle |\vec{a}| = 0}$ или ${\displaystyle |\vec{b}| = 0}$ или ${\displaystyle \sin{(\vec{a}, \ \vec{b})} = 0: \hat{(\vec{a}, \ \vec{b})} = 0^{ \circ }}$ или ${\displaystyle \pi }$.
8. Смешанное произведение: ${\displaystyle (\vec{a} \times \vec{b}) \cdot \vec{c} = \begin{vmatrix} a_{1} & a_{2} & a_{3} \\ b_{1} & b_{2} & b_{3} \\ c_{1}&c_{2}&c_{3} \end{vmatrix} }$
