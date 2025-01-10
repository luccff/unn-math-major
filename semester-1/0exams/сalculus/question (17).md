### Доказать единственность предела функции.
---
Утверждение. Если существует предел числовой функции, то он единственен. 
Доказательство:
Пусть ${\displaystyle f(x)}$ имеет два различных предела в точке ${\displaystyle a: L_{ 1 } \wedge L_{ 2 }}$, где ${\displaystyle L_{ 1 } \neq L_{ 2 }}$.
Зададимся ${\displaystyle * \ \varepsilon = \cfrac{|L_{ 1 }-L_{ 2 }|}{2}}$. По определению предела функции, для ${\displaystyle \varepsilon>0 \ \exists\delta_{ 1 }, \ \delta_{ 2 } > 0}$:
$$\displaylines{
0< |x-a| <\delta_{ 1 } \hookrightarrow |f(x) - L_{ 1 }| < \varepsilon \\
0< |x-a| <\delta_{ 2 } \hookrightarrow |f(x) - L_{ 2 }| < \varepsilon
}$$
Обозначим, что ${\displaystyle \delta = \min(\delta_{ 1 },\ \delta_{ 2 })}$, тогда ${\displaystyle \forall{x} : 0<|x-a|<\delta}$ выполняются оба неравенства:
$$\displaylines{
|f(x)-L_{ 1 }| <\varepsilon \\
|f(x)-L_{ 2 }| <\varepsilon
}$$
Тогда
$$\displaylines{
|L_{ 1 }-L_{ 2 }| = |L_{ 1 } - f(x)| + |f(x) - L_{ 2 }| < \varepsilon + \varepsilon = 2\varepsilon
}$$
Подставляя ${\displaystyle \varepsilon = *}$ получаем:
$$\displaylines{
|L_{ 1 } -L_{ 2 }| < |L_{ 1 }-L_{ 2 }|
}$$
Противоречие. 