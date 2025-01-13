##### Правило Крамера.
---
### Правило Крамера
**Правило Крамера** — это метод нахождения решения системы линейных уравнений вида:
$$
A \vec{x} = \vec{b},
$$
где:
- $A$ — квадратная матрица порядка $n$ с ненулевым определителем $\det(A) \neq 0$,
- $\vec{x} = (x_1, x_2, \dots, x_n)^T$ — вектор неизвестных,
- $\vec{b} = (b_1, b_2, \dots, b_n)^T$ — вектор свободных членов.

Решение для $x_i$ вычисляется как:
$$
x_i = \frac{\det(A_i)}{\det(A)},
$$
где $A_i$ — это матрица, полученная заменой $i$-го столбца матрицы $A$ на вектор $\vec{b}$.

---

### Формула
Для матрицы $A$ и системы уравнений:
$$
\begin{pmatrix}
a_{11} & a_{12} & \dots & a_{1n} \\
a_{21} & a_{22} & \dots & a_{2n} \\
\vdots & \vdots & \ddots & \vdots \\
a_{n1} & a_{n2} & \dots & a_{nn}
\end{pmatrix}
\begin{pmatrix}
x_1 \\ x_2 \\ \vdots \\ x_n
\end{pmatrix}
=
\begin{pmatrix}
b_1 \\ b_2 \\ \vdots \\ b_n
\end{pmatrix},
$$
решения:
$$
x_i = \frac{\det(A_i)}{\det(A)}, \quad i = 1, 2, \dots, n,
$$
где $A_i$ — это матрица:
$$
A_i =
\begin{pmatrix}
a_{11} & \dots & b_1 & \dots & a_{1n} \\
a_{21} & \dots & b_2 & \dots & a_{2n} \\
\vdots & \ddots & \vdots & \ddots & \vdots \\
a_{n1} & \dots & b_n & \dots & a_{nn}
\end{pmatrix}.
$$
(В $A_i$ $i$-й столбец заменён на $\vec{b}$).

### Условия применения

1. Матрица $A$ должна быть квадратной ($n \times n$).
2. Определитель $\det(A)$ не должен быть равен нулю ($\det(A) \neq 0$).

### Пример

Решим систему:
$$
\begin{cases}
x_1 + 2x_2 + 3x_3 = 1, \\
4x_1 + 5x_2 + 6x_3 = 2, \\
7x_1 + 8x_2 + 10x_3 = 3.
\end{cases}
$$
1. Матрица $A$:
$$
A =
\begin{pmatrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
7 & 8 & 10
\end{pmatrix}, \quad
\vec{b} =
\begin{pmatrix}
1 \\ 2 \\ 3
\end{pmatrix}.
$$

2. Вычислим $\det(A)$:
$$
\det(A) = 1 \cdot \begin{vmatrix} 5 & 6 \\ 8 & 10 \end{vmatrix} - 2 \cdot \begin{vmatrix} 4 & 6 \\ 7 & 10 \end{vmatrix} + 3 \cdot \begin{vmatrix} 4 & 5 \\ 7 & 8 \end{vmatrix}.
$$

Расчёт:
$$
\det(A) = 1 \cdot (5 \cdot 10 - 6 \cdot 8) - 2 \cdot (4 \cdot 10 - 6 \cdot 7) + 3 \cdot (4 \cdot 8 - 5 \cdot 7),
$$
$$
\det(A) = 1 \cdot (-10) - 2 \cdot (-2) + 3 \cdot (-3) = -10 + 4 - 9 = -15.
$$


3. Вычислим $\det(A_1)$ (заменяем 1-й столбец на $\vec{b}$):
$$
A_1 =
\begin{pmatrix}
1 & 2 & 3 \\
2 & 5 & 6 \\
3 & 8 & 10
\end{pmatrix}.
$$
$$
\det(A_1) = 1 \cdot \begin{vmatrix} 5 & 6 \\ 8 & 10 \end{vmatrix} - 2 \cdot \begin{vmatrix} 2 & 6 \\ 3 & 10 \end{vmatrix} + 3 \cdot \begin{vmatrix} 2 & 5 \\ 3 & 8 \end{vmatrix}.
$$
Расчёт:
$$
\det(A_1) = 1 \cdot (-10) - 2 \cdot (-2) + 3 \cdot (-1) = -10 + 4 - 3 = -9.
$$

4. Аналогично находим $\det(A_2)$ и $\det(A_3)$:
$$
\det(A_2) = 0, \quad \det(A_3) = 15.
$$

5. Решения:
$$
x_1 = \frac{\det(A_1)}{\det(A)} = \frac{-9}{-15} = \frac{3}{5}, \quad
x_2 = \frac{\det(A_2)}{\det(A)} = \frac{0}{-15} = 0, \quad
x_3 = \frac{\det(A_3)}{\det(A)} = \frac{15}{-15} = -1.
$$

Итоговое решение:
$$
\vec{x} =
\begin{pmatrix}
\cfrac{3}{5} \\ 0 \\ -1
\end{pmatrix}.
$$
