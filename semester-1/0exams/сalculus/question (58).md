### Остаточный член формулы Тейлора в форме Пеано. Вывести.
---
Пусть есть многочлен Тейлора:
$$\displaylines{
P_{ n }(x) = f(a) + f'(a)(x-a) + \frac{f''(a)}{2!}(x-a)^{ 2 } + \dots + \frac{f^{ (n) }(a)}{n!}(x-a)^{ n }  
}$$
По формуле Тейлора
$$\displaylines{
f(x) = P_{ n }(x) + R_{ n }(x)
}$$
можно выразить ${\displaystyle R_{ n }(x)}$:
$$\displaylines{
R_{ n }(x) = f(x) - P_{ n }(x)
}$$
 
Из определения видно, что ${\displaystyle R_{ n }(x)}$ имеет порядок малости выше, чем ${\displaystyle (x-a)^{ n }}$, то есть:
$$\displaylines{
R_{ n }(x) = o((x-a)^{ n }), \  x \to  a
}$$
