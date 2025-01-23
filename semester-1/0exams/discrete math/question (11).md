##### Сравнение мощностей множеств, равномощные множества: ${\displaystyle |A| = |B|, \  |A| \leq |B|, \  |A|<|B|}$. Свойства равномощности (рефлексивность, симметричность, транзитивность). Равномощность интервалов, полуинтервалов и отрезков в ${\displaystyle \mathbb{R}}$. Счетные множества. Несчетные множества. Свойства счетных множеств. Примеры. Несчетность множества ${\displaystyle \mathbb{R}}$. Мощность континуума. Теорема Кантора (${\displaystyle |A| < |2^{ A }|}$ для любого множества ${\displaystyle A}$). Следствие: несчетность множества ${\displaystyle 2^{ \mathbb{N} }}$. Равномощность ${\displaystyle 2^{ \mathbb{N} }}$ и множества ${\displaystyle \{ 0, \ 1 \}^{ \infty }}$ бесконечных последовательностей из 0 и 1.
---
### Сравнение бесконечных множеств.
$$\displaylines{
A, \ B - \text{ конечные. } \\
}$$
Утверждение.
$$\displaylines{
|A| \leq |B| \iff \exists\text{ инъекция  } f: A \to  B \\
|A| \geq |B | \iff \exists\text{ сюрьекция } f: A \to  B\\
|A|=|B| \iff \exists\text{ биекция } f: A \to  B
}$$
Определение. ${A, \ B \text{ любые множества }}$
$$\displaylines{
A \sim B \text{ или } |A| = |B| \iff  \exists\text{ биекция } f:A \to  B \\
|A|\leq |B| \iff \exists\text{ инъекция } f:A \to B \\
|A| < |B| \iff \begin{cases}
|A| \leq |B| \\
A \cancel{\sim } B \ (\text{нет биекции})
\end{cases}
}$$
Утверждение.
$$\displaylines{
|A| \leq |B| \iff  \exists B' \subseteq B, \ A \sim B' \\
\text{ Доказательство: } (\implies)  \quad \exists f:A \to  B \text{ инъкекция } \quad B' = f(A)(\impliedby ) \quad \begin{matrix}
 \exists g:A \to  B' \text{ биекция }  \\
\overset{\sim }{g}: A \to  B \text{ инъекция }  \\
\overset{\sim }{g}(x) = g(x) \quad\forall{x \in A}
\end{matrix}
}$$
Утверждение 2.
$$\displaylines{
A\sim B, \ |B| < |C| \implies |A| < |C| \\
\text{ Доказательство: } \quad f: A \to  B \text{ биекция }, \ g: B \to  C \text{ инъекция }\implies  g \circ f: A \to  C \text{ инъекция } \\
\implies  |A| \leq |C| \\
\text{ Докажем, что } A \cancel{\sim } C \\
\text{ От противного: } \text{ Пусть  } A \sim  C \implies \exists \ h: A \to  C \text{ биекция } \\
h \circ f^{ -1 } : B \to  C \text{ биекция } - \text{ противоречние. }
}$$
Свойства ${\sim}$:
1) ${A \sim A \quad (id_{ A }: A \to A)}$
2) ${A \sim B \implies B\sim A}$
3) ${A \sim B, \ B \sim C \implies A \sim C}$

Пример.
$$\displaylines{
\mathbb{N} \sim  \{ 1, \ 4, \ 9, \ 16, \ 25, \ \dots  \} = \{ n^{ 2 } | n \in \mathbb{N} \} \\
n \longmapsto n^{ 2 }
}$$
Пример.
$$\displaylines{
\mathbb{Z} \sim  \mathbb{N} \\
f: \mathbb{Z} \to  \mathbb{N} \text{ биекция }
}$$
Пример.
$$\displaylines{
[0; 1) \sim  (0;1) \\
f:[0; 1) \to  (0;1) \\
f(x) = \begin{cases}
\dfrac{1}{2}, \ x \neq 0 \\
\dfrac{x}{2}, \ x = \dfrac{1}{2^{ k }}, \ k \in \mathbb{N} \\ 
x, \ \text{ иначе } 
\end{cases}
}$$

