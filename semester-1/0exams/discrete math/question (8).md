##### Отношение эквивалентности. Примеры. Разбиение множества. Показать, что любое разбиение множества задает на нем отношение эквивалентности. Классы эквивалентности. Свойства классов эквивалентности (каждый класс однозначно определяется любым своим элементом; два любых класса либо совпадают, либо не пересекаются). Теорема о факторизации. Фактор множество ${\displaystyle A/R}$.
---
${\displaystyle R \subseteq A^{ 2 }}$ - отношение эквивалентности, если ${\displaystyle R}$ - рефлексивно, симметрично, транзитивно.

Отношение равенства на любом множестве есть отношение эквивалентности.
Отношение параллельности прямых на плоскости - отношение эквивалентности.
Если ${\displaystyle xRy}$, то говорят что ${\displaystyle x}$ и ${\displaystyle y}$  сравнимы по модулю ${\displaystyle n}$: ${\displaystyle x\equiv y \mod{n}}$

Разбиение множества $A$ – это такое семейство его непустых подмножеств, что $\forall$ элемент из $A$ принадлежит ровно одному подмножеству этого семейства. Подмножество семейства – это часть разбиения. Части разбиения не пересекаются.

Пусть $A$ – конечно. 
$$\displaylines{
F = \{ F_{ 1 }, F_{ 2 }, \dots, F_{ k } \} \ – \ F \text{  разбиение }А \\ 
1. \ \ F_{ i } \subseteq A \text{ и } F_{ i } \neq \emptyset \\ 
2. \ \ A = F_{ 1 } \cup F_{ 2 } \cup \dots \cup F_{ k } \\ 
3. \ \ F_{ i } \cap F_{ j } = \emptyset, \ \ i \neq j
}$$

Любое разбиение множества $A$ задает на нем отношение эквивалентности, и обратно — каждое отношение эквивалентности задает разбиение.
Доказательство:
1. Разбиение ${\displaystyle \to}$ отношение эквивалентности:
$$\displaylines{
aRb \iff a, \  b \text{ принадлежат одному подножеству разбиения }
}$$
Рефлексивность: ${\displaystyle a, \ a}$ лежат в одном подмножестве.
Симметричность: если ${\displaystyle a, \ b}$ в одном подмножестве, ${\displaystyle b, \ a}$ тоже.
Транзитивность: если ${\displaystyle a, \ b}$ в одном подмножестве и ${\displaystyle b, \ c}$ в одном, то ${\displaystyle a, \ c}$ тоже.

2. Отношение эквивалентности ${\displaystyle \to}$ разбиение:
Классы эквивалентности ${\displaystyle [a] = \{ b \in A \ | \ aRb \}}$ образуют разбиение.
Непересекаемость: если ${\displaystyle [a] \cap [b] = \emptyset}$, то ${\displaystyle [a] = [b]}$
Объединение: ${\displaystyle \bigcup_{ a \in A }[a] = A}$.

Класс эквивалентности ${\displaystyle a}$ - это множество всех элементов, связанных с ${\displaystyle a}$ отношением ${\displaystyle R}$:
$$\displaylines{
[a] = \{ b \in A \ | \ aRb \}
}$$
${\displaystyle a \in [a] }$, так как ${\displaystyle aRa}$.

Пример: ${\displaystyle A = \mathbb{Z}, \  x \sim y \iff x - y \ \vdots \ 2}$
$$\displaylines{
[0] = \{ y \in  \mathbb{Z}  : 0-y \ \vdots  \ 2 \} = \{ 2n: n \in  \mathbb{Z}  \} \\
[1] = \{ y \in \mathbb{Z} : 1 - y \ \vdots  \ 2 \} = \{ 2n+1: n \in  \mathbb{Z}  \} \\
[2] = [0], \   [5] = [1] \\
F = \{ [0], \  [1] \} - \text{ разбиение  } \mathbb{Z} 
}$$

Утверждение. ${\displaystyle y \in [x] \implies [y] = [x]}$
Доказательство: ${\displaystyle x \sim y}$ по определению.
$$\displaylines{
\forall{z} \in [y] \implies  y \sim z \implies x \sim z \implies  z \in  [x] \implies [y] \subseteq [x] \\
\forall{a} \in  [x] \implies x \sim a \implies y \sim a \implies  a \in  [y] \implies [x] \subseteq [y]
}$$

Следствие: ${\displaystyle \forall{x, \ y} \in A}$ либо ${\displaystyle [x] = [y]}$, либо ${\displaystyle [x] \cap [y] = \emptyset}$.
Доказательство: пусть ${\displaystyle \exists z \in [x] \cap [y] \implies z \in [x], \ [y] \implies [z] = [x] = [y] \implies [x] = [y]}$. Если пусто, то нечего доказывать.

Теорема о факторизации. Если существует отношение эквивалентности на множестве ${\displaystyle A}$, тогда такое множество ${\displaystyle F = \{ [x] :x \in A \}}$ - разбиение ${\displaystyle A}$. При этом $F$ называют фактор множеством $A$ по отношению к $R \ (\sim)$ и обозначается $F = A/R (\sim)$. 

Доказательство: ${\displaystyle \forall{x} \in A : x \in[x]}$. Если ${\displaystyle x \in [y]}$, то ${\displaystyle [x] = [y] \implies x}$ принадлежит только одному классу эквивалентности.