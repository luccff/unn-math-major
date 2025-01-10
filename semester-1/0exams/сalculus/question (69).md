### Дифференциал дуги. Длина дуги как параметр.
---
Рассмотрим гладкую кривую ${\displaystyle \Gamma}$ в пространстве заданную параметрически, где ${\displaystyle r(t)}$ её векторное представление:
$$\displaylines{
r(t) = (x(t), \  y(t), \  z(t)), \  t \in  [a, \  b]
}$$
где ${\displaystyle x(t), \ y(t), \ z(t)}$ - гладкие функции.
Для малой длинный дуги ${\displaystyle \Delta s}$ соответствующей малому изменению параметра ${\displaystyle \Delta t}$, длинна дуги может быть приближена длинной векторе ${\displaystyle \Delta r}$:
$$\displaylines{
\Delta s \approx |\Delta r| = \sqrt{ (\Delta x)^{ 2 }+(\Delta y)^{ 2 }+(\Delta z)^{ 2 } }
}$$
При устремлении ${\displaystyle \Delta t \to 0}$ получаем дифференциал дуги:
$$\displaylines{
ds = \sqrt{ \left( \frac{dx}{dt}  \right)^{ 2 }+ \left( \frac{dy}{dt}  \right)^{ 2 } + \left( \frac{dz}{dt} \right)^{ 2 } }dt
}$$
Векторное представление дифференциала дуги:
$$\displaylines{
ds = \left| \frac{dr}{dt} \right| dt, \  
}$$
где ${\displaystyle \dfrac{dr}{dt}}$ - это вектор касательной скорости к кривой.
Для плоской кривой ${\displaystyle z(t) = 0}$:
$$\displaylines{
ds = \sqrt{ \left( \frac{dx}{dt}  \right)^{ 2 }+ \left( \frac{dy}{dt}  \right)^{ 2 }  }dt
}$$
Длинна дуги кривой ${\displaystyle r}$ от точки ${\displaystyle t = a}$ до точки ${\displaystyle t = b}$ вычисляется как интеграл от дифференциала дуги:
$$\displaylines{
S = \int_{a}^{b}  \, ds = \int_{a}^{b}  \sqrt{ \left( \frac{dx}{dt}  \right)^{ 2 }+ \left( \frac{dy}{dt}  \right)^{ 2 } + \left( \frac{dz}{dt} \right)^{ 2 } }dt  
}$$
Для плоской кривой:
$$\displaylines{
\int_{a}^{b}  \sqrt{ \left( \frac{dx}{dt}  \right)^{ 2 }+ \left( \frac{dy}{dt}  \right)^{ 2 } }dt  
}$$

Длинна дуги как параметр. Если использовать длину дуги ${\displaystyle s}$ в качестве параметра для кривой, то параметризация кривой упрощается. Пусть ${\displaystyle s}$ - длинна дуги, измеряемая от некоторой начальной точки кривой ${\displaystyle t_{ 0 }}$. Тогда:
$$\displaylines{
s(t) = \int_{t_{ 0 }}^{t} \left| \frac{dr}{dt} \right|  \, dt 
}$$
Функция ${\displaystyle s(t)}$ монотонно возрастает, и её можно обратить: ${\displaystyle t = t(s)}$. Таким образом кривая переписывается как:
$$\displaylines{
r(s) = (x(s), \  y(s), \  z(s))
}$$
Важное свойство:
$$\displaylines{
\left| \frac{dr}{ds} \right|  = 1
}$$
Это означает, что ${\displaystyle s}$ - естественный параметр кривой.
Вторая производная ${\displaystyle \frac{d^{ 2 }r}{ds^{ 2 }}}$ называется вектором кривизны.
