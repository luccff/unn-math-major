### Равномерная непрерывность функции на множестве. Теорема Кантора о равномерной непрерывности на отрезке. Доказать.
---
Функция ${\displaystyle f(x)}$ называется **равномерно непрерывной** на ${\displaystyle E}$ если:
$$\displaylines{
 \forall{\varepsilon} >0 \ \  \exists \delta_{ \varepsilon } >0: \forall{x', \ x'' \in E}: (x'-x'') < \delta \hookrightarrow |f(x') - f(x'')| < \varepsilon
}$$
**Теорема Кантора:**
Если функция ${\displaystyle f(x)}$ непрерывна на замкнутом отрезке ${\displaystyle [a, \ b]}$, то она равномерно непрерывна на этом отрезке.

*Доказательство*:
Предположим противное: $f(x)$ непрерывна на $[a, b]$, но не равномерно непрерывна. Тогда существует $\varepsilon_0>0$, для которого, как бы мало мы ни выбрали $\delta>0$, найдутся точки $x_n, y_n \in[a, b]$, такие что:
$$
\left|x_n-y_n\right|<\frac{1}{n}, \quad\left|f\left(x_n\right)-f\left(y_n\right)\right| \geq \varepsilon_0 .
$$
 Компактность отрезка: Поскольку $[a, b]$ - компакт, последовательность $\left\{x_n\right\}$ имеет сходящуюся подпоследовательность $x_{n_k} \rightarrow c \in[a, b]$. Тогда $y_{n_k} \rightarrow c$, так как $\left|x_n-y_n\right|<\cfrac{1}{n}$.
Непрерывность $f(x)$ : По непрерывности $f(x)$ на $[a, b]$ :

$$
f\left(x_{n_k}\right) \rightarrow f(c), \quad f\left(y_{n_k}\right) \rightarrow f(c)
$$
Следовательно:
$$
\left|f\left(x_{n_k}\right)-f\left(y_{n_k}\right)\right| \rightarrow 0 \quad \text { при } k \rightarrow \infty
$$
Противоречие: По условию $\left|f\left(x_n\right)-f\left(y_n\right)\right| \geq \varepsilon_0$ для всех $n$, что противоречит $\left|f\left(x_{n_k}\right)-f\left(y_{n_k}\right)\right| \rightarrow 0$.
