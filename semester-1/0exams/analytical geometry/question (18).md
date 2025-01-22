#### Определение смешанного произведения. Доказательство линейности смешанного произведения. Выражение смешенного произведения через объем параллелепипеда. 
---
Смешанным произведением ${\displaystyle \vec{a}, \ \vec{b}, \ \vec{c}}$ называется число, равное скалярному произведению ${\displaystyle \vec{a}}$ на векторное произведение ${\displaystyle \vec{b}}$ и ${\displaystyle \vec{c}}$.
$$\displaylines{
(\vec{a}, \  [\vec{b}, \  \vec{c}])
}$$
1. Линейность смешанного произведения: ${\displaystyle (\vec{a}+\vec{b}, \vec{c}, \vec{d}) = (\vec{a}, \vec{c}, \vec{d}) + (\vec{b}, \vec{c}, \vec{d})}$.
Доказательство:
$$\displaylines{ (\vec{a}+\vec{b}, \vec{c}, \vec{d}) = ((\vec{a}+\vec{b})\times \vec{c})\cdot \vec{d} = (\vec{a}\times \vec{c} + \vec{b}\times \vec{c})\cdot \vec{d} = (\vec{a}\times \vec{c})\cdot \vec{d} + (\vec{b} \times \vec{c})\cdot \vec{d} = (\vec{a}, \vec{c}, \vec{d}) + (\vec{b}, \vec{c}, \vec{d}) }$$
2. ${\displaystyle (\lambda \vec{a}, \vec{b}, \vec{c}) = \lambda(\vec{a}, \vec{b}, \vec{c})}$
Доказательство: 
$$\displaylines{ (\lambda\vec{a}, \vec{b}, \vec{c}) = (\lambda\vec{a}) \cdot (\vec{b}\times \vec{c}) = \lambda(\vec{a}\cdot (\vec{b}\times \vec{c})) = \lambda(\vec{a}, \vec{b}, \vec{c}) }$$
3. Выражение через объем параллелепипеда
![[Pasted image 20250119183045.png | 500]]
${\displaystyle V}$ - объем параллелепипеда, построенного на ${\displaystyle \vec{a}, \ \vec{b}, \ \vec{c}}$.
$$\displaylines{
\vec{a}, \  \vec{b}, \  \vec{c} = \begin{cases}
V, \ & \vec{a}, \  \vec{b}, \  \vec{c} - \text{ правая }\\ 
-V, \ & \vec{a}, \  \vec{b}, \  \vec{c} - \text{ левая }
\end{cases}
}$$
