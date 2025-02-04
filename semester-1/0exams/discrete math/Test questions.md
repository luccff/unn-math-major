1. Сколько слов длины $n$ можно составить из алфавита мощности семь, таких, чтобы буква $а_{ 1 }$ повторялась ровно пять раз?
Пусть есть алфавит ${\displaystyle \{ a_{1}, \ a_{2}, \ a_{3}, \ a_{4}, \ a_{5}, \ a_{ 6 }, \ a_{ 7 } \}}$. 
Мы должны выбрать 5 позиций из ${\displaystyle n}$ для буквы ${\displaystyle a_{ 1 }}$. Количество способов это: ${\displaystyle \binom{n}{5}}$. В оставшихся ${\displaystyle n-5}$ позициях могут стоять любые буквы из оставшихся 6 букв. Каждую из оставшихся можно заполнить одной из 6 букв: ${\displaystyle 6^{ n-5 }}$. Следовательно общее количество таких слов равно ${\displaystyle \binom{n}{5} \cdot 6^{ n-5 }}$.
2. Сколько 5-элементных подмножеств в множестве ${\displaystyle 2^{ \{ a, \ b, \ c, \ d \} } - 2^{ \{ d, \ e \} }}$?
$$\displaylines{
2^{ 4 } - 2 = 14 \\
\binom{12}{5} = 2002
}$$
3. Описать свойства отношения $R \in \mathbb{N} \times \mathbb{N}$$: xRy \iff x \leq y \cdot y$.
$$\displaylines{
\textbf{ Рефлексивность: } \forall{x \in  \mathbb{N} }: \ xRx \ (x\leq x\cdot x) - \text{ верно } \forall{x\geq 0}.\\
\textbf{ Антисимметричность: } \ \forall{x, \  y \in  \mathbb{N} : } \  x\neq y \implies \begin{cases} x\cancel{R}y \\ \text{ или } \\ y \cancel{R} x \end{cases} \\
\text{ Пример: } x = 4, \  y = 2 \implies \begin{cases}
4\leq 4  \\
2\leq 16
\end{cases} - \text{  не антисимметрично. } \\
\textbf{ Транзитивность: } \forall{x, \  y, \  z \in  \mathbb{N} }: \begin{cases}
xRy \\
yRz
\end{cases} \implies xRz \\
\text{ Пример: } x = 5, \  y = 3, \  z = 2: \begin{cases}
5\leq 9\\
3 \leq 4
\end{cases} \ \cancel{\implies} 5 \leq 4 - \text{ не транзитивно. } \\
\textbf{ Симметричность: } \forall{x, \  y \in  \mathbb{N} }: xRy \implies yRx \\ 
\text{ Пример: } x = 1, \   y = 2: 1 \leq 4 \cancel{\implies } 2 \leq 1 - \text{ не симметрично. }
}$$