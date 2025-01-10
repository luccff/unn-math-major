### Теоремы о пределах последовательности, связанных с неравенствами.
---
**Теорема 1**. Если все члены сходящейся последовательности ${\{ x_{n} \}}$ начиная с некоторого номера ${N_{ 0 }}$ таковы, что ${x_{n}>0 \ (n\geq N_{ 0 })}$, то ${\displaystyle\lim_{ n \to \infty } {x_{n}} \geq 0}$.  

*Доказательство*: обозначим ${\displaystyle\lim_{ n \to \infty } {x_{n}}} = a$. Необходимо доказать, что ${ a \geq 0 }$. Предположим противное ${ a<0}$. Рассмотрим ${|x_{n} - a|}$ при ${ n\geq N_{ 0 }}$. 
$$\displaylines{
|x_{n} - a| = |x_{n} + (-a)| = |x_{n}| + |a| \geq |a|, \ \text{ так как  } x_{n} \geq 0 \text{ при  } n\geq  N_{ 0 } \\
\text{ Таким образом,  } |x_{n}-a| \geq |a| \quad (1)
}$$
С другой стороны, по определению предела сходящейся числовой последовательности, можно выбрать ${ \varepsilon = a}$. Получим, что 
$$\displaylines{
|x_{n} - a| < |a| \text{ при } n\geq N(\varepsilon) \quad (2)
}$$
следовательно, при ${n > \max( \ N_{ 0 }, \ N(\varepsilon) \ )}$ должны одновременно выполнятся оба условия ${(1), \ (2)}$, что невозможно. Противоречие доказывает теорему.

**Теорема 2**. Если начиная с некоторого номера ${ N_{ 0 }}$ сходящиеся последовательности ${\{ x_{n} \}, \ \{ y_{n} \}}$ таковы, что ${x_{n}\leq y_{n}}$, то ${\displaystyle\lim_{ n \to \infty } {x_{n}} \leq \displaystyle\lim_{ n \to \infty } {y_{n}}}$

*Доказательство*: действительно, если ${ x_{n} \leq y_{n}}$, то ${|y_{n} - x_{n}| \geq 0 }$ при ${n \geq N_{ 0 }}$. Тогда  по предыдущей теореме ${ \displaystyle\lim_{ n \to \infty } {(y_{n} - x_{n})} \geq0}$. Так как ${\{ x_{n} \}, \ \{ y_{n} \}}$ сходящиеся последовательности, то тогда
$$\displaylines{
\lim_{ n \to \infty } {(y_{n} - x_{n})} = \lim_{ n \to \infty } {y_{n}} - \lim_{ n \to \infty } {x_{n}} \geq 0, \ \text{ то есть } \lim_{ n \to \infty } {y_{n}} \geq \lim_{ n \to \infty } {x_{n}} 
}$$
что и требовалось доказать.

*Замечание*: может случится так, что ${ x_{n} > 0 }$, тогда как ${\displaystyle\lim_{ n \to \infty } {x_{n} = 0}}$. Пример: ${x_{n} = \cfrac{1}{n} > 0}$, ${\displaystyle\lim_{ n \to \infty } {\cfrac{1}{n}}}$ = 0

**Теорема 3 (О двух милиционерах)**. Пусть начиная с некоторого номера ${N_{ 0 }}$ сходящиеся последовательности ${\{ x_{n} \}, \ \{ y_{n} \}, \ \{ z_{n} \}}$ связаны неравенствами ${x_{n} \leq y_{n} \leq z_{n}}$, причем последовательности  сходятся к одному пределу ${\displaystyle \lim_{ n \to \infty } {x_{n}} = \lim_{ n \to \infty } {z_{n}} = a}$, тогда последовательность ${\displaystyle \{ y_{n} \}}$ также сходится и имеет тот же предел, то есть ${\displaystyle  \lim_{ n \to \infty } {y_{n} } = a}$.

*Доказательство*: зададимся ${\displaystyle \varepsilon > 0}$, тогда 
$$\displaylines{
\exists N_{ 1 }(\varepsilon) : n> N_{ 1 }(\varepsilon) \ |x_{n} - a| < \varepsilon, \ \text{ а также } \ \exists N_{ 2 }(\varepsilon): n> N_{ 2 }(\varepsilon)  \ |z_{n} - a| < \varepsilon
}$$
При ${\displaystyle  n> }$ ${\displaystyle  \max(N_{ 1 }(\varepsilon), \ N_{ 2 }(\varepsilon))}$ выполняются оба этих неравенства, то есть выполнено, что 
$$\displaylines{
a- \varepsilon < x_{n} < a +\varepsilon \\ \text{ и } \\ a - \varepsilon < z_{n} < a + \varepsilon
}$$
Имея в виду неравенства ${\displaystyle  x_{n} \leq y_{n} \leq z_{n}}$ можно записать, что 
$$\displaylines{
a - \varepsilon < x_{n} \leq y_{n} \leq z_{n} < a+ \varepsilon
}$$
Таким образом, при  ${\displaystyle  n> }$ ${\displaystyle  \max(N_{ 1 }(\varepsilon), \ N_{ 2 }(\varepsilon))}$ выполнено
$$\displaylines{
a-\varepsilon \leq  y_{n} \leq  a+\varepsilon \implies  \lim_{ n \to \infty } {y_{n}} = a
}$$

**Теорема 4**. Если неубывающая (невозрастающая) последовательность ограничена сверху (снизу), то она имеет предел.

*Доказательство*: действительно, если последовательность ${\displaystyle \{ x_{n} \}}$ ограничена сверху, то она имеет точную верхнюю грань ${\displaystyle \sup \{ x_{n} \}} = L$. Докажем, что ${\displaystyle \lim_{ n \to \infty } {x_{n}} = L}$. Зададимся ${\displaystyle  \varepsilon > 0}$ и рассмотрим ${\displaystyle L -\varepsilon}$. По определению супремума, всегда найдется ${\displaystyle x_{N}}$ такое, что ${\displaystyle L \geq x_{N} > L - \varepsilon}$ и тем более, ${\displaystyle L - \varepsilon < x_{N} \leq x_{n} < L+\varepsilon}$, то есть ${\displaystyle |x_{n} -L| < \varepsilon \implies \lim_{ n \to \infty } {x_{n}}  = L}$. Теорема доказана.


