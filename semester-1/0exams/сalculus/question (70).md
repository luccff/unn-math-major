### Дифференциал дуги. Доказать эквивалентность длины дуги, длины хорды и диффе ренциала дуги при условии, что приращение аргумента стремится к нулю. Направляющие косинусы касательной и векторная функция, задающая кривую с помощью параметрических уравнений относительно длины дуги.
---
Рассмотрим гладкую кривую ${\displaystyle \Gamma}$ в пространстве заданную параметрически, где ${\displaystyle r(t)}$ её векторное представление:
$$\displaylines{
r(t) = (x(t), \  y(t), \  z(t)), \  t \in  [a, \  b]
}$$
где ${\displaystyle x(t), \ y(t), \ z(t)}$ - гладкие функции.
Элемент дуги ${\displaystyle ds}$ на малом участке кривой выражается как:
$$\displaylines{
ds = \sqrt{ \left( \frac{dx}{dt}  \right)^{ 2 }+ \left( \frac{dy}{dt}  \right)^{ 2 } + \left( \frac{dz}{dt} \right)^{ 2 } }dt
}$$
Векторное представление дифференциала дуги:
$$\displaylines{
ds = \left| \frac{dr}{dt} \right| dt, \  
}$$
где ${\displaystyle \dfrac{dr}{dt}}$ - это вектор касательной скорости к кривой.

Длинна дуги кривой ${\displaystyle r}$ от точки ${\displaystyle t = a}$ до точки ${\displaystyle t = b}$ вычисляется как интеграл от дифференциала дуги:
$$\displaylines{
S = \int_{a}^{b}  \, ds = \int_{a}^{b}  \sqrt{ \left( \frac{dx}{dt}  \right)^{ 2 }+ \left( \frac{dy}{dt}  \right)^{ 2 } + \left( \frac{dz}{dt} \right)^{ 2 } }dt  
}$$
Длинна хорды между двумя точками на кривой ${\displaystyle t_{ 1 }, \ t_{ 2 }}$ равна:
$$\displaylines{
L = |r(t_{ 2 })-r(t_{ 1 })|
}$$

Доказательство эквивалентности длины дуги, длины хорды и дифференциала дуги.
Рассмотрим малый участок кривой между ${\displaystyle t, \ t+\Delta t}$. Для такого участка:
- Длинна хорды приближенно равна:
$$\displaylines{
L  = |r(t+\Delta t)-r(t)| \approx \left| r(t)+ \frac{dr}{dt}\Delta t - r(t) \right| \approx \left| \frac{dr}{dt} \right| \Delta t
}$$
Где разложение ${\displaystyle r(t+\Delta t)}$ в ряд Тейлора по ${\displaystyle \Delta t}$ до линейного члена дает данное приближение.

- Длинна хорды между этими точками:
$$\displaylines{
\Delta s = \int_{t}^{t + \Delta t} \sqrt{ \left( \frac{dx}{dt}  \right)^{ 2 }+ \left( \frac{dy}{dt}  \right)^{ 2 } + \left( \frac{dz}{dt} \right)^{ 2 } }dt  \approx \sqrt{ \left( \frac{dx}{dt}  \right)^{ 2 }+ \left( \frac{dy}{dt}  \right)^{ 2 } + \left( \frac{dz}{dt} \right)^{ 2 } }\Delta t 
}$$
Когда ${\displaystyle \Delta t \to 0}$, разница между длинной дуги и длинной хорды стремится к нулю:
$$\displaylines{
\Delta s - L \to  0
}$$
Следовательно, при ${\displaystyle \Delta t \to 0}$ длинна дуги, длинна хорды и дифференциала дуги становятся эквивалентными  