#### Вывод формулы для векторного произведения в ортонормированном базисе.
---
Координаты векторного произведения в ортонормированном базисе. Базис ортонормирован, если ${\displaystyle (e_{ i }, \ e_{ j }) = \begin{cases} 1, \  i = j \\ 0, \  i \neq j\end{cases}}$
$$\displaylines{
\text{ В базисе } \vec{i}, \ \vec{j}, \ \vec{k}: \ \vec{a} = (a_{ 1 }, \ a_{ 2 }, \ a_{ 3 }), \ \vec{b} = (b_{ 1 }, \ b_{ 2 }, \ b_{ 3 }) \implies \\
\implies \vec{a}\times \vec{b} = \begin{vmatrix}
\vec{i} & \vec{j} & \vec{k} \\
a_{ 1 } & a_{ 2 } & a_{ 3 } \\
b_{ 1 } & b_{ 2 } & b_{ 3 }
\end{vmatrix} = \begin{vmatrix}
a_{ 2 } & a_{ 3 } \\
b_{ 2 } & b_{ 3 }
\end{vmatrix} \cdot \vec{i} - \begin{vmatrix}
a_{ 1 } & a_{ 3 } \\
b_{ 1 } & b_{ 3 }
\end{vmatrix}\cdot \vec{j} + \begin{vmatrix}
a_{ 1 } & a_{ 2 } \\
b_{ 1 } & b_{ 2 }
\end{vmatrix} \cdot \vec{k} = \\ = (a_{ 2 }b_{ 3 }-a_{ 3 }b_{ 2 }, \ a_{ 3 }b_{ 1 }-a_{ 1 }b_{ 3 }, \ a_{ 1 }b_{ 2 }-a_{ 2 }b_{ 1 })
}$$
Доказательство:
$$\displaylines{
\begin{array}{c|c|c}
 & \vec{i} & \vec{j} & \vec{k} \\
\hline 
\vec{i} & \vec{0} & \vec{k} & -\vec{j} \\
\hline 
\vec{j} & -\vec{k} & \vec{0} & \vec{i} \\
\hline 
\vec{k} & \vec{j} & -\vec{i} & \vec{0}
\end{array} \quad  \begin{matrix}
\vec{a}\times \vec{b} = (a_{ 1 }\vec{i}+a_{ 2 }\vec{j}+a_{ 3 }\vec{k}) \times (b_{ 1 }\vec{i}+b_{ 2 }\vec{j}+b_{ 3 }\vec{k}) = \\ = a_{ 1 }b_{ 2 }\vec{k} - a_{ 1 }b_{ 3 }\vec{j} - a_{ 2 }b_{ 1 }\vec{k} + a_{ 2 }b_{ 3 }\vec{i} + a_{ 3 }b_{ 1 }\vec{j} - a_{ 3 }b_{ 2 }\vec{i} = \\ =(a_{ 2 }b_{ 3 }-a_{ 3 }b_{ 2 }, \ a_{ 3 }b_{ 1 }-a_{ 1 }b_{ 3 }, \ a_{ 1 }b_{ 2 }-a_{ 2 }b_{ 1 })
\end{matrix}
}$$
