## Последовательности в $\mathbb{R}^n$

### Определение последовательности точек в $\mathbb{R}^n$

Последовательность в $n$-мерном евклидовом пространстве $\mathbb{R}^n$ — это отображение
$$
\mathbb{N} \to \mathbb{R}^n,
$$
где каждому $k \in \mathbb{N}$ соответствует точка $M_k = (x_1^k, x_2^k, \ldots, x_n^k) \in \mathbb{R}^n$.

### Предел последовательности

Последовательность $\{ M_k \}_{k \geq 1}$ сходится к точке $M_0 = (x_1^0, x_2^0, \ldots, x_n^0) \in \mathbb{R}^n$, если
$$
M_0 = \lim_{k \to \infty} M_k \iff \forall \varepsilon > 0 \quad \exists k_0 \in \mathbb{N} : \forall k > k_0 \implies \rho(M_0, M_k) < \varepsilon,
$$
где $\rho(M_0, M_k) = \sqrt{\sum_{i=1}^n (x_i^k - x_i^0)^2}$ — евклидова метрика, а $M_k \in U_\varepsilon(M_0)$ — $\varepsilon$-окрестность точки $M_0$.

**Замечание.** Сходимость последовательности $M_k \to M_0$ эквивалентна сходимости числовой последовательности расстояний:
$$
M_k \to M_0 \iff \rho(M_0, M_k) \to 0.
$$



**Единственность предела.**  
Предел последовательности в $\mathbb{R}^n$, если он существует, единствен.

**Доказательство.**  
Предположим, что $\{ M_k \}_{k \geq 1}$ имеет два предела: $M_0$ и $\hat{M}_0$, где $M_0 \neq \hat{M}_0$. Тогда
$$
M_0 = \lim_{k \to \infty} M_k \iff \forall \varepsilon_0 > 0 \quad \exists k_0 \in \mathbb{N} : \forall k > k_0 \implies \rho(M_0, M_k) < \varepsilon_0,
$$
$$
\hat{M}_0 = \lim_{k \to \infty} M_k \iff \forall \hat{\varepsilon}_0 > 0 \quad \exists \hat{k}_0 \in \mathbb{N} : \forall k > \hat{k}_0 \implies \rho(\hat{M}_0, M_k) < \hat{\varepsilon}_0.
$$
Пусть $\varepsilon = \rho(M_0, \hat{M}_0) > 0$. Выберем $\varepsilon_0 = \hat{\varepsilon}_0 = \frac{\varepsilon}{2}$. Тогда для $k > \max\{ k_0, \hat{k}_0 \}$ по неравенству треугольника:
$$
\rho(M_0, \hat{M}_0) \leq \rho(M_0, M_k) + \rho(M_k, \hat{M}_0) < \varepsilon_0 + \hat{\varepsilon}_0 = \frac{\varepsilon}{2} + \frac{\varepsilon}{2} = \varepsilon.
$$
Получаем $\rho(M_0, \hat{M}_0) < \varepsilon = \rho(M_0, \hat{M}_0)$, что возможно только при $\rho(M_0, \hat{M}_0) = 0$, то есть $M_0 = \hat{M}_0$. Следовательно, предел единствен.