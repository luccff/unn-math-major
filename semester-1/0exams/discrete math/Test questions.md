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
1. Дан универс ${\displaystyle U = \{ 1, \ 2, \ 3, \  \dots, \ n \}}$. Охарактеризовать бинарное отношение бинарное отношение на ${\displaystyle 2^{ U }}$ между произвольными множествами ${\displaystyle A}$ и ${\displaystyle B}$, ${\displaystyle A R B}$, если ${\displaystyle A\overline{B} = \varnothing}$.
$$\displaylines{
ARB \iff A \cap \overline{B} = \varnothing \iff A \subseteq B.
}$$
Свойства отношения:
1. Рефлексивность: ${\displaystyle \forall{A:} A \subseteq A \implies ARA}$.
2. Антисимметричность: ${\displaystyle \forall{A, \ B}: A \subseteq B \wedge B \subseteq A \implies A = B}$.
3. Транзитивность: ${\displaystyle \forall{A, \ B, \ C}: A \subseteq B \wedge B \subseteq C \implies A \subseteq C}$.
Отношение является частичным порядком.

1. Дано множество ${\displaystyle A}$ и в нем подмножества ${\displaystyle B, \ C}$, причем ${\displaystyle |A -B \cap C| = 8}$, ${\displaystyle |B| = 5, \ |C-B| = 1, \  |B \cap C| = 3}$. Сколько имеется таких подмножеств ${\displaystyle X \subseteq A}$, что ${\displaystyle |X-(B \cup C)| = 2, \  |X \cap (B-C)| = 2}$?

$$\displaylines{
C = (C-B) \cup (B \cap C) \implies |C| = 1 + 3 = 4 \\
B = (B - C) \cup  (B \cap C) \implies |B - C| = 5 - 3 = 2 \\
|A| = |A - BC| + |BC| = 8 + 3 = 11 \\
|B \cup C| = |B| + |C| - |B \cap C| = 5 + 4 - 3 = 6 \\
|A - (B \cup C)| = |A| - |B \cup C| = 11 - 6 = 5. \\
\\
X - (B \cup  C) = X \cap  (A - (B \cup C)) \implies \binom{5}{2} = 10 \\
|B - C| = 2 \implies \binom{2}{2} = 1 \\
|B \cap C| = 3, \  |C-B| = 1 \implies \text{ ост. элементов } 4 \\
\implies 10 \cdot  1 \cdot  2^{ 4 } = 160.
}$$

2. Дано множество ${\displaystyle A}$ и в нем подмножества ${\displaystyle B, \ C}$, причем ${\displaystyle |B| = 5, \ |C| = 3, \  |B \cup C | = 7, \  |A-B| = 7.}$ Сколько имеется таких подмножеств ${\displaystyle X \subseteq A }$, что ${\displaystyle X \cap(C-B) = \varnothing}$, ${\displaystyle |X \cap B|\geq 4}$, ${\displaystyle |X-(B \cup C)| = 2}$?

3. Сколько четырех элементных подмножеств в множестве ${\displaystyle 2^{ \{ a, \ b, \ c, \ d \} } \otimes 2^{ \{ c, \ d, \ e \} }}$?
$$\displaylines{
|A| = 2^{ 4 } = 16, \  |B| = 2^{ 3 } = 8 \\
|A \otimes B| = |A| + |B| - 2|A \cap  B| = 16 - 8 - 2 \cdot 2 ^{ 2 } = 16 \\
\binom{16}{4} = 1820.
}$$

