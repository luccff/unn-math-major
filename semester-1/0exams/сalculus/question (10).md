### Последовательность ${ \left\{  \left( 1 + \frac{1}{n} \right) ^{ n }  \right\}}$. Доказать монотонность и ограниченность. Определение числа ${\displaystyle e}$
---
Рассмотрим последовательность ${\displaystyle a_{n} = \left( 1+\frac{1}{n} \right)^{ n }}$. Докажем монотонность и ограниченность.
Доказательство монотонности: рассмотрим отношение последовательных членов
$$\displaylines{
\frac{a_{n+1}}{a_{n}} = \frac{\left( 1+\cfrac{1}{n+1} \right)^{ n+1 }}{\left( 1+\cfrac{1}{n} \right)^{ n }} \\
}$$
Воспользуемся ${\displaystyle a = \ln(\exp(a))}$:
$$\displaylines{
\ln\left( \frac{a_{n+1}}{a_{n}} \right)  = (n+1)\ln\left( 1+ \frac{1}{n+1} \right) - n\ln\left( 1+ \frac{1}{n} \right)
}$$
Воспользуемся разложением ${\displaystyle \ln(1+x) \approx x- \frac{x^{ 2 }}{2}}$
$$\displaylines{
1) \ \ln\left( 1 + \frac{1}{n+1} \right) \approx \frac{1}{n+1} - \frac{1}{2(n+1)^{ 2 }} \\
2) \ln\left( 1+ \frac{1}{n} \right) \approx \frac{1}{n} - \frac{1}{2n^{ 2 }}
}$$
Тогда
$$\displaylines{
\ln\left( \frac{a_{n+1}}{a_{n}}  \right) \approx (n+1) \cdot \left( \frac{1}{n+1} - \frac{1}{2(n+1)^{ 2 }} \right) - n \left( \frac{1}{n} - \frac{1}{2n^{ 2 }} \right)
}$$
Упрощая, получаем
$$\displaylines{
\ln\left( \frac{a_{n+1}}{a_{n}}  \right) \approx  \frac{1}{2n} - \frac{1}{2n+2}
}$$
Можно заметить, что 
$$\displaylines{
\frac{1}{2n} > \frac{1}{2n+2}
}$$
Значит 
$$\displaylines{
\ln\left( \frac{a_{n+1}}{a_{n}}  \right) > 0 \implies  \frac{a_{n+1}}{a_{n}} > 1 \implies  a_{n+1}>a_{n} 
}$$
Доказательство ограниченности:
По биномиальной теореме
$$\displaylines{
\left( 1+\frac{1}{n} \right)^{ n } = 1 + \binom{n}{1} \frac{1}{n} + \binom{n}{2} \frac{1}{n^{ 2 }} + \dots +\binom{n}{n} \frac{1}{n^{ n }}
}$$
Разложим по биному Ньютона:
$$\displaylines{
\left( 1+\frac{1}{n} \right)^{ n } < 1 + 1 + \frac{1}{2!} + \frac{1}{3!} + \dots \frac{1}{n!~}
}$$
Для оценки остатка, воспользуемся суммой убывающей геометрической прогрессии, так как все члены, начиная с ${\displaystyle  \frac{1}{n!}}$ уменьшаются быстрее:
$$\displaylines{
S = \frac{a_{ 1 }}{1-q}, \ \text{ где } a_{ 1 } = \frac{1}{2}, \  q = \frac{1}{2} \\
S = \frac{\cfrac{1}{2}}{1- \cfrac{1}{2}} = 1
}$$
Таким образом 
$$\displaylines{
\left( 1+\frac{1}{n} \right)^{ n } < 1+ 1+ 1 = 3
}$$
Ограниченность доказана.

Так как последовательность ${\displaystyle a_{n}}$ монотонно возрастает и ограничена сверху, следовательно она имеет предел. Обозначим его за ${\displaystyle e}$
$$\displaylines{
e = \lim_{ n \to \infty } {\left( 1+\frac{1}{n} \right)^{ n }}
}$$
Очевидно, что ${\displaystyle 2<e<3}$. Приближенное значение ${\displaystyle  e \approx 2,718281828459045}$
