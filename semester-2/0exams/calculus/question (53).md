**Различные метрики.**  
В $\mathbb{R}^n$ сходимость последовательности не зависит от выбора метрики. Например, для точек $A = (a_1, \ldots, a_n)$, $B = (b_1, \ldots, b_n)$ возможны метрики:
$$\displaylines{
\rho_1(A, B) = \sqrt{\sum_{i=1}^n (a_i - b_i)^2}, \\ \rho_2(A, B) = \sum_{i=1}^n |a_i - b_i|, \ \\ \rho_3(A, B) = \max_{i=1,\ldots,n} |a_i - b_i|.
}$$
Сходимость эквивалентна для всех этих метрик (в силу эквивалентности норм в $\mathbb{R}^n$).

Норма в $\mathbb{R}^n$ — это функция $\| \cdot \|: \mathbb{R}^n \to \mathbb{R}$, которая измеряет "длину" вектора $x = (x_1, \ldots, x_n)$ и удовлетворяет аксиомам: неотрицательности ($\|x\| \geq 0$, $\|x\| = 0 \iff x = 0$), однородности ($\|\lambda x\| = |\lambda| \|x\|$) и неравенства треугольника ($\|x + y\| \leq \|x\| + \|y\|$). 
### Основная теорема: сходимость по координатам

**Теорема.**  
Последовательность $\{ M_k \}_{k \geq 1}$, где $M_k = (x_1^k, \ldots, x_n^k)$, сходится к $M_0 = (x_1^0, \ldots, x_n^0)$ тогда и только тогда, когда $x_i^k \to x_i^0$ для всех $i = 1, \ldots, n$.

**Доказательство.**  
$(\implies)$ Пусть $M_k \to M_0$. Тогда $\rho(M_k, M_0) = \sqrt{\sum_{i=1}^n (x_i^k - x_i^0)^2} < \varepsilon$ для $k > k_0$. Поскольку $|x_i^k - x_i^0| \leq \rho(M_k, M_0)$, то $|x_i^k - x_i^0| < \varepsilon$, то есть $x_i^k \to x_i^0$.

$(\impliedby)$ Пусть $x_i^k \to x_i^0$ для всех $i$. Для любого $\varepsilon > 0$ существуют $k_0^i$, такие что $|x_i^k - x_i^0| < \frac{\varepsilon}{\sqrt{n}}$ для $k > k_0^i$. Выберем $k_0 = \max_i \{ k_0^i \}$. Тогда для $k > k_0$:
$$
\rho(M_k, M_0) = \sqrt{\sum_{i=1}^n (x_i^k - x_i^0)^2} < \sqrt{n \cdot \left( \frac{\varepsilon}{\sqrt{n}} \right)^2} = \varepsilon.
$$
Следовательно, $M_k \to M_0$.

Преобразовать уравнение $$\displaylines{
\sin{(x)}^{ 2 } \frac{\partial ^{ 2 }z}{\partial x^{ 2 }} - 2y\sin{(x)} \frac{\partial ^{ 2 }z}{\partial x\partial y}+ y^{ 2 } \frac{\partial ^{ 2 }z}{\partial y^{ 2 }} = 0    
}$$
принимая ${\displaystyle \begin{cases}u = y\tan{\left( \frac{x}{2} \right)} \\ v = y\end{cases}}$ за новые переменные.