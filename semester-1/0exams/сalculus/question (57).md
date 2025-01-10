### Порядок касания (степень близости) функций. Многочлен Тейлора. Формула Тейлора. Формула Маклорена.
---
*Определение*. Две функции ${\displaystyle f(x) \wedge g(x)}$ имеют **порядок касания** ${\displaystyle k}$ в точке ${\displaystyle x = a}$, если разность ${\displaystyle f(x) - g(x)}$ имеет порядок малости ${\displaystyle o((x-a)^{ k })}$, то есть:
$$\displaylines{
f(x) - g(x) = o((x-a)^{ k }), \  \text{ при } x \to  a
}$$
Это означает, что функции совпадают в точке ${\displaystyle a}$ вместе с их первыми ${\displaystyle k}$ производными:
$$\displaylines{
f(a) = g(a), \  f'(a) = g'(a), \  \dots , \  f^{ (k) } (a)= g^{ (k) }(a)
}$$
Если ${\displaystyle k =\infty}$, то говорят, что функции касательно совпадают в точке ${\displaystyle a}$.

*Определение*. Многочлен Тейлора порядка ${\displaystyle n}$ для функции ${\displaystyle f(x)}$ в точке ${\displaystyle a}$ - это полином, который аппроксимирует функцию ${\displaystyle f(x)}$ с точностью до порядка ${\displaystyle n}$ включительно:
$$\displaylines{
P_{ n }(x) = f(a) + f'(a)(x-a) + \frac{f''(a)}{2!}(x-a)^{ 2 } + \dots + \frac{f^{ (n) }(a)}{n!}(x-a)^{ n }  
}$$
**Формула Тейлора**.
Для любого ${\displaystyle x}$ вблизи ${\displaystyle a}$ функция ${\displaystyle f(x)}$ может быть записана в виде:
$$\displaylines{
f(x) = P_{ n }(x) + R_{ n }(x)
}$$
где ${\displaystyle R_{ n }(x)}$ - остаточный член (ошибка аппроксимации), который обычно записывают в форме Лагранжа:
$$\displaylines{
R_{ n }(x) = \frac{f^{ (n+1) }(\xi)}{(n+1)}(x-a)^{ n+1 }, \  \quad   \xi \in (a, \  x) 
}$$
Формула Маклорена.
Это частный случай формулы Тейлора, где ${\displaystyle a = 0}$:
$$\displaylines{
f(x) = f(0) + f'(0)x + \frac{f''(0)}{2!}x^{ 2 } + \dots + \frac{f^{ (n) }(0)}{n!}x^{ n } + R_{ n }(x)
}$$