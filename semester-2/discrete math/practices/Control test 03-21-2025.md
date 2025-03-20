Задание 1.
Граф ${\displaystyle G}$ задан матрицей смежности:
$$\displaylines{
\begin{matrix}
\ \ \ \   v_{ 1 } \ \  v_{ 2 } \ \  v_{ 3 } \ \  v_{ 4 } \ \   v_{ 5 }  \ \   v_{ 6 } \ \  v_{ 7 } \ \  v_{ 8 }
\end{matrix}\\ \begin{matrix}
v_{ 1 } \\
v_{ 2 } \\
v_{ 3 } \\
v_{ 4 } \\
v_{ 5 } \\
v_{ 6 } \\
v_{ 7 } \\
v_{ 8 }
\end{matrix}\begin{pmatrix}
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
2. Найти ${\displaystyle \text{ diam}(G), \ \text{ rad}(G), \ \text{ Center}(G)}$.назовём
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
    \node[circle, draw, minimum size=8mm, font=\large] (v2) at (0, 3) {$v_2$};
    \node[circle, draw, minimum size=8mm, font=\large] (v3) at (-3, -3) {$v_3$}; % Перемещена в левый низ
    \node[circle, draw, minimum size=8mm, font=\large] (v4) at (0, 0) {$v_4$};
    \node[circle, draw, minimum size=8mm, font=\large] (v5) at (3, 0) {$v_5$};
    \node[circle, draw, minimum size=8mm, font=\large] (v6) at (0, -3) {$v_6$};
    \node[circle, draw, minimum size=8mm, font=\large] (v7) at (3, -3) {$v_7$};
    \node[circle, draw, minimum size=8mm, font=\large] (v8) at (6, -3) {$v_8$};

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

2. По данному графу построит таблицу расстояний:
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

3. По теореме Понтрягина-Куратовского граф ${\displaystyle G}$ не планарен, если он содержит подграф, являющийся подразбиением ${\displaystyle K_{ 5 }}$ или ${\displaystyle K_{ 3, 3 }}$.
Рассмотрим вершины ${\displaystyle \{ v_{ 2 }, \ v_{ 4 }, \ v_{ 5 } \}}$ и ${\displaystyle \{ v_{ 3 }, \ v_{ 6 }, \ v_{ 7 } \}}$. Это подграф является подразбиением ${\displaystyle K_{ 3,3 }}$, так как все ребра между долями либо присутствуют, либо могут быть заменены путями длинны 2. Следовательно, граф не планарен.

4. Граф ${\displaystyle G}$ самодополнителен, если он изоморфен дополнению ${\displaystyle \overline{G}}$.
В нашем графе ${\displaystyle |V| = 8, \ |E| = 14}$. Для самодополнительного графа ${\displaystyle \overline{G}}$ с ${\displaystyle n}$ вершинами ${\displaystyle |E| = \frac{n(n-1)}{4}}$. 
$$\displaylines{
|E| = \frac{8(8-1)}{4}  \\
14 = 14
}$$
Необходимое условие выполнилось.
Построим его:
```tikz
\begin{document}

\begin{tikzpicture}[scale=1.2]
    % Определение вершин
    \node[circle, draw, minimum size=8mm, font=\large] (v1) at (-3, 3) {$v_1$};
    \node[circle, draw, minimum size=8mm, font=\large] (v2) at (0, 3) {$v_2$};
    \node[circle, draw, minimum size=8mm, font=\large] (v3) at (-3, -3) {$v_3$};
    \node[circle, draw, minimum size=8mm, font=\large] (v4) at (-1, 0) {$v_4$};
    \node[circle, draw, minimum size=8mm, font=\large] (v5) at (3, 1) {$v_5$};
    \node[circle, draw, minimum size=8mm, font=\large] (v6) at (0, -2) {$v_6$};
    \node[circle, draw, minimum size=8mm, font=\large] (v7) at (3, -2) {$v_7$};
    \node[circle, draw, minimum size=8mm, font=\large] (v8) at (6, -3) {$v_8$};

    % Рисование рёбер для \overline{G}
    \draw[thick] (v1) -- (v3);
    \draw[thick] (v1) -- (v5);
    \draw[thick] (v1) -- (v6);
    \draw[thick] (v1) -- (v7);
    \draw[thick] (v1) -- (v8);
    \draw[thick] (v2) -- (v6);
    \draw[thick] (v2) -- (v7);
    \draw[thick] (v2) -- (v8);
    \draw[thick] (v3) -- (v4);
    \draw[thick] (v3) -- (v7);
    \draw[thick] (v3) -- (v8);
    \draw[thick] (v4) -- (v8);
    \draw[thick] (v5) -- (v6);
    \draw[thick] (v6) -- (v8);
\end{tikzpicture}

\end{document}
```

Можно заметить, что вершина ${\displaystyle v_{ 1 }}$ имеет 5 смежных вершин, когда у ${\displaystyle G \ \max_{ v_{ i } \in V } \deg(v_{ i }) = 4}$, значит нельзя с помощью перестановок вершин в ${\displaystyle \overline{G}}$ получить ${\displaystyle G}$. Следовательно граф ${\displaystyle \overline{G} \cancel{\cong} G}$ и граф ${\displaystyle G}$ не является самодополнительным.

Задание 2.
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
