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

2. ${\displaystyle \text{diam}(G) = \max_{ x \in  V } \max_{ y \in V } d(x, \  y)}$. 