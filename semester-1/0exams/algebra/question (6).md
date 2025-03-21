##### Группа подстановок n-й степени. Четность подстановки. Транспозиции. Разложение подстановки в произведение транспозиций и четность перестановки.
---
### Группа подстановок $n$-й степени
**Группа подстановок $S_n$** (или группа перестановок) — это множество всех возможных перестановок $n$-элементного множества $X = \{1, 2, \dots, n\}$, наделённое операцией композиции подстановок.

1. Элементы группы $S_n$ — это биекции $\sigma: X \to X$, то есть перестановки множества $X$.
2. Композиция подстановок $\sigma$ и $\tau$ ($\sigma \circ \tau$) определяется как последовательное применение: $(\sigma \circ \tau)(x) = \sigma(\tau(x))$.
3. Нейтральным элементом в $S_n$ является тождественная подстановка $e(x) = x$ для всех $x \in X$.
4. Для каждой подстановки $\sigma$ существует обратная подстановка $\sigma^{-1}$, такая, что $\sigma \circ \sigma^{-1} = e$.

Число элементов группы $S_n$ равно $n!$.

Пример: Для $n = 3$, множество $\{1, 2, 3\}$ имеет $3! = 6$ перестановок:
$$
S_3 = \{\text{id}, (1\;2), (1\;3), (2\;3), (1\;2\;3), (1\;3\;2)\}.
$$

### Чётность подстановки
Чётность подстановки определяется через количество **инверсий**. Подстановка $\sigma$ является:
- **Чётной**, если число инверсий в ней чётно.
- **Нечётной**, если число инверсий нечётно.

### Инверсии
Инверсия — это пара $(i, j)$, где $i < j$, но $\sigma(i) > \sigma(j)$.

Пример: Для подстановки $\sigma = [3, 1, 2]$,
- Инверсии: $(3 > 1), (3 > 2)$,
- Число инверсий $I(\sigma) = 2$, значит, подстановка чётная.

 Связь с разложением в транспозиции
Чётность подстановки также определяется количеством транспозиций в её разложении:
- Если подстановка разложена в чётное число транспозиций, то она чётная.
- Если в нечётное число транспозиций — нечётная.

### Транспозиции
**Транспозиция** — это подстановка, меняющая местами два элемента, оставляя остальные элементы на своих местах. Обозначается $(i\;j)$, где $i, j \in \{1, 2, \dots, n\}$.

Пример: Транспозиция $(1\;3)$ при применении к $X = [1, 2, 3]$ даст $X' = [3, 2, 1]$.

Свойства транспозиций
1. Каждая транспозиция является **нечётной** подстановкой (одно инвертирование увеличивает число инверсий на 1).
2. Любая перестановка может быть разложена в произведение транспозиций.

### Разложение подстановки в произведение транспозиций и чётность подстановки
Теорема. Любая подстановка $\sigma \in S_n$ может быть представлена в виде произведения транспозиций:
$$
\sigma = (i_1\;j_1)(i_2\;j_2)\dots(i_k\;j_k).
$$

Свойства
1. Чётность числа транспозиций в разложении определяет чётность подстановки:
   - Если $k$ — чётное, то подстановка чётная.
   - Если $k$ — нечётное, то подстановка нечётная.
2. Разложение в транспозиции **не уникально**, но чётность количества транспозиций всегда остаётся неизменной.


Пусть дана подстановка $\sigma = (1\;3\;2)$ для множества $\{1, 2, 3\}$ (циклическая перестановка). Разложим её в транспозиции:
$$
\sigma = (1\;2)(1\;3).
$$
Здесь 2 транспозиции (чётное число), значит, подстановка $\sigma$ чётная.

### Группа чётных подстановок ($A_n$)
Множество всех чётных подстановок из $S_n$ образует подгруппу, называемую **группой чётных подстановок** $A_n$ (или **альтернирующей группой**). Число элементов в $A_n$ равно $\frac{n!}{2}$.
