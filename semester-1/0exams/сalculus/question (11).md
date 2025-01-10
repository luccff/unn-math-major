### Сформулировать теорему Штольца. Использовать ее для поиска предела последовательности ${\left\{  \frac{\log_{a}(n)}{n}  \right\}}$
---
**Теорема Штольца.** Пусть ${\displaystyle \{ y_{n} \}}$ возрастающая бесконечно большая последовательность и пусть ${\displaystyle \left\{  \frac{x_{n+1}-x_{n}}{y_{n+1} -y_{n}}  \right\}}$ сходится и имеет предел ${\displaystyle  a}$. Тогда последовательность ${\displaystyle \left\{  \frac{x_{n}}{y_{n}}  \right\}}$ тоже сходится и имеет тот же предел ${\displaystyle  a}$.
Иначе:
$$\displaylines{
\lim_{ n \to \infty } {\frac{x_{n}}{y_{n}}} = \lim_{ n \to \infty } \frac{x_{n+1}-x_{n}}{y_{n+1} -y_{n}}  = a
}$$
Смысл теоремы: если "локальный темп роста" ${\displaystyle \left\{  \frac{x_{n+1}-x_{n}}{y_{n+1} -y_{n}}  \right\}}$ стабилизируется (имеет конечный предел ${\displaystyle a}$), то и отношение самих последовательностей стабилизируется к тому же пределу ${\displaystyle  a}$.

Пример: ${\displaystyle {\lim_{ n \to \infty }\frac{\log_{a}(n)}{n} }}$
Имеем:
$$\displaylines{
x_{n} = \log_{a}(n), \ y_{n} = n 
}$$
Применяем теорему:
$$\displaylines{
\begin{align}
\lim_{ n \to \infty }\frac{x_{n+1} - x_{n}}{y_{n+1} - y_{n}} = & \lim_{ n \to \infty }\frac{\log_{a}(n+1)-\log_{a}(n)}{(n+1) - n} = \\ & =
\lim_{ n \to \infty } \frac{\log_{a}\left( \cfrac{n+1}{n}  \right)}{1} \\ & =
\lim_{ n \to \infty } \log_{a}\left( 1+\frac{1}{n} \right) \\ & =
\log_{a}(1) = 0 

\end{align}
}$$
Следовательно ${\displaystyle \lim_{ n \to \infty } {\cfrac{\log_{a}(n)}{n}} = 0}$
