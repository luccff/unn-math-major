## Предел функции нескольких переменных по множеству
### Определение предела по множеству
Рассмотрим функцию $f: D \to \mathbb{R}$, где $D \subset \mathbb{R}^n$, и точку $M_0 \in \mathbb{R}^n$, которая является предельной точкой множества $D \subset \mathbb{R}^n$. Пусть $E \subset D$ — некоторое подмножество, такое что $M_0$ является предельной точкой $E$.

**Определение.**
Функция $f$ имеет предел $A \in \mathbb{R}$ по множеству $E$ при $M \to M_0$, если
$$
\lim_{M \to M_0, M \in E} f(M) = A \iff \forall \varepsilon > 0 \quad \exists \delta > 0 : \forall M \in E, \ 0 < \rho(M, M_0) < \delta \implies |f(M) - A| < \varepsilon,
$$
где $\rho(M, M_0) = \sqrt{\sum_{i=1}^n (x_i - x_i^0)^2}$ — евклидова метрика, $M = (x_1, \ldots, x_n)$, $M_0 = (x_1^0, \ldots, x_n^0)$.

**Геометрическое пояснение.**  
Предел по множеству $E$ означает, что функция $f(M)$ стремится к $A$, когда $M$ приближается к $M_0$, оставаясь в множестве $E$. Это ограничивает пути приближения к $M_0$ только теми, которые лежат в $E$. Если $E = D$, то это обычный предел функции. Если $E$ — подмножество, например, кривая или плоскость, то предел рассматривается только вдоль точек этого подмножества.

**Замечание.**  
Для существования предела $\lim_{M \to M_0} f(M)$ необходимо, чтобы пределы по всем возможным подмножествам $E \subset D$, для которых $M_0$ — предельная точка, совпадали. Если пределы по разным множествам различны, то общий предел функции в точке $M_0$ не существует.

### Примеры функций с разными пределами по различным множествам
Рассмотрим функции двух переменных ($n = 2$) в точке $M_0 = (0, 0)$, чтобы показать, как пределы по различным множествам могут отличаться, что приводит к отсутствию общего предела.

#### Пример 1
Функция:
$$
f(x, y) = \frac{xy}{x^2 + y^2}, \quad (x, y) \neq (0, 0), \quad f(0, 0) = 0.
$$
Область определения: $D = \mathbb{R}^2$.

**По множеству $E_1 = \{ (x, 0) \mid x \neq 0 \}$ (ось $Ox$).**  
Подставим $y = 0$:
$$
f(x, 0) = \frac{x \cdot 0}{x^2 + 0^2} = 0.
$$
Тогда $\lim_{x \to 0, (x, 0) \in E_1} f(x, 0) = 0$.

**По множеству $E_2 = \{ (0, y) \mid y \neq 0 \}$ (ось $Oy$).**  
Подставим $x = 0$:
$$
f(0, y) = \frac{0 \cdot y}{0^2 + y^2} = 0.
$$
Тогда $\lim_{y \to 0, (0, y) \in E_2} f(0, y) = 0$.

**По множеству $E_3 = \{ (x, x) \mid x \neq 0 \}$ (прямая $y = x$).**  
Подставим $y = x$:
$$
f(x, x) = \frac{x \cdot x}{x^2 + x^2} = \frac{x^2}{2x^2} = \frac{1}{2}.
$$
Тогда $\lim_{x \to 0, (x, x) \in E_3} f(x, x) = \frac{1}{2}$.

**По множеству $E_4 = \{ (x, kx) \mid x \neq 0, k \in \mathbb{R} \}$ (прямая $y = kx$).**  
Подставим $y = kx$:
$$
f(x, kx) = \frac{x \cdot kx}{x^2 + (kx)^2} = \frac{kx^2}{x^2 + k^2 x^2} = \frac{k}{1 + k^2}.
$$
Тогда $\lim_{x \to 0, (x, kx) \in E_4} f(x, kx) = \frac{k}{1 + k^2}$, что зависит от $k$. Например, при $k = 1$: $\frac{1}{1 + 1} = \frac{1}{2}$; при $k = 0$: $\frac{0}{1 + 0} = 0$.

**Вывод.**  
Пределы по множествам $E_1$ и $E_2$ равны 0, по $E_3$ — $\frac{1}{2}$, а по $E_4$ зависят от $k$. Поскольку пределы по разным множествам различны, общий предел $\lim_{(x, y) \to (0, 0)} f(x, y)$ не существует.

#### Пример 2
Функция:
$$
f(x, y) = \frac{x^2 y}{x^4 + y^2}, \quad (x, y) \neq (0, 0), \quad f(0, 0) = 0.
$$
Область определения: $D = \mathbb{R}^2$.

**По множеству $E_1 = \{ (x, 0) \mid x \neq 0 \}$ (ось $Ox$).**  
$$
f(x, 0) = \frac{x^2 \cdot 0}{x^4 + 0^2} = 0.
$$
Тогда $\lim_{x \to 0, (x, 0) \in E_1} f(x, 0) = 0$.

**По множеству $E_2 = \{ (x, x^2) \mid x \neq 0 \}$ (парабола $y = x^2$).**  
Подставим $y = x^2$:
$$
f(x, x^2) = \frac{x^2 \cdot x^2}{x^4 + (x^2)^2} = \frac{x^4}{x^4 + x^4} = \frac{x^4}{2x^4} = \frac{1}{2}.
$$
Тогда $\lim_{x \to 0, (x, x^2) \in E_2} f(x, x^2) = \frac{1}{2}$.

**По множеству $E_3 = \{ (x, kx^2) \mid x \neq 0, k \in \mathbb{R} \}$ (парабола $y = kx^2$).**  
Подставим $y = kx^2$:
$$
f(x, kx^2) = \frac{x^2 \cdot kx^2}{x^4 + (kx^2)^2} = \frac{kx^4}{x^4 + k^2 x^4} = \frac{k}{1 + k^2}.
$$
Тогда $\lim_{x \to 0, (x, kx^2) \in E_3} f(x, kx^2) = \frac{k}{1 + k^2}$, что зависит от $k$. Например, при $k = 1$: $\frac{1}{1 + 1} = \frac{1}{2}$; при $k = 0$: $\frac{0}{1 + 0} = 0$.

**Вывод.**  
Предел по $E_1$ равен 0, по $E_2$ — $\frac{1}{2}$, по $E_3$ зависит от $k$. Различные пределы по разным множествам указывают на отсутствие общего предела $\lim_{(x, y) \to (0, 0)} f(x, y)$.