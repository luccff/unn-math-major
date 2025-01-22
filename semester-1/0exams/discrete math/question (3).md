##### Множество всех подмножеств множества (булеан). Теорема о числе подмножеств конечного множества.
---
Если элементами множества ${\displaystyle X}$ являются подмножества ${\displaystyle A}$, то говорят, что ${\displaystyle X}$ есть семейство подмножеств ${\displaystyle A}$. Семейство всех подмножеств ${\displaystyle A}$ обозначается через ${\displaystyle 2^{ A }}$. Например ${\displaystyle A = \{ a, \ b \}}$, то ${\displaystyle 2^{ A } = \{ \emptyset, \ \{ a \}, \ \{ b \}, \ \{ a, \ b \} \}}$.

Теорема о числе подмножеств.
Если ${\displaystyle A}$ - конечное множество, то ${\displaystyle |2^{ A }| = 2^{ |A| }}$.
Доказательство:
Пусть ${\displaystyle |A| = n}$. 
При ${\displaystyle n = 0}$: ${\displaystyle 2^{ 0 } = 1}$ - верно.
При ${\displaystyle n>0}$ возьмем ${\displaystyle x \in A}$ и обозначим ${\displaystyle B = A\backslash\{ x \}}$. Тогда ${\displaystyle |B| = n-1}$. Предположим что ${\displaystyle \forall{B}}$ с ${\displaystyle |B| = n-1}$ утверждение верно: ${\displaystyle |2^{ B }| = 2^{ n-1 }}$.
Тогда подмножества ${\displaystyle A}$ делятся на 2 типа: содержащие ${\displaystyle x}$ и не содержащие ${\displaystyle x}$. 
1.  Это подмножества множества ${\displaystyle B}$. Их количество равно ${\displaystyle 2^{ n-1 }}$.
2. Каждое такое подмножество можно получить, взяв любое подмножество $B$ и добавив к нему элемент $x$. Количество таких подмножеств также равно ${\displaystyle  2^{ n-1 }}$.
Общее число подмножеств ${\displaystyle A}$: ${\displaystyle |2^{ A }| = 2^{ n-1 } + 2^{ n-1 } = 2^{ n }}$.