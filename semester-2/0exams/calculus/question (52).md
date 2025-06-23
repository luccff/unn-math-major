Ограниченность сходящейся последовательности.  
Если $\{ M_k \}_{k \geq 1}$ сходится к $M_0$, то она ограничена, то есть существует $R > 0$, такое что $\forall k \quad M_k \in B_R(O)$, где $O = (0, 0, \ldots, 0)$ и $B_R(O) = \{ M \in \mathbb{R}^n : \rho(O, M) \leq R \}$.

**Доказательство.**  
Поскольку $M_k \to M_0$, для $\varepsilon = 1$ существует $k_0 \in \mathbb{N}$, такое что для всех $k > k_0$
$$
\rho(M_0, M_k) < 1 \implies M_k \in B_1(M_0).
$$
Рассмотрим конечное множество расстояний $\{ \rho(M_0, M_1), \rho(M_0, M_2), \ldots, \rho(M_0, M_{k_0}) \}$. Пусть
$$
\overline{\rho} = \max_{i=1, \ldots, k_0} \rho(M_0, M_i), \quad \tilde{\rho} = \rho(O, M_0) + 1.
$$
Тогда выберем $R = \max\{ \overline{\rho}, \tilde{\rho} \}$. Для $k \leq k_0$ имеем $\rho(O, M_k) \leq \rho(O, M_0) + \rho(M_0, M_k).AIAssistant: \leq \overline{\rho} \leq R$. Для $k > k_0$, по неравенству треугольника:
$$
\rho(O, M_k) \leq \rho(O, M_0) + \rho(M_0, M_k) < \rho(O, M_0) + 1 \leq \tilde{\rho} \leq R.
$$
Таким образом, $\rho(O, M_k) \leq R$ для всех $k$, то есть $\{ M_k \}$ ограничена.