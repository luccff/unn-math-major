Дано отношение R на множестве A. Определите, является ли оно симметричным, антисимметричным, транзитивным, отношением эквивалентности, отношением порядка. Для отношения эквивалентности найдите классы эквивалентности, для отношения порядка – минимальные и максимальные элементы.

---
$$\displaylines{
20) \ xRy \iff 5x \geq 3y; \\
a) \ A = \{ 6,7,8,9,10 \} \\
}$$
1.Рефлексивность(${\forall{x}\in A \hookrightarrow xRx}$): $$\displaylines{
\forall{x} \in A \ \ \ 5x\geq 3x \implies 2x\geq 0 \implies R - \text{ рефлексивно}
}$$2.Cимметричность(${ \forall{x, y \in A} \ xRy\implies yRx}$):
$$\displaylines{
\forall{x, y \in A} \hookrightarrow 5x\geq3y, \ 5y\geq3x \implies R - \text{симметрично }
}$$

3.Антисимметричность(${ \forall{x, y \in A}\ \ xRy \wedge yRx \implies x = y}$): $$\displaylines{
\text{Пусть }  x = 6 \text{ и } y = 7: \\
xRy: 30\geq21 \\
yRx: 35\geq18 \\
x \neq y \implies R - \text{ не антисимметрично }
}$$4.Транзитивность(${\forall{x,y,z \in A} \ xRy \wedge yRz \implies xRz}$): $$\displaylines{
\text{ Пусть } xRy \text{ и } yRz: 5x\geq3y \text{ и } 5y\geq3z \\
25x \geq 15y, \ 15y \geq 9z \hookrightarrow25x\geq9z \implies 5x \geq \frac{9}{5}z \\
\frac{9}{5}z < 3x \implies 5x\geq3z \implies R - \text{ транзитивно }
}$$5.Отношение эквивалентности(если R - рефлексивно, симметрично и транзитивно): $$\displaylines{
\text{ В силу } 1, 2, 4 \ R - \text{ отношение эквивалентности } \\
[x] = \{ y \in A \ | \ xRy \}
}$$6.Отношение порядка:$$\displaylines{
\text{ R - транзитивно и рефлексивно } \implies \text{ квазипорядок на } A
}$$
---
$$\displaylines{
b) \ A = \{ 0,1,2,4,7 \}
}$$

1.Рефлексивность(${\forall{x}\in A \hookrightarrow xRx}$):$$\displaylines{
\forall{x} \in A \ \ \ 5x\geq 3x \implies 2x\geq 0 \implies R - \text{ рефлексивно}
}$$2.Cимметричность(${ \forall{x, y \in A} \ xRy\implies yRx}$): $$\displaylines{
\text{ Пусть } x = 7, \ y = 2:\\
xRy:35\geq6 \\
yRx: 10\geq21\\
\implies R - \text{ не симметрично }
}$$3.Антисимметричность(${ \forall{x, y \in A}\ \ xRy \wedge yRx \implies x = y}$): $$\displaylines{
5x+5y \geq 3y+ 3x \implies x\geq y \implies x = y
}$$4.Транзитивность(${\forall{x,y,z \in A} \ xRy \wedge yRz \implies xRz}$): $$\displaylines{
\text{ Пусть } xRy \text{ и } yRz: 5x\geq3y \text{ и } 5y\geq3z \\
25x \geq 15y, \ 15y \geq 9z \hookrightarrow25x\geq9z \implies 5x \geq \frac{9}{5}z \\
\frac{9}{5}z < 3x \implies 5x\geq3z \implies R - \text{ транзитивно }
}$$5.Отношение эквивалентности(если R - рефлексивно, симметрично и транзитивно): $$\displaylines{
\text{ В силу } 2 \ R - \text{ не отношение эквивалентности }
}$$6.Отношение порядка:$$\displaylines{
\text{ R - рефлексивно, антисимметрично  и транзитивно } \implies \text{ оно является }\\ \text{ отношением частичного порядка на }A
}$$7.Максимальные и минимальные элементы:$$\displaylines{
\text{ Максимальный: }0 \iff \cancel\exists x\in A:0Rx, \ x\neq0 \\
\text{ Минимальный: }7 \iff \forall{y \in A} \hookrightarrow 7Ry, \ y \neq 7 \text{ и } \cancel\exists x \in A:xR7, \ x\neq7
}$$