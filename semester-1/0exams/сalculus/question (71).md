### Угол смежности дуги. Средняя кривизна кривой. Кривизна кривой в точке, определение, геометрический смысл. Радиус кривизны. Вычисление кривизны. Геометрический смысл второй производной. Центр и круг кривизны. Эволюта и эвольвента.
---
**Угол смежности** дуги - это угол, который образует касательная к кривой в точке с направлением, связывающим начальную и конечную точки дуги (хорду)ю

Для кривой, заданной параметрически, угол смежности определяется как угол между вектором касательной и вектором хорды.
$$\displaylines{
\cos{(\varphi)} =\frac{T \cdot C}{|T| |C|}  = \frac{\cfrac{dr}{ds} \cdot  (r(t_{ 2 })-r(t_{ 1 }))}{\left| \cfrac{dr}{ds} \right| \cdot  \left|  (r(t_{ 2 })-r(t_{ 1 })) \right|  } 
}$$
При ${\displaystyle t_{ 2 } \to t_{ 1 }}$ угол ${\displaystyle \varphi}$ стремится к нулю, так как хорда совпадает с направлением касательной.

**Средняя кривизна** на дуге ${\displaystyle \Gamma}$, заданной между точками ${\displaystyle t_{ 1 }, \ t_{ 2 }}$ определяется как:
$$\displaylines{
\overline{k} = \frac{\Delta \varphi}{\Delta S}, \   
}$$
где ${\displaystyle \Delta \varphi}$ изменение угла наклона касательной к кривой на дуге, ${\displaystyle \Delta S}$ длина дуги.
Средняя кривизна измеряет среднее изменение направления касательной на единицу длины дуги.

**Кривизна кривой в точке** - это предел средней кривизны при ${\displaystyle \Delta S \to 0}$:
$$\displaylines{
k = \lim_{ \Delta S \to 0} {\frac{\Delta \varphi}{\Delta s}}
}$$
Формула кривизны: для плоской кривой ${\displaystyle y = f(x)}$ кривизна в точке выражается через первую и вторую производные:
$$\displaylines{
k = \frac{|f''(x)|}{\bigg(1+\big(f'(x)\big)^{ 2 }\bigg)^{ 2/3 }} 
}$$
Для параметрически заданной кривой ${\displaystyle r(t) = (x(t), \ y(t), \ z(t))}$:
$$\displaylines{
k = \frac{|r'(t) \times r''(t)}{|r'(t)|^{ 3 }} 
}$$
Кривизна характеризует "изгиб" кривой в данной точке. Чем больше ${\displaystyle k}$, тем сильнее кривая отклоняется от прямой.

Вторая производная характеризует скорость изменения первой производной, то есть скорость изменения наклона касательной. В геометрическом плане вторая производная связана с кривизной. Чем больше ${\displaystyle f''(x)}$, тем больше изгиб кривой в данной точке.

**Радиус кривизны** - это величина, обратная кривизне:
$$\displaylines{
R = \frac{1}{k}
}$$
Он описывает радиус окружности, которая наиболее точно приближает кривую в данной точке (окружность называется **кругом кривизны**). Чем больше радиус кривизны, тем меньше кривизна, чем меньше радиус кривизны, тем больше кривизна.


**Центр кривизны** — это центр окружности, которая наиболее точно приближает кривую в данной точке.

**Круг кривизны** — это окружность с радиусом ${\displaystyle R}$, центром в точке ${\displaystyle O}$, расположенной на нормали к кривой.

**Эволюта** кривой ${\displaystyle \Gamma}$ - это геометрическое место центров кривизны данной кривой. Это кривая, вдоль которой перемещается центр круга кривизны.
Формула для эволюты плоской кривой ${\displaystyle y = f(x)}$:
$$\displaylines{
x_{ э } = x - R\cos{(\varphi)}, \  \quad    y_{ э } = y - R\sin{(\varphi)}
}$$
**Эвольвента** кривой ${\displaystyle \Gamma}$ это кривая, которая получается при разматывании невесомой нити, намотанной на ${\displaystyle \Gamma}$.


