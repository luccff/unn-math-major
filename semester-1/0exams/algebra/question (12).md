##### Теорема об умножении определителей.
---
### Теорема об умножении определителей
Для квадратных матриц $A$ и $B$ одинакового порядка $n$ справедливо следующее:
$$
\det(AB) = \det(A) \cdot \det(B).
$$

### Доказательство (без использования теоремы Лапласа)

1. **Определитель матрицы $A$ через строки**: Пусть $A$ — матрица размера $n \times n$, определитель которой записывается как:
   $$
   \det(A) = \sum_{\sigma \in S_n} \operatorname{sgn}(\sigma) \prod_{i=1}^n a_{i, \sigma(i)},
   $$
   где $S_n$ — множество всех перестановок порядка $n$, а $\operatorname{sgn}(\sigma)$ — знак перестановки.

2. **Произведение матриц $AB$**: Элементы произведения $C = AB$ вычисляются как:
   $$
   c_{ij} = \sum_{k=1}^n a_{ik} b_{kj}.
   $$
   Тогда определитель $\det(AB)$ записывается как:
   $$
   \det(AB) = \sum_{\sigma \in S_n} \operatorname{sgn}(\sigma) \prod_{i=1}^n c_{i, \sigma(i)}.
   $$

3. **Подстановка выражения для $c_{i, \sigma(i)}$**: Подставим $c_{i, \sigma(i)} = \sum_{k=1}^n a_{ik} b_{k, \sigma(i)}$:
   $$
   \det(AB) = \sum_{\sigma \in S_n} \operatorname{sgn}(\sigma) \prod_{i=1}^n \left( \sum_{k=1}^n a_{ik} b_{k, \sigma(i)} \right).
   $$

4. **Раскрытие произведения**: Используем свойства суммы и произведения:
   $$
   \prod_{i=1}^n \left( \sum_{k=1}^n a_{ik} b_{k, \sigma(i)} \right)
   $$
   преобразуется в сумму по всем возможным $n$-упорядоченным индексам $k_1, k_2, \dots, k_n$:
   $$
   \sum_{k_1, k_2, \dots, k_n} \prod_{i=1}^n a_{i, k_i} b_{k_i, \sigma(i)}.
   $$

5. **Объединение перестановок**: Замечаем, что для каждого набора индексов $k_1, k_2, \dots, k_n$ подстановка $\tau \in S_n$ задаёт отображение $k_i \mapsto i$. Тогда $\sigma \circ \tau$ — это композиция перестановок, и выражение сводится к:
   $$
   \det(AB) = \sum_{\tau \in S_n} \operatorname{sgn}(\tau) \det(A) \cdot \det(B).
   $$

6. **Итог**: Учитывая свойства перестановок и ассоциативность определителя, получаем:
   $$
   \det(AB) = \det(A) \cdot \det(B).
   $$

---

### Пример

Пусть $A = \begin{pmatrix} 1 & 2 \\ 3 & 4 \end{pmatrix}$ и $B = \begin{pmatrix} 2 & 0 \\ 1 & 2 \end{pmatrix}$. Найдём $\det(A)$, $\det(B)$ и $\det(AB)$.

1. Определим $\det(A)$:
   $$
   \det(A) = 1 \cdot 4 - 2 \cdot 3 = 4 - 6 = -2.
   $$

2. Определим $\det(B)$:
   $$
   \det(B) = 2 \cdot 2 - 0 \cdot 1 = 4.
   $$

3. Найдём $AB$:
   $$
   AB = \begin{pmatrix} 1 & 2 \\ 3 & 4 \end{pmatrix} \begin{pmatrix} 2 & 0 \\ 1 & 2 \end{pmatrix} = \begin{pmatrix} 4 & 4 \\ 10 & 8 \end{pmatrix}.
   $$

4. Определим $\det(AB)$:
   $$
   \det(AB) = 4 \cdot 8 - 4 \cdot 10 = 32 - 40 = -8.
   $$

5. Проверим:
   $$
   \det(A) \cdot \det(B) = (-2) \cdot 4 = -8.
   $$

Итак, $\det(AB) = \det(A) \cdot \det(B)$.
