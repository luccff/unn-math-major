Работу выполнил Уткин Никита 3824Б1МА1.
### Задание 1.
Граф ${\displaystyle G}$ задан матрицей смежности:
$$\displaylines{
\begin{pmatrix}
0 & 1 & 0 & 1 & 0 & 0 & 0 & 0 \\
1 & 0 & 1 & 1 & 1 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 & 1 & 1 & 0 & 0 \\
1 & 1 & 0 & 0 & 1 & 1 & 1 & 0 \\
0 & 1 & 1 & 1 & 0 & 0 & 1 & 1 \\
0 & 0 & 1 & 1 & 0 & 0 & 1 & 0 \\
0 & 0 & 0 & 1 & 1 & 1 & 0 & 1 \\
0 & 0 & 0 & 0 & 1 & 0 & 1 & 0
\end{pmatrix}
}$$
Требуется:
1. Задать граф списками смежности и изобразить его.
2. Найти ${\displaystyle \text{ diam}(G), \ \text{ rad}(G), \ \text{ Center}(G)}$.
3. Определить, является ли граф планарным.
4. Определить, является ли граф самодополнительным.

Решение:
1. Матрица смежности описывает неориентированный граф с 8 вершинами, обзовём их ${\displaystyle (v_{ 1 }, \ v_{ 2 }, \ \dots, \ v_{ 8 }) }$. 
Зададим граф списками смежности:
$$\displaylines{
\begin{aligned}
& v_{ 1 }: \ v_{ 2 }, \  v_{ 4 } \\
& v_{ 2 }: \ v_{ 1 }, \  v_{ 3 }, \  v_{ 4 }, \  v_{ 5 } \\
& v_{ 3 }: \ v_{ 2 }, \  v_{ 5 }, \  v_{ 6 } \\
& v_{ 4 }: \ v_{ 1 }, \  v_{ 2 }, \  v_{ 5 }, \  v_{ 6 }, \  v_{ 7 } \\
& v_{ 5 }: \ v_{ 2 }, \  v_{ 3 }, \  v_{ 4 }, \  v_{ 7 }, \  v_{ 8 } \\
& v_{ 6 }: \ v_{ 3 }, \  v_{ 4 }, \  v_{ 7 } \\
& v_{ 7 }: \ v_{ 4 }, \  v_{ 5 }, \  v_{ 6 }, \  v_{ 8 } \\
& v_{ 8 }: \ v_{ 5 }, \  v_{ 7 }
\end{aligned}
}$$

Изобразим его:
```tikz
\begin{document}

\begin{tikzpicture}[scale=1.2]
    \node[circle, draw, minimum size=8mm, font=\large] (v1) at (-3, 3) {$v_1$};
    \node[circle, draw, minimum size=8mm, font=\large] (v2) at (-3, 0) {$v_2$};
    \node[circle, draw, minimum size=8mm, font=\large] (v3) at (-3, -3) {$v_3$};
    \node[circle, draw, minimum size=8mm, font=\large] (v4) at (3, 3) {$v_4$};
    \node[circle, draw, minimum size=8mm, font=\large] (v5) at (0, 0) {$v_5$};
    \node[circle, draw, minimum size=8mm, font=\large] (v6) at (6, -3) {$v_6$};
    \node[circle, draw, minimum size=8mm, font=\large] (v7) at (3, -2) {$v_7$};
    \node[circle, draw, minimum size=8mm, font=\large] (v8) at (0, -2) {$v_8$};

    % Рисование рёбер
    \draw[thick] (v1) -- (v2);
    \draw[thick] (v1) -- (v4);
    \draw[thick] (v2) -- (v3);
    \draw[thick] (v2) -- (v4);
    \draw[thick] (v2) -- (v5);
    \draw[thick] (v3) -- (v5);
    \draw[thick] (v3) -- (v6);
    \draw[thick] (v4) -- (v5);
    \draw[thick] (v4) -- (v6);
    \draw[thick] (v4) -- (v7);
    \draw[thick] (v5) -- (v7);
    \draw[thick] (v5) -- (v8);
    \draw[thick] (v6) -- (v7);
    \draw[thick] (v7) -- (v8);
\end{tikzpicture}

\end{document}
```

2. По данному графу построим таблицу расстояний:
$$\displaylines{
\begin{array}{|c|cccccccc|c|} \hline 
x \backslash y & 1 & 2 & 3 & 4 & 5 & 6 & 7 & 8 & \text{ecc}(y) \\
\hline
1 & 0 & 1 & 2 & 1 & 2 & 2 & 2 & 3 & 3 \\
2 & 1 & 0 & 1 & 1 & 1 & 2 & 2 & 2 & 2 \\
3 & 2 & 1 & 0 & 2 & 1 & 1 & 2 & 2 & 2 \\
4 & 1 & 1 & 2 & 0 & 1 & 1 & 1 & 2 & 2 \\
5 & 2 & 1 & 1 & 1 & 0 & 2 & 1 & 1 & 2 \\
6 & 2 & 2 & 1 & 1 & 2 & 0 & 1 & 2 & 2 \\
7 & 2 & 2 & 2 & 1 & 1 & 1 & 0 & 1 & 2 \\
8 & 3 & 2 & 2 & 2 & 1 & 2 & 1 & 0 & 3 \\ \hline 
\end{array}
}$$

