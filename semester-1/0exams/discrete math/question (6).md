##### Отношения между множествами. Бинарные отношения. Способы задания бинарных отношений. Примеры. Операции над отношениями. Обратное отношение.
---
Бинарным отношением между множествами ${\displaystyle A}$ и ${\displaystyle B}$ называется любое подмножество ${\displaystyle R}$ прямого произведения ${\displaystyle A\times B}$. Если ${\displaystyle R}$ - отношение и ${\displaystyle (x, \ y) \in R}$, то говорят, что элемент ${\displaystyle x}$ находится в отношении ${\displaystyle R}$ с элементом ${\displaystyle y}$. Запись - ${\displaystyle xRy}$. В случае, когда ${\displaystyle A = B}$, мы говорим просто об отношении ${\displaystyle R}$ на ${\displaystyle A}$.
Элементы множества ${\displaystyle A\times B}$ - упорядоченные пары, поэтому из того, что ${\displaystyle xRy \cancel{\implies} yRx}$.
Пример: ${\displaystyle 2 < 5 \cancel{ \implies} 5 < 2}$.
$$\displaylines{
R \subseteq A_{ 1 } \times \dots \times A_{ n } - \text{ n-мерное отношение между множествами } A_{ 1 }, \dots, A_{ n } \\ 
}$$

Пример:
$$\displaylines{
A \text{ - люди} \\ 
B \text{ - страны} \\ 
R \subseteq A \times B \\ 
xRy \iff  x\text{ бывал в } y
}$$

Способы задания бинарных отношений: 
$$\displaylines{
\text{A, B – конечные} \\ 
R \subseteq A \times B
}$$
1. Перечисление: ${\displaystyle R = \{ (x_{ 1 }, y_{ 1 }), (x_{ 3 }, y_{ 7 }), \dots \} \\ }$
2. Таблица ${\displaystyle A = \{ a_{ 1 }, \dots, a_{ n } \} ; B = \{ b_{ 1 }, \dots, b_{ m } \} }$
$$\displaylines{
\begin{cases}
1, \   &  a_{ i }Rb_{ j } \\
0, \   &  a_{ i }\cancel{R}b_{ j }
\end{cases}
}$$
Отношение делимости

|     |  1  |  2  |  3  |  4  |
| :-: | :-: | :-: | :-: | :-: |
|  1  |  1  |  1  |  1  |  1  |
|  2  |  0  |  1  |  0  |  1  |
|  3  |  0  |  0  |  1  |  0  |
|  4  |  0  |  0  |  0  |  1  |

3. Граф отношений. Это диаграмма, которая строится следующим образом. Пусть ${\displaystyle R}$ - отношение на множестве ${\displaystyle A}$. Элементы множества ${\displaystyle A}$ изобразим кружками, эти кружки называют вершинами графа. Если ${\displaystyle xRy}$, то рисуем стрелку от ${\displaystyle x}$ к ${\displaystyle y}$.
![[Pasted image 20250123160723.png]]

Операции над отношениями: так как отношение есть множество пар, то любые операции над множествами можно применять к отношениям. Если ${\displaystyle R_{ 1 }, \ R_{ 2 }}$ - отношения, то ${\displaystyle R_{ 1 } \cup R_{ 2 }, \ R_{ 1 } \cap R_{ 2 }}$ и т.д. - тоже отношения на ${\displaystyle A}$. Если ${\displaystyle R}$ - отношение на ${\displaystyle A}$, то ${\displaystyle \overline{R}}$ - дополнение отношения ${\displaystyle R}$ на ${\displaystyle A}$.
Обратное отношение ${\displaystyle R^{ -1 }}$ к отношению ${\displaystyle R}$: ${\displaystyle R^{ -1 } = \{ (x, \ y): (y, \ x) \in R \}}$.
![[Pasted image 20250123161240.png]]
