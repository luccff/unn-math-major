### Деление отрезка в данном отношении.
---
Пусть $\vec{AM} = \lambda \vec{MB} \implies \vec{r}_{ M } =  \dfrac{\vec{r}_{ A } + \lambda \vec{r}_{ B }}{1 + \lambda}$. 
![[Pasted image 20250118210644.png]]
Доказательство:
$$\displaylines{
\vec{OA} + \vec{AB} = \vec{OB} \implies  \vec{AB} = \vec{OB} - \vec{OA} \\
\vec{AB} = \vec{r}_{ B } - \vec{r}_{ a } \\
\vec{AB} = \vec{AM} + \vec{MB} = (1+\lambda)\vec{MB} \\
\vec{MB} = \frac{\vec{AB}}{1+ \lambda} = \frac{\vec{r}_{ B } - \vec{r}_{ A }}{1+\lambda}  \\
\begin{aligned}
\vec{OM} = \vec{OB} + \vec{BM} & =\vec{OB} - \vec{MB} \\
&= \vec{OB} - \frac{\vec{r}_{ B } - \vec{r}_{ A }}{1+\lambda}\\
&= \vec{r}_B - \frac{\vec{r}_B - \vec{r}_A}{1+\lambda} \\
&= \frac{(1+\lambda)\vec{r}_B - (\vec{r}_B - \vec{r}_A)}{1+\lambda} \\ 
&= \frac{\vec{r}_B + \lambda\vec{r}_B - \vec{r}_B + \vec{r}_A}{1+\lambda} \\ 
&= \frac{\lambda\vec{r}_B + \vec{r}_A}{1+\lambda} = \frac{ \vec{r}_A + \lambda\vec{r}_B}{1+\lambda}
\end{aligned}
}$$