Теорема Кантора-Шрёдера-Бернштейна.
$$\displaylines{
\text{ Если } \exists \text{ инъекц. } f: A \to  B \text{ и } g: B \to A, \ \text{ то } A \sim  B
}$$
---
### Счётные множества.
Определение.
$$\displaylines{
A - \text{ счетное, если } A \sim \mathbb{N}\\
(\exists\text{ биекция } f: A \to  \mathbb{N}, \ g:\mathbb{N} \to  A)
}$$
Определение.
$$\displaylines{
A - \text{ несчетное, если } A - \text{ бесконечное и  } A \cancel{\sim } \mathbb{N}
}$$
Теорема.
$$\displaylines{
(0;1) - \text{ несчётные }
}$$
Доказательство от противного.
$$\displaylines{ \text{ Сноска. }\\
x \in (0;1) \quad x = 0, \ x_{1}, \ x_{2}, \ \dots \\
 0, \ a_{1}, \  \dots a_{n}, 9, \ 9\dots =
0, \ a_{1}, \ \dots a_{n+1}, \ 0, \ 0
}$$
$$\displaylines{
\text{ Пусть } (0, \ 1) \sim  \mathbb{N} \\
\exists\text{ биекция } f: \mathbb{N} \to  (0;1) \\
f(1) = 0, \ x_{11}, \ x_{12}, \ \dots \\
f(2) = 0, \ x_{21}, \ x_{22}, \ \dots \\
f(3) = 0, \ x_{31}, \ x_{32}, \ \dots \\
\dots \\
\text{ Рассматриваем цифры } x_{jj}, \ j=1, \ 2\dots \\
\text{ Строим число  } y = 0, \ y_{1} y_{2}y_{3}\dots y_{n}\dots \\
y_{n} = \begin{cases}
2, \ \text{ если } x_{nn} = 1  \\
1, \  \text{ если } x_{nn}\neq 1
\end{cases} \\
y\neq f(1) (\text{отлич. в первой цифре после запятой}) \\
y\neq f(n) \quad \forall{n} \in  \mathbb{N} (y_{n}\neq x_{nn}) \\
\text{ Противоречие. }
}$$
Следствие.
$$\displaylines{
\mathbb{R} - \text{ несчетные }, \ |\mathbb{N}| < |\mathbb{R}|
}$$
Все счетные множества равномощны.

Определение.
$$\displaylines{
\text{ Если } A\sim \mathbb{R}, \ \text{ то } A \text{ имеет можщность } \textbf{ континуума }
}$$
Теорема Кантора.
$$\displaylines{
\forall{\text{ ин. } A} \quad |A|<|2^{ A }| \\
\text{ Доказательство: } |A| \leq |2^{ A} \quad \exists i: A \to  2^{ A } \\
\text{ Докажем, что  } A \not \sim 2^{ A } \\
\text{ От противного. } \text{ Пусть  } \exists\text{ биекция } f:A\to 2^{ A } \ f(x) \subseteq A \\
M = \{ x \in A | x \not \in f(x) \} \subseteq A \quad M \in  2^{ A } \\
f: A \to  2^{ A } \\
m \longmapsto M = f(m) \\
\text{ Вопрос: } m \in f(m) ? \\
m \in  f(m) = M \implies  m \cancel{\in } f(m) \text{ противоречие } \\
m \cancel{\in}  f(m) = M \implies  m \in f(m) \text{ противоречие }
}$$
Бесконечная иерархия мощностей.
$$\displaylines{
|\mathbb{N}| < |2^{ \mathbb{N} }| < |2^{ 2^{ \mathbb{N} } }| < \dots 
}$$
Утверждение.
$$\displaylines{
\text{ Множество бесконечно последовательно из 0 и 1 равномощно } 2^{ \mathbb{N} } \\
\text{ Доказательсвто: } f: 2^{ \mathbb{N} } \to S \text{ биекция }\\
\emptyset \longmapsto 000\dots \\
\{ 1, \ 3 \} \longmapsto 1010\dots 
}$$
Теорема.
$$\displaylines{
\mathbb{R}\sim 2^{ \mathbb{N} }
}$$