${\displaystyle \text{diam}(G) = \max_{ x \in  V } \max_{ y \in V } d(x, \  y) = \max_{ x \in V } \text{ ecc}(x)}$. Следовательно, ${\displaystyle \text{ diam}(G) = 3}$.
Радиус - минимальный эксцентриситет. ${\displaystyle \text{ rad}(G) = \min_{ x \in V } \text{ ecc}(x)}$, следовательно, ${\displaystyle \text{ rad}(G) = 2}$.
Центр графа - множество всех вершин с минимальным эксцентриситетом. Следовательно, ${\displaystyle \text{ Center}(G) = \{ v_{ 2 }, \ v_{ 3 }, \ v_{ 4 }, \ v_{ 5 }, \ v_{ 6 }, \ v_{ 7 } \}}$.

3. Так как мы смогли нарисовать граф без пересечения ребер, это доказывает, что он планарен. Выполним проверку по формуле Эйлера:
$$\displaylines{
|E| \leq 3|V| - 6 \\
14 \leq 8 \cdot 8 - 6 = 14 \leq 18
}$$
4. Граф ${\displaystyle G}$ самодополнителен, если он изоморфен дополнению ${\displaystyle \overline{G}}$.
В нашем графе ${\displaystyle |V| = 8, \ |E| = 14}$. Для самодополнительного графа ${\displaystyle \overline{G}}$ с ${\displaystyle n}$ вершинами ${\displaystyle |E| = \frac{n(n-1)}{4}}$. 
$$\displaylines{
|E| = \frac{8(8-1)}{4}  \\
14 = 14
}$$
Необходимое условие выполнилось.
Запишем матрицу смежности для ${\displaystyle \overline{G}:}$
$$\displaylines{
\overline{G} = \begin{pmatrix}
0 & 0 & 1 & 0 & 1 & 1 & 1 & 1 \\
0 & 0 & 0 & 0 & 0 & 1 & 1 & 1 \\
1 & 0 & 0 & 1 & 0 & 0 & 1 & 1 \\
0 & 0 & 1 & 0 & 0 & 0 & 0 & 1 \\
1 & 0 & 0 & 0 & 0 & 1 & 0 & 0 \\
1 & 1 & 0 & 0 & 1 & 0 & 0 & 1 \\
1 & 1 & 1 & 0 & 0 & 0 & 0 & 0 \\
1 & 1 & 1 & 1 & 0 & 1 & 0 & 0
\end{pmatrix}
}$$
Методом пристального взгляда, можно заметить подстановку изоморфизма между ${\displaystyle G}$ и ${\displaystyle \overline{G}}$:
$$\displaylines{
\begin{pmatrix}
v_1 & v_2 & v_3 & v_4 & v_5 & v_6 & v_7 & v_8 \\
v_8' & v_7' & v_6' & v_5' & v_4' & v_3' & v_2' & v_1'
\end{pmatrix}
}$$
Итого: изоморфность подтверждается через перестановку ${\displaystyle v_{ i } \leftrightarrow v_{ 9-i }}$.

