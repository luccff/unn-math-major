##### Корни n-ой степени из комплексного числа. Корни из единицы. Группа корней n-ой степени из 1. Первообразные корни n-ой степени из 1.
---
### Корни ${\displaystyle n}$-ой степени из комплексного числа
Корни ${\displaystyle n}$-ой степени из числа ${\displaystyle z = r(\cos{(\varphi)}+i\sin{(\varphi)})}$ это решение уравнения ${\displaystyle w^{ n } = z}$. Каждое такое решение ${\displaystyle w_{ k }}$ записывается в виде:
$$\displaylines{
w_{ k } = \sqrt[n]{ r } \cdot  \left( \cos{\left( \frac{\varphi + 2\pi k}{n}  \right) + i \sin{\left( \frac{\varphi + 2\pi k}{n}  \right)}} \right), \  \quad  k = 0, \  1, \  2, \  \dots , \   n-1
}$$
### Корни из единицы
$$\displaylines{
w^{ n } = 1 \\
1 = \cos{(0)} + i\sin{(0)} \\
w_{ k } = \cos{\left( \frac{2\pi k}{n} \right)} + i \sin{\left( \frac{2\pi k}{n} \right)}, \   \quad k = 0, \  1, \  2\dots , \  n-1
}$$
### Группа корней ${\displaystyle n}$-ой степени из 1
$$\displaylines{
W = \{ w_{ 0 }, \  w_{ 1 }, \   w_{ 2 }, \ \dots \ , \   w_{ n-1 } \}, \  
}$$
где ${\displaystyle w_{ k } = \cos{\left( \frac{2\pi k}{n} \right)} + i \sin{\left( \frac{2\pi k}{n} \right)}}$ образует группу относительно умножения.
Свойства: 
1. замкнутость (произведение двух корней ${\displaystyle w_{ k }}$ и ${\displaystyle w_{ j }}$ также является корнем ${\displaystyle n}$-ой степени из 1)
2. ассоциативность (следует из свойств умножения комплексных чисел.)
3. существует нейтральный элемент (${\displaystyle w_{ 0 } = 1}$)
4. обратимость (для ${\displaystyle w_{ k }}$ это ${\displaystyle w_{ n-k }}$).

### Первообразные корни ${\displaystyle n}$-ой степени из 1
Первообразный корень ${\displaystyle n}$-ой степени из 1 - это такой корень ${\displaystyle \zeta = w_{ k }}$, для которого его степени ${\displaystyle \zeta^{ 1 }, \  \zeta ^{ 2 }, \ \dots, \ \zeta^{ n }}$ дают все ${\displaystyle n}$ различных корней ${\displaystyle n}$-ой степени из 1.
Этот корень является первообразным тогда и только тогда, когда наибольший общий делитель ${\displaystyle k}$ и ${\displaystyle n}$ равен ${\displaystyle 1}$. 
Формально: ${\displaystyle \zeta^{ k } \neq 1}$ для ${\displaystyle 1 \leq k < n}$, но ${\displaystyle \zeta ^{ n } = 1}$.

Доказательство: пусть ${\displaystyle \zeta^{ m } = 1}$ для ${\displaystyle 1\leq m<n}$. Тогда ${\displaystyle m}$ должно делить ${\displaystyle n}$, чтобы ${\displaystyle \frac{2\pi k m}{n}}$ соответствовало полному обороту ${\displaystyle 2\pi l, \  l \in \mathbb{Z}}$. Если ${\displaystyle НОД(k, \ n) = 1}$, то ${\displaystyle \zeta^{ m } \neq 1}$ так как ${\displaystyle k}$ не делится на ${\displaystyle \frac{n}{m}}$. Следовательно все степени ${\displaystyle \zeta^{ k }}$ дают различные ${\displaystyle n}$ корней, а ${\displaystyle \zeta = 1.}$
