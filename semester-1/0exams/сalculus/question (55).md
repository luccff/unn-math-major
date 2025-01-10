### Теорема Коши. Доказать
---
Теорема Коши (обобщение теоремы Лагранжа):
$$\displaylines{
\begin{pmatrix}
f, \ g - \text{ непрерывны на  } [a, \ b] \\
f, \ g - \text{ дифференцируемы на  }(a, \ b) \\
g(x) \neq 0, \  x \in  {(a, \ b)}
\end{pmatrix} \implies \begin{pmatrix}
\exists c \in (a, \ b):  
\cfrac{f(b)-f(a)}{g(b) -g(a)} = \cfrac{f'(c)}{g'(c)}   
\end{pmatrix}
}$$
Доказательство. 
$$\displaylines{
F(x) = f(x) -f(a) -\frac{f(b) - f(a)}{g(b) - g(a)}(g(x) - g(a))
}$$
По теореме Ролля (непрерывность, дифференцируемость и ${\displaystyle F(a)=F(b)=0}$), значит существует такая точка ${\displaystyle c \in (a, \ b)}$, что ${\displaystyle F'(c) = 0}$
$$\displaylines{
F'(x) = f'(x) - \frac{f(b)-f(a)}{g(b)-g(a)}g'(x) 
}$$
Значит:
$$\displaylines{
\exists c \in (a, \  b):F'(c) = 0\\
0 = f'(c)-\frac{f(b)-f(a)}{g(b)-g(a)}g'(c) \\
\frac{f(b)-f(a)}{g(b)-g(a)} = \frac{f'(c)}{g'(c)} 
}$$