---
### Задание 2.
Задан код Прюфера ${\displaystyle P(T) = (3, \ 2, \ 4, \ 7, \ 4, \ 2, \ 7, \ 7, \ 2, \ 5)}$. Восстановить исходное дерево, затем выполнить проверку, выписав полную таблицу. Найти ${\displaystyle \text{ Center}(T)}$ по построению кода Прюфера.
$$\displaylines{
n - 2 = 10 \implies  n = 12. \\
\begin{array}{|c|cccccccccccc|c|} \hline 
 i& 1 & 2 & 3 & 4 & 5 & 6 & 7 & 8 & 9 & 10 & 11 & 12 & (a_{i}; b_{i}) \\ \hline 
1 & \boxed{1} & 4 & 2 & 3 & 2 & 1 & 4 & 1 & 1 & 1 & 1 & 1 & (1 ; 3) \\ \hline 
2 & 0 & 4 & \boxed{1} & 3 & 2 & 1 & 4 & 1 & 1 & 1 & 1 & 1 & (3 ; 2) \\ \hline 
3 & 0 & 3 & 0 & 3 & 2 & \boxed{1} & 4 & 1 & 1 & 1 & 1 & 1 & (6 ; 4) \\ \hline 
4 & 0 & 3 & 0 & 2 & 2 & 0 & 4 & \boxed{1} & 1 & 1 & 1 & 1 & ( 8; 7) \\ \hline 
5 & 0 & 3 & 0 & 2 & 2 & 0 & 3 & 0 & \boxed{1} & 1 & 1 & 1 & (9 ; 4) \\ \hline 
6 & 0 & 3 & 0 & \boxed{1} & 2 & 0 & 3 & 0 & 0 & 1 & 1 & 1 & (4 ; 2) \\ \hline 
7 & 0 & 2 & 0 & 0 & 2 & 0 & 3 & 0 & 0 & \boxed{1} & 1 & 1 & ( 10; 7) \\ \hline 
8 & 0 & 2 & 0 & 0 & 2 & 0 & 2 & 0 & 0 & 0 & \boxed{1} & 1 & (11 ; 7) \\ \hline 
9 & 0 & 2 & 0 & 0 & 2 & 0 & \boxed{1} & 0 & 0 & 0 & 0 & 1 & (7 ; 2) \\ \hline 
10 & 0 & \boxed{1} & 0 & 0 & 2 & 0 & 0 & 0 & 0 & 0 & 0 & 1 & (2 ; 5) \\ \hline 
11 & 0 & 0 & 0 & 0 & 1 & 0 & 0 & 0 & 0 & 0 & 0 & 1 & (5 ; 12) \\ \hline 

\end{array}
}$$
Построим дерево:
```tikz
\begin{document}

\begin{tikzpicture}[scale=1.2]
    \node[circle, draw, minimum size=8mm, font=\large] (1) at (-6, -3) {$1$};
    \node[circle, draw, minimum size=8mm, font=\large] (2) at (0, 3) {$2$};
    \node[circle, draw, minimum size=8mm, font=\large] (3) at (-4, 0) {$3$};
    \node[circle, draw, minimum size=8mm, font=\large] (4) at (-2, 0) {$4$};
    \node[circle, draw, minimum size=8mm, font=\large] (5) at (0, 0) {$5$};
    \node[circle, draw, minimum size=8mm, font=\large] (6) at (-4, -3) {$6$};
    \node[circle, draw, minimum size=8mm, font=\large] (7) at (4, 0) {$7$};
    \node[circle, draw, minimum size=8mm, font=\large] (8) at (2, -3) {$8$};
    \node[circle, draw, minimum size=8mm, font=\large] (9) at (-2, -3) {$9$};
    \node[circle, draw, minimum size=8mm, font=\large] (10) at (4, -3) {$10$};
    \node[circle, draw, minimum size=8mm, font=\large] (11) at (6, -3) {$11$};
    \node[circle, draw, minimum size=8mm, font=\large] (12) at (0, -3) {$12$};
    
    \draw[thick] (2) -- (4);
    \draw[thick] (2) -- (3);
    \draw[thick] (2) -- (5);
    \draw[thick] (2) -- (7);
    \draw[thick] (4) -- (6);
    \draw[thick] (4) -- (9);
    \draw[thick] (3) -- (1);
    \draw[thick] (5) -- (12);
    \draw[thick] (7) -- (8);
    \draw[thick] (7) -- (10);
    \draw[thick] (7) -- (11);
    
\end{tikzpicture}

\end{document}
```
По изображению дерева можно увидеть, что у вершины 2 минимальный эксцентриситет ${\displaystyle = 2, }$ следовательно ${\displaystyle \text{ Center}(T) = \{ 2 \}.}$
Закодируем дерево заново, чтобы проверить.
Алгоритм: находим лист с наименьшим номером, записываем номер вершины с которой этот лист соединен в код, удаляем лист и ребро. Повторяем ${\displaystyle n-2}$ раз.
$$\displaylines{
\begin{aligned}
1. \ & \text{ Удаляем вершину 1, записываем 3 в код: } [3] \\
2. \ & \text{ Удаляем вершину 3, записываем 2 в код: } [3, \  2] \\
3. \ & \text{ Удаляем вершину 6, записываем 4 в код: } [3, \  2, \  4] \\
4. \ & \text{ Удаляем вершину 8, записываем 7 в код: } [3, \  2, \  4, \  7] \\
5. \ & \text{ Удаляем вершину 9, записываем 4 в код: } [3, \  2, \  4, \  7, \  4] \\
6. \ & \text{ Удаляем вершину 4, записываем 2 в код: } [3, \  2, \  4, \  7, \  4, \  2] \\
7. \ & \text{ Удаляем вершину 10, записываем 7 в код: } [3, \  2, \  4, \  7, \  4, \  2, \ 7 ] \\
8. \ & \text{ Удаляем вершину 11, записываем 7 в код: } [3, \  2, \  4, \  7, \  4, \  2, \ 7, \  7 ] \\
9. \ & \text{ Удаляем вершину 7, записываем 2 в код: } [3, \  2, \  4, \  7, \  4, \  2, \ 7, \  7, \ 2  ] \\
10. \ &  \text{ Удаляем вершину 2, записываем 5 в код: } [3, \  2, \  4, \  7, \  4, \  2, \ 7, \  7, \ 2 , \  5 ]
\end{aligned}
}$$
Они полностью совпадают. Визуализацию можно посмотреть [тут.](https://www.youtube.com/watch?v=cyQWlj34XG8)

---
### Задание 3. 
Дан граф-дерево ${\displaystyle T}$ с ${\displaystyle n\geq2}$ вершинами, в котором нет таких вершин ${\displaystyle v}$, что ${\displaystyle deg(v) = 2}$. Доказать, что в графе ${\displaystyle T}$ не менее чем ${\displaystyle \frac{n}{2} + 1}$ листьев.
Доказательство:
Лемма о рукопожатиях говорит, что ${\displaystyle \sum_{v \in V} \deg(v) = 2|E|}$. Для дерева ${\displaystyle T}$ с ${\displaystyle n }$ вершинами ${\displaystyle |E| = n-1}$:
$$\displaylines{
\sum_{v \in  V} \deg(v) = 2(n-1) 
}$$
Пусть ${\displaystyle l}$ - число листьев ${\displaystyle (\deg(v) = 1)}$, ${\displaystyle k}$ - число внутренних вершин ${\displaystyle (\deg(v) \geq 3)}$.
$$\displaylines{
 n=l + k  \\
\sum_{v \in  V} \deg(v) = \sum_{\text{листья}} \deg(v) + \sum_{\text{внутренние}}^{} \deg(v) \\
\sum_{v \in  V} \deg(v) \geq l+3k \\
l+3k \leq 2(n-1). \text{ Выразим } k \text{ через } n \text{ и } l \text{ и упростим}: \\
-2l + 3n \leq  2n-2 \\
-2l + n + 2 \leq 0 \\
l \geq  \frac{n+2}{2} \\
l \geq \frac{n}{2} + 1
}$$
Замечание: для ${\displaystyle n = 3}$ построить дерево без вершины ${\displaystyle deg(v) = 2}$ невозможно.

---

Примечание. В последующих задачах мною будут использоваться обозначения не как в самих задачах и лекциях, а как удобно мне. Я не люблю обозначать графы, множества вершин и ребер одними буквами с разными индексами, мне сложно в них ориентироваться. 

---
### Задание 4.
Доказать, что изоморфизм графов является отношением эквивалентности.
Доказательство:
1. Рефлексивность:
$$\displaylines{
\forall{G}: \ G \cong G
}$$
Рассмотрим ${\displaystyle G}$ с множеством вершин ${\displaystyle V}$ и множеством ребер ${\displaystyle E}$. Зададим отображение:
$$\displaylines{
f: V \to V,  \quad \forall{v \in  V} : f(v) = v
}$$
Проверим, является ли ${\displaystyle f}$ изоморфизмом: ${\displaystyle f}$ - биекция, так как каждую вершину ${\displaystyle v}$ она отображает в саму себя. 
${\displaystyle f}$ сохраняет ребра: ${\displaystyle (u, \ v) \in E \to (f(u), \ f(v)) = (u, \ v)}$. 
Итого: ${\displaystyle G \cong G}$.

2. Симметричность:
$$\displaylines{
\forall{G, \  H}:  \ G \cong H \implies H \cong G
}$$
Пусть ${\displaystyle G \cong H}$, то есть ${\displaystyle \exists f}$ биекция ${\displaystyle : V(G) \to V(H)}$, которая сохраняет ребра ${\displaystyle (u, \ v) \in E(G) \iff (f(u), \ f(v)) \in E(H)}$. 
Поскольку ${\displaystyle f}$ биекция, ${\displaystyle \exists f^{ -1 }}$, которое тоже будет биекцией. 
Проверим его на изоморфизм: пусть ${\displaystyle (x, \ y) \in E(H)}$, тогда ${\displaystyle \exists u, \ v \in V(G): f(u) = x, \  f(v) = y, \ (u, \ v) \in E(G)}$ ${\displaystyle \implies}$ ${\displaystyle (f^{ -1 }(x), \ f^{ -1 }(y)) = (u, \ v) \in E(G)}$, значит ${\displaystyle f^{ -1 }}$ сохраняет ребра ${\displaystyle (x, \ y) \in E(H) \iff (f^{ -1 }(x), \ f^{ -1 }(y)) \in E(G)}$. 
Итого: ${\displaystyle f^{ -1 }}$ - изоморфизм между ${\displaystyle H }$ и ${\displaystyle G \implies H \cong G}$.

3. Транзитивность:
$$\displaylines{
\forall{G, \  H, \  K}: \ G \cong H, \  H \cong K\implies G \cong K
}$$
Пусть ${\displaystyle G \cong H, \ H \cong K}$ с изоморфизмами ${\displaystyle f: V(G) \to V(H)}$ и ${\displaystyle g: V(H) \to V(K)}$ соответственно. 
Рассмотрим ${\displaystyle g \circ f: V(G) \to V(K)}$: это биекция, так как композиция двух биекций - биекция.
Сохранение ребер:
$$\displaylines{
\begin{aligned}
&\text{ Если } (u, \  v) \in  E(G) \to  (f(u), \  f(v)) \in  E(H) \\
&\text{ Если } (f(u), \  f(v)) \in  E(H) \to  (g(f(u)), \   g(f(v))) \in  E(K) \\
& \text{ Следовательно, из } (u, \  v) \in E(G) \implies (g(f(u)), \  g(f(v))) \in  E(K) 
\end{aligned}
}$$
Итого: ${\displaystyle g \circ f}$ - изоморфизм между ${\displaystyle G}$ и ${\displaystyle K \implies G \cong K}$.

В итоге, изоморфизм обладает свойствами 1, 2, 3, следовательно изоморфизм графов является отношением эквивалентности на множестве всех графов.

---
### Задание 5. 
Графы ${\displaystyle G}$ и ${\displaystyle H}$ изоморфны, если существует биекция ${\displaystyle \varphi: V(G) \to V(H)}$, что ${\displaystyle \forall{a, \ b} \in V(G): (a, \ b) \in E(G) \iff (\varphi(a), \ \varphi(b)) \in E(H)}$. Доказать, что ${\displaystyle \psi: E(G) \to E(H)}$ тоже будет биекцией.
Доказательство:
1. Инъективность ${\displaystyle \psi}$:
Чтобы показать, что ${\displaystyle \psi}$ - инъекция, надо доказать, что если ${\displaystyle \psi(e_{ 1 }) = \psi(e_{ 2 })}$ для каких то ребер ${\displaystyle e_{ 1 }, \ e_{ 2 } \in E(G)}$, то ${\displaystyle e_{ 1 } = e_{ 2 }}$.
Пусть ${\displaystyle e_{ 1 } = (a, \ b), \ e_{ 2 } = (c, \ d)}$ - два ребра в ${\displaystyle G}$. Предположим, что ${\displaystyle \psi(e_{ 1 }) = \psi(e_{ 2 })}$, то есть ${\displaystyle (\varphi(a), \ \varphi(b)) = (\varphi(c), \ \varphi(d))}$. Так как ${\displaystyle \varphi}$ - биекция, то есть и инъекция, значит из этого равенства следует, что ${\displaystyle \varphi(a) = \varphi(c) \implies a = c}$ и ${\displaystyle \varphi(b) = \varphi(d) \implies b = d}$. 
Таким образом, ${\displaystyle e_{ 1 } = e_{ 2 } = (a, \ b) = (c, \ d)}$.
2. Сюръективность ${\displaystyle \psi}$:
Чтобы показать, что ${\displaystyle \psi}$ - сюръекция, надо доказать, что ${\displaystyle \forall{}}$ ребра ${\displaystyle h \in E(H)}$ существует ребро ${\displaystyle e \in E(G)}$, такое что ${\displaystyle \psi(e) = h}$.
Пусть ${\displaystyle h = (x, \ y) \in E(H)}$. Так как ${\displaystyle \varphi: V(G) \to V(H)}$ биекция, то есть и сюръекция, значит ${\displaystyle \exists a, \ b \in V(G): \varphi(a) = x, \ \varphi(b) = y}$. По условию изоморфизма:
$$\displaylines{
(x, \  y) = (\varphi(a), \  \varphi(b)) \in  E(H) \implies  (a, \  b) \in  E(G) \\
e = (a, \  b) \in  E(G), \  \text{ тогда: } \\
\psi(e) = \psi((a, \  b)) = (\varphi(a), \  \varphi(b)) = (x, \  y) = h
}$$
Таким образом, ${\displaystyle \forall{h} \in E(H) \ \exists e \in E(G): \psi(e) = h}$.

---
### Задание 6. 
Доказать, что если графы ${\displaystyle G}$ и ${\displaystyle H}$ изоморфны, то их дополнения ${\displaystyle \overline{G}}$ и ${\displaystyle \overline{H}}$ тоже будут изоморфными.
Доказательство:
Надо найти биекцию ${\displaystyle \psi: V(\overline{G}) \to V(\overline{H}): (a, \ b) \in E(\overline{G}) \iff (\psi(a), \ \psi(b)) \in E(\overline{H})}$.
Так как ${\displaystyle G \cong H \implies \exists }$ биекция ${\displaystyle \varphi: V(G) \to V(H): (a, \ b) \in E(G) \iff (\varphi(a), \ \varphi(b)) \in E(H)}$. ${\displaystyle V(\overline{G}) = V(G), \ V(\overline{H}) = V(H)}$. Значит мы можем использовать ту же биекцию ${\displaystyle \varphi: V(\overline{G}) \to V(\overline{H})}$.
Проверим сохранение ребер в дополнениях:
$$\displaylines{
\begin{aligned}
& \forall{a, \  b} \in  V(\overline{G}) \text{ надо доказать, что } (a, \  b) \in  E(\overline{G}) \iff  (\varphi(a), \  \varphi(b)) \in  E(\overline{H}): \\
& 1. \ (a, \  b) \in E(\overline{G}) \iff  (a, \  b) \cancel{\in } E(G), \  \\
& 2. \ (\varphi(a), \  \varphi(b)) \in  E(\overline{H}) \iff  (\varphi(a), \  \varphi(b)) \cancel{\in } E(H). \\ 
&\text{Подставляем: } \\
&  (a, \  b) \in  E(\overline{G}) \iff  (a, \  b) \cancel{\in } E(G) \iff (\varphi(a), \  \varphi(b)) \cancel{\in } E(H) \iff (\varphi(a), \  \varphi(b)) \in  E(\overline{H})
\end{aligned}
}$$
Значит, биекция ${\displaystyle \varphi}$ также сохраняет структуру ребер между ${\displaystyle \overline{G}}$ и ${\displaystyle \overline{H} \implies \overline{G} \cong \overline{H}}$.

---
### Задание 7. 
Какие из следующих графов являются двудольными:
$$\displaylines{
\overline{C_{ 5 }}, \  \overline{2C_{ 4 }}, \  \overline{K_{ 5 } + K_{ 6 }}, \  \overline{2K_{ 2 } \circ 2K_{ 2 }}?
}$$
1. ${\displaystyle \overline{C_{ 5 }}}$  - есть нечетный цикл длинны 5, значит не двудольный.
```tikz
\begin{document}

\begin{tikzpicture}[scale=1.2]
    \node[circle, draw, minimum size=8mm, font=\large] (1) at (-2, 0.5) {$1$};
    \node[circle, draw, minimum size=8mm, font=\large] (2) at (0, 2) {$2$};
    \node[circle, draw, minimum size=8mm, font=\large] (3) at (2, 0.5) {$3$};
    \node[circle, draw, minimum size=8mm, font=\large] (4) at (1.5, -2) {$4$};
    \node[circle, draw, minimum size=8mm, font=\large] (5) at (-1.5, -2) {$5$};
    
    \draw[thick] (1) -- (3);
    \draw[thick] (3) -- (5);
    \draw[thick] (5) -- (2);
    \draw[thick] (2) -- (4);
    \draw[thick] (4) -- (1);
\end{tikzpicture}

\end{document}
```
2. В ${\displaystyle \overline{2C_{ 4 }}}$ есть циклы нечетной длинны, например ${\displaystyle  1  -  5 - 4 -1}$, значит не двудольный.
```tikz
\begin{document}
\begin{tikzpicture}[scale=2]

    \node[circle, draw, minimum size=8mm, font=\large] (v1) at (0, 2) {$1$};
    \node[circle, draw, minimum size=8mm, font=\large] (v2) at (2, 3) {$2$};
    \node[circle, draw, minimum size=8mm, font=\large] (v3) at (0, 0) {$3$};
    \node[circle, draw, minimum size=8mm, font=\large] (v4) at (2, -1) {$4$};
    
    \node[circle, draw, minimum size=8mm, font=\large] (v5) at (5, 3) {$5$};
    \node[circle, draw, minimum size=8mm, font=\large] (v6) at (7, 2) {$6$};
    \node[circle, draw, minimum size=8mm, font=\large] (v7) at (5, -1) {$7$};
    \node[circle, draw, minimum size=8mm, font=\large] (v8) at (7, 0) {$8$};

    % Все рёбра между группами (K_{4,4})
    \foreach \i in {1, 2, 3, 4} {
        \foreach \j in {5, 6, 7, 8} {
            \draw[thick] (v\i) -- (v\j);
        }
    }
            \draw[thick] (v1) -- (v4);
            \draw[thick] (v3) -- (v2);
            \draw[thick] (v5) -- (v8);
            \draw[thick] (v6) -- (v7);
\end{tikzpicture}
\end{document}
```
3. ${\displaystyle \overline{K_{ 5 } + K_{ 6 }}}$ - полный двудольный граф ${\displaystyle K_{ 5, \ 6 }}$.
```tikz
\begin{document}
\begin{tikzpicture}[scale=3]
    \foreach \i in {1, 2, 3, 4, 5} {
        \node[circle, draw, minimum size=8mm, font=\large] (v\i) at (2+\i, 1) {$\i$};
    }

    \foreach \i in {6, 7, 8, 9, 10, 11} {
        \node[circle, draw, minimum size=8mm, font=\large] (v\i) at (\i-3.5, -1) {$\i$};
    }

    \foreach \i in {1, 2, 3, 4, 5} {
        \foreach \j in {6, 7, 8, 9, 10, 11} {
            \draw[thick] (v\i) -- (v\j);
        }
    }
\end{tikzpicture}
\end{document}
```

4. ${\displaystyle \overline{2K_{ 2 } \circ 2K_{ 2 }}}$ - два четных цикла длинны 4, значит двудольный:
```tikz
\begin{document}
\begin{tikzpicture}[scale = 2]

\begin{scope}[local bounding box=original]
    \node[circle, draw, minimum size=8mm, font=\large] (1) at (0,0) {$1$};
    \node[circle, draw, minimum size=8mm, font=\large] (2) at (2,0) {$3$};
    \node[circle, draw, minimum size=8mm, font=\large] (3) at (2,-2) {$2$};
    \node[circle, draw, minimum size=8mm, font=\large] (4) at (0,-2) {$4$};
    
    \draw[thick] (1) -- (2);
    \draw[thick] (2) -- (3);
    \draw[thick] (3) -- (4);
    \draw[thick] (4) -- (1);
    
\end{scope}

\begin{scope}[local bounding box=line, xshift=4cm]
    \node[circle, draw, minimum size=8mm, font=\large] (ab) at (0,0)  {$5$};
    \node[circle, draw, minimum size=8mm, font=\large] (bc) at (2,0)  {$7$};
    \node[circle, draw, minimum size=8mm, font=\large] (cd) at (2,-2) {$8$};
    \node[circle, draw, minimum size=8mm, font=\large] (da) at (0,-2) {$6$};
    
    \draw[thick] (ab) -- (bc);
    \draw[thick] (bc) -- (cd);
    \draw[thick] (cd) -- (da);
    \draw[thick] (da) -- (ab);

\end{scope}

\end{tikzpicture}
\end{document}
```
Итого: двудольные 3, 4.

---
### Задание 8.
Какие из следующих графов являются планарными:
$$\displaylines{
\overline{C_{ 5 } + K_{ 1 }}, \   \overline{K_{ 3 } + K_{ 4 }}, \   \overline{3K_{ 2 }}, \   \overline{K_{ 1 } \circ \overline{K_{ 5 }}}?
}$$
1. ${\displaystyle \overline{C_{ 5 } + K_{ 1 }}}$ является планарным, плоская укладка:
```tikz
\begin{document}

\begin{tikzpicture}[scale=1.2]
    \node[circle, draw, minimum size=8mm, font=\large] (1) at (-3, 0) {$1$};
    \node[circle, draw, minimum size=8mm, font=\large] (2) at (2, -3) {$2$};
    \node[circle, draw, minimum size=8mm, font=\large] (3) at (0, 2) {$3$};
    \node[circle, draw, minimum size=8mm, font=\large] (4) at (-2, -3) {$4$};
    \node[circle, draw, minimum size=8mm, font=\large] (5) at (3, 0) {$5$};
    \node[circle, draw, minimum size=8mm, font=\large] (6) at (0, -0.5) {$6$};
    
    \draw[thick] (1) -- (3);
    \draw[thick] (3) -- (5);
    \draw[thick] (5) -- (2);
    \draw[thick] (2) -- (4);
    \draw[thick] (4) -- (1);
    \draw[thick] (1) -- (6);
    \draw[thick] (3) -- (6);
    \draw[thick] (5) -- (6);
    \draw[thick] (2) -- (6);
    \draw[thick] (4) -- (6);

    
\end{tikzpicture}

\end{document}
```
2. ${\displaystyle \overline{K_{ 3 } + K_{ 4 }} }$ - содержит подграф ${\displaystyle K_{ 3, \ 3 }}$, значит граф не планарен.
```tikz
\begin{document}

\begin{tikzpicture}[scale=1.2]
    \node[circle, draw, minimum size=8mm, font=\large] (1) at (0, 1) {$1$};
    \node[circle, draw, minimum size=8mm, font=\large] (2) at (4, 1) {$2$};
    \node[circle, draw, minimum size=8mm, font=\large] (3) at (-4, 1) {$3$};
    \node[circle, draw, minimum size=8mm, font=\large] (4) at (-4, -2) {$4$};
    \node[circle, draw, minimum size=8mm, font=\large] (5) at (4, -2) {$5$};
    \node[circle, draw, minimum size=8mm, font=\large] (6) at (0, 3) {$6$};
    \node[circle, draw, minimum size=8mm, font=\large] (7) at (0, -2) {$7$};
    
    \draw[thick] (1) -- (6);
    \draw[thick] (6) -- (2);
    \draw[thick] (6) -- (3);
    \draw[thick] (3) -- (4);
    \draw[thick] (1) -- (7);
    \draw[thick] (2) -- (5);
    \draw[thick] (2) -- (7);
    \draw[thick] (2) -- (4);
    \draw[thick] (3) -- (7);
    \draw[thick] (3) -- (5);
    \draw[thick] (1) -- (4);
    \draw[thick] (1) -- (5);

    
\end{tikzpicture}

\end{document}
```
2. ${\displaystyle \overline{3K_{ 2 }}}$ планарный, плоская укладка:
```tikz
\begin{document}

\begin{tikzpicture}[scale=1.2]
    \node[circle, draw, minimum size=8mm, font=\large] (1) at (1, -1) {$1$};
    \node[circle, draw, minimum size=8mm, font=\large] (2) at (4, -3) {$2$};
    \node[circle, draw, minimum size=8mm, font=\large] (3) at (0, 1) {$3$};
    \node[circle, draw, minimum size=8mm, font=\large] (4) at (-4, -3) {$4$};
    \node[circle, draw, minimum size=8mm, font=\large] (5) at (0, 3) {$5$};
    \node[circle, draw, minimum size=8mm, font=\large] (6) at (-1, -1) {$6$};
    
    \draw[thick] (5) -- (2);
    \draw[thick] (2) -- (4);
    \draw[thick] (4) -- (5);
    \draw[thick] (5) -- (3);
    \draw[thick] (3) -- (2);
    \draw[thick] (3) -- (1);
    \draw[thick] (1) -- (4);
    \draw[thick] (1) -- (6);
    \draw[thick] (6) -- (4);
    \draw[thick] (6) -- (3);

    
\end{tikzpicture}

\end{document}
```
4. ${\displaystyle \overline{K_{ 1 } \circ \overline{K_{ 5 }}}}$ не планарен, так как содержит подграф ${\displaystyle K_{ 5 }}$.
```tikz
\begin{document}

\begin{tikzpicture}[scale=1.2]
    \node[circle, draw, minimum size=8mm, font=\large] (1) at (-2, 0.5) {$1$};
    \node[circle, draw, minimum size=8mm, font=\large] (2) at (0, 2) {$2$};
    \node[circle, draw, minimum size=8mm, font=\large] (3) at (2, 0.5) {$3$};
    \node[circle, draw, minimum size=8mm, font=\large] (4) at (1.5, -2) {$4$};
    \node[circle, draw, minimum size=8mm, font=\large] (5) at (-1.5, -2) {$5$};
    \node[circle, draw, minimum size=8mm, font=\large] (0) at (-4, 0) {$0$};
    
    \draw[thick] (1) -- (2) -- (3) -- (4) -- (5) -- (1);
    \draw[thick] (1) -- (3);
    \draw[thick] (3) -- (5);
    \draw[thick] (5) -- (2);
    \draw[thick] (2) -- (4);
    \draw[thick] (4) -- (1);
\end{tikzpicture}
\end{document}
```
Итого: планарные графы 1, 3.

---
### Задание 9. 
Пусть ${\displaystyle D = (d_{ 1 }, \ d_{ 2 }, \ \dots, \ d_{ n })}$ - набор степеней вершин самодополнительного графа ${\displaystyle G}$. Доказать, что 
$$\displaylines{
d_{ i } = n-1 - d_{ n+1-i}, \  \quad    i =1, \  2, \  \dots , \  \left\lfloor  \frac{n}{2} \right\rfloor 
}$$
Доказательство:
Пусть ${\displaystyle d_{ 1 }\geq d_{ 2 }\geq\dots\geq d_{ n }}$ - упорядоченная последовательность степеней вершин ${\displaystyle G}$. Для ${\displaystyle \overline{G}}$ степени вершин равны: ${\displaystyle n-1-d_{ n }\leq n-1-d_{ n-1 } \leq \dots \leq n-1-d_{ 1 }}$.
Так как ${\displaystyle G \cong \overline{G}}$ их последовательности должны совпадать с точностью до перестановки. Так как обе последовательности уже упорядочены, они должны быть идентичными:
$$\displaylines{
d_{ 1 }\geq d_{ 2 }\geq \dots \geq d_{ n } = n-1-d_{ n }\leq n-1-d_{ n-1 } \leq \dots \leq n-1-d_{ 1 }
}$$
Для выполнения этого равенства необходимо, чтобы ${\displaystyle d_{ i } = n-1 - d_{ n+1-i }, \  i =1, \  2, \  \dots , \  \left\lfloor  \frac{n}{2} \right\rfloor }$.
Пусть ${\displaystyle n = 2k}$, тогда имеем ${\displaystyle k}$ пар:
$$\displaylines{
\begin{aligned}
& d_{ 1 } = n-1-d_{ n } \\
& d_{ 2 } = n-1-d_{ n-1 } \\
& \vdots \\
& d_{ k } = n-1-d_{ k+1 } \\
\end{aligned}
}$$
Пусть ${\displaystyle n = 2k+1}$, тогда: имеем ${\displaystyle k}$ пар, центральная вершина ${\displaystyle d_{ k+1 }}$ должна удовлетворять ${\displaystyle d_{ k+1 } = n-1 - d_{ k+1 } \implies d_{ k+1 } = \frac{n-1}{2}}$.
Изоморфизм ${\displaystyle \varphi: G \to \overline{G}}$ отображает вершину ${\displaystyle v_{ i }}$ со степенью ${\displaystyle d_{ i }}$ в вершину ${\displaystyle \varphi(v_{ i })}$ со степень ${\displaystyle n-1-d_{ i }}$, чтобы сохранить порядок степеней, вершина ${\displaystyle v_{ i }}$ должна соответствовать вершине ${\displaystyle v_{ n+1-i }}$, что и дает ${\displaystyle d_{ i } = n-1 - d_{ n+1-i }}$.

---
### Задание 10. 
Реберным графом ${\displaystyle L(G)}$ для неориентированного графа ${\displaystyle G}$ называется граф, который имеет множество вершин, взаимнооднозначно соответствующих множеству ребер графа ${\displaystyle G}$, причем две вершины смежны тогда и только тогда, когда соответствующие им ребра в ${\displaystyle G}$ смежны. Привести пример графа ${\displaystyle G}$, для которого выполнимо ${\displaystyle L(G) \cong G}$.

Решение: рассмотрим цикл ${\displaystyle C_{ n }}$, для любого ${\displaystyle n\geq3}$ выполняется ${\displaystyle L(C_{ n }) = C_{ n }}$.
${\displaystyle C_{ n }}$ имеет ${\displaystyle n}$ вершин и ${\displaystyle n}$ ребер, каждое ребро соединяет две соседние вершины. Каждое ребро ${\displaystyle e_{ i }}$ в ${\displaystyle C_{ n }}$ становится вершиной ${\displaystyle v_{ i }}$ в ${\displaystyle L(C_{ n })}$. Две вершины ${\displaystyle v_{ i }, \ v_{ j }}$ в ${\displaystyle L(C_{ n })}$ соединены ребром, когда соответствующие им ребра ${\displaystyle e_{ i }, \ e_{ j }}$ в ${\displaystyle C_{ n }}$ имеют общую вершину.
В цикле каждое ребро смежно ровно с двумя соседними по циклу ребрами, поэтому реберный граф ${\displaystyle L(C_{ n })}$ также образует цикл из ${\displaystyle n}$ вершин, что изоморфно ${\displaystyle G}$.
Пример, для ${\displaystyle n = 4}$:
```tikz
\begin{document}
\begin{tikzpicture}[scale = 2]

\begin{scope}[local bounding box=original]
    \node[circle, draw, minimum size=8mm, font=\large] (a) at (0,0) {$a$};
    \node[circle, draw, minimum size=8mm, font=\large] (b) at (2,0) {$b$};
    \node[circle, draw, minimum size=8mm, font=\large] (c) at (2,-2) {$c$};
    \node[circle, draw, minimum size=8mm, font=\large] (d) at (0,-2) {$d$};
    
    \draw[thick] (a) -- (b) node[above, sloped, pos = 0.5, font=\large] {$(a,b)$};
    \draw[thick] (b) -- (c) node[above, sloped, pos = 0.5, font=\large] {$(b,c)$};
    \draw[thick] (c) -- (d) node[above, sloped, pos = 0.5, font=\large] {$(d,c)$};
    \draw[thick] (d) -- (a) node[above, sloped, pos = 0.5, font=\large] {$(d,a)$};
    
\end{scope}

\begin{scope}[local bounding box=line, xshift=4cm]
    \node[circle, draw, minimum size=8mm, font=\large] (ab) at (0,0)  {$(a,b)$};
    \node[circle, draw, minimum size=8mm, font=\large] (bc) at (2,0)  {$(b,c)$};
    \node[circle, draw, minimum size=8mm, font=\large] (cd) at (2,-2) {$(d,c)$};
    \node[circle, draw, minimum size=8mm, font=\large] (da) at (0,-2) {$(d,a)$};
    
    \draw[thick] (ab) -- (bc);
    \draw[thick] (bc) -- (cd);
    \draw[thick] (cd) -- (da);
    \draw[thick] (da) -- (ab);

\end{scope}

\end{tikzpicture}
\end{document}
```

