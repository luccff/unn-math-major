### Теоремы о пределах

Рассмотрим последовательности $\{ M_k' \} \sim \vec{OM_k'}$, $\{ M_k'' \} \sim \vec{OM_k''}$, их сумму $\{ M_k' + M_k'' \} \sim \vec{OM_k'} + \vec{OM_k''}$ и умножение на скаляр $\{ \lambda M_k' \} \sim \lambda \vec{OM_k'}$.

**Теорема 1.**  
Если $\lim_{k \to \infty} M_k' = M_0'$ и $\lim_{k \to \infty} M_k'' = M_0''$, то
$$
\lim_{k \to \infty} (M_k' + M_k'') = M_0' + M_0''.
$$

**Доказательство.**  
По основной теореме $(x_i'^k \to x_i'^0, x_i''^k \to x_i''^0)$. Тогда $x_i'^k + x_i''^k \to x_i'^0 + x_i''^0$, и по основной теореме $M_k' + M_k'' \to M_0' + M_0''$.

**Теорема 2.**  
Если $\lim_{k \to \infty} M_k' = M_0'$, то $\lim_{k \to \infty} \lambda M_k' = \lambda M_0'$.

**Доказательство.**  
Аналогично, $x_i'^k \to x_i'^0$ влечет $\lambda x_i'^k \to \lambda x_i'^0$, и по основной теореме $\lambda M_k' \to \lambda M_0'$.
