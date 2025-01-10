### Приложение. Полярные координаты. Формулы перехода от декартовых координат к полярным в случае согласования декартовой и полярной систем координат. Построение простейших графиков в полярных координатах (по таблице значений).
---
Полярная система координат- точка определяется полярным углом и полярным радиусом ${\displaystyle (|\vec{r}|, \ \varphi)}$
$$\displaylines{
\begin{cases}
r = \sqrt{ x^{ 2 }+y^{ 2 } }  \\
\varphi = \arctan{\left( \dfrac{y}{x} \right)}
\end{cases}
}$$
Пример 1. ${r = 1}$  окружность с радиусом ${r = 1}$
$$\displaylines{

\begin{array}{c|c|c|c|c|c|c|c|c}

\varphi & 0 & \dfrac{\pi}{4} & \dfrac{\pi}{2} & \pi & \dfrac{3\pi}{2} & 2\pi \cr

\hline

r & 1 & 1 & 1 & 1 & 1 & 1

\end{array}

}$$
Переход из Д.С.К в П.С.К:

$$\displaylines{
x^{ 2 } + y^{ 2 } = 1 \hookrightarrow (r\cos{(\varphi)})^{ 2 }+(r\sin{(\varphi)})^{ 2 }=1 \to r^{ 2 }\cos{(\varphi)}^{ 2 }+r^{ 2 }\sin{(\varphi)}^{ 2 }\\r^{ 2 }(\cos{(\varphi)}^{ 2 }+\sin{(\varphi)}^{ 2 })\\r^{ 2 } = 1 \to \boxed{r = 1}
}$$
![[Pasted image 20250110045337.png | 400]]

Пример 2. ${r(\varphi) = \sin{(2\varphi)}}$
$$\displaylines{
\begin{array}{c|c|c|c|c|c|c|c|c}
\varphi & 0 & \dfrac{\pi}{4} & \dfrac{\pi}{2} & \left( \dfrac{\pi}{2};\pi \right)&\pi&\dfrac{5\pi}{4} & \dfrac{3\pi}{2} & \left( \dfrac{3\pi}{2};2\pi \right)\\
\hline
r & 0 & 1 & 0 &r<0& 0 & 1 & 0 & r<0
\end{array}

}$$
Более строго: ${\sin{(2\varphi)}}$ имеет период ${\pi}$.
$$\displaylines{
\text{При } \varphi \in \left[ 0; \dfrac{\pi}{4} \right] \sin{(2\varphi) \uparrow} \text{ от 0 до 1} \\
\text{При } \varphi \in \left[ \dfrac{\pi}{4}; \dfrac{\pi}{2} \right] \sin{(2\varphi)}\downarrow \text{ от ${1}$ до ${0}$}\\
\text{При } \varphi \in \left[ \dfrac{\pi}{2};\pi \right] \sin{(2\varphi)}<0; r<0 \\
\text{При } \varphi \in [\pi;2\pi]\text{продолжим периодически}
}$$
![[Pasted image 20250110045500.png|400]]
