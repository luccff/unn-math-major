### Теорема Лагранжа. Доказать.
---
Теорема Лагранжа. Пусть ${\displaystyle f(x)}$ непрерывна на ${\displaystyle [a, \ b]}$ и дифференцируема на ${\displaystyle (a, \ b)}$, тогда существует хотя бы одна точка ${\displaystyle с \in (a, \ b)}$, такая что:
$$\displaylines{
f'(c) = \frac{f(b)- f(a)}{b - a} 
}$$
Доказательство: рассмотрим вспомогательную функцию ${\displaystyle g(x) = f(x) - \frac{f(b)-f(a)}{b- a}(x-a)}$. ${\displaystyle g(a) = g(b) = 0}$, что удовлетворяет теореме Ролля (непрерывность, дифференцируемость и ${\displaystyle g(a)=g(b)=0}$), значит существует такая точка ${\displaystyle c \in (a, \ b)}$, что ${\displaystyle g'(c) = 0}$
Найдем ${\displaystyle g'(x)}$:
$$\displaylines{
g'(x) = f'(x) - \frac{f(b)-f(a)}{b-a} 
}$$
Так как ${\displaystyle g'(c) = 0}$ получаем:
$$\displaylines{
f'(c) -\frac{f(b)-f(a)}{b-a} = 0
}$$
Следовательно:
$$\displaylines{
f'(c) = \frac{f(b)-f(a)}{b-a} 
}$$
![[Pasted image 20250108084454.png | 400]]
