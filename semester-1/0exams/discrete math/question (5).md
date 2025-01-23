##### Уравнения и системы уравнений в алгебре множеств. Алгоритм нахождения решений. Необходимые и достаточные условия существования решения. Число решений.
---
Система уравнений в алгебре множеств - совокупность нескольких уравнений, объединенных условием одновременного выполнения. Уравнения в алгебре множеств - теоретико-множественное отношение над множествами, среди которых есть неизвестное множество ${\displaystyle X}$.

Алгоритм решения уравнения:
1. ${\displaystyle A \subseteq B \iff A\overline{B} = \emptyset}$
2. ${\displaystyle A = B \iff A \otimes B = \emptyset}$

Рассмотрим уравнение ${\displaystyle \varphi(A_{ 1 }, \ \dots, \ A_{ k }, \ X) = \psi(A_{ 1 }, \ \dots, \ A_{ k }, \ X)}$. В нем ${\displaystyle A_{ 1 }, \ \dots, \ A_{ k } \subseteq U, \ X}$ - неизвестное множество, ${\displaystyle \varphi, \ \psi}$ - формулы, содержащие теоретико-множественные операции. ${\displaystyle X_{ 0 }}$ - частное решение уравнения, если при подстановке ${\displaystyle \varphi, \ \psi}$ задают одно и то же множество.

Применим лемму 2 к уравнению:
$$\displaylines{
\varphi(A_{ 1 }, \  \dots , \  A_{ k }, \  X) \otimes \psi(A_{ 1 }, \  \dots , \  A_{ k }, \  X) = \emptyset
}$$
Применим основные тождества и приведем к такому виду:
$$\displaylines{
F_{ 1 }X \cup F_{ 2 }\overline{X} \cup  F_{ 3 } = \emptyset
}$$
${\displaystyle F_{ 1 }, \ F_{ 2 }, \ F_{ 3 }}$ - множества, не содержащие ${\displaystyle X}$, зависящие от ${\displaystyle A_{ 1 }, \ \dots, \ A_{ k }}$.
Чтобы такое уравнение было равно пустому множеству, необходимо, чтобы каждое множество было равно ${\displaystyle \emptyset}$:
$$\displaylines{
\begin{cases}
F_{ 1 }X = \emptyset \\
F_{ 2 }\overline{X} = \emptyset \\
F_{ 3 } = \emptyset
\end{cases} \iff \begin{cases}
X \subseteq \overline{F_{ 1 }} \\
F_{ 2 } \subseteq X \\
F_{ 3 } = \emptyset
\end{cases} \implies \begin{cases}
F_{ 2 } \subseteq \overline{F_{ 1 }} \\
F_{ 3 } = \emptyset
\end{cases} \implies \begin{cases}
 F_{ 2 }F_{ 1 } = \emptyset  \\
F_{ 3 } = \emptyset
\end{cases}
}$$
${\displaystyle F_{ 2 }F_{ 1 } \cup F_{ 3 } = \emptyset}$ - необходимым и достаточным условием существования уравнения.

Различное число решений будет получаться, если к наименьшему числу решений ${\displaystyle X_{ 0 } = F_{ 2 }}$ добавлять любые подмножества разности ${\displaystyle \overline{F_{ 1 }} - F_{ 2 } = \overline{F_{ 1 }} \  \overline{F_{ 2 }}}$. Всего таких подмножеств ${\displaystyle 2^{ |\overline{F_{ 1 }} \ \overline{F_{ 2 }} |}}$ - число различных решений уравнения.

Число решений - всевозможные множества, при подстановке которых уравнение превращается в верное тождество.
