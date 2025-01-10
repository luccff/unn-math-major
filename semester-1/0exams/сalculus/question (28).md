### Эквивалентные бесконечно малые. Использование эквивалентных бесконечно малых при раскрытии неопределенностей вида ${ \cfrac{0}{0}}$, соответствующую теорему доказать. Сравнение бесконечно малых в окрестности ${\displaystyle  x = 0}$ с функцией ${\displaystyle y = ax^{ n }, \ n \in \mathbb{N}}$ - шкала бесконечно малых. Найти предел функции ${\displaystyle \lim_{ x \to 0 } {\left( x\cdot\sin{\left( \frac{1}{x} \right)} \right)}}$.
---

**Эквивалентные бесконечно малые.**
Определение. Две функции ${\displaystyle f(x) \wedge g(x)}$ называются эквивалентными бесконечно малыми в точке ${\displaystyle x = a}$, если ${\displaystyle \lim_{ x \to a } {\frac{f(x)}{g(x)}} = 1}$ и обозначаются ${\displaystyle f(x) \sim g(x), \ x \to a}$. Это означает, что обе функции стремятся к нулю с одинаковой скоростью.

**Использование эквивалентных бесконечно малых для раскрытия неопределённостей вида** ${\displaystyle \left[ \frac{0}{0} \right]}$. 
При вычислении предела такого вида неопределенности, мы можем заменить числитель и знаменатель на эквивалентные бесконечно малыми функциями. 

Если ${\displaystyle f(x)\sim\varphi(x) \wedge g(x)\sim\psi(x), \ x \to a}$, то 
$$\displaylines{
\lim_{ x \to a } {\frac{f(x)}{g(x)}} = \lim_{ x \to a } {\frac{\varphi(x)}{\psi(x)}}, \ \text{ если предел справа существует }
}$$
*Доказательство*:
Пусть ${\displaystyle f(x) \sim \varphi(x)}$, то есть:
$$\displaylines{
\lim_{ x \to a } {\frac{f(x)}{\varphi(x)}} = 1
}$$
Аналогично ${\displaystyle g(x) \sim \psi(x)}$:
$$\displaylines{
\lim_{ x \to a } {\frac{g(x)}{\psi(x)} } = 1
}$$
Рассмотрим предел ${\displaystyle \lim_{ x \to a } {\frac{f(x)}{g(x)}}}$
$$\displaylines{
\frac{f(x)}{g(x)} = \frac{f(x)}{\varphi(x)} \cdot \frac{\varphi(x)}{\psi(x)} \cdot \frac{\psi(x)}{g(x)}
}$$
Так как ${\displaystyle \lim_{ x \to a } {\frac{f(x)}{\varphi(x)} = 1}, \ \lim_{ x \to a } {\frac{g(x)}{\psi(x)} = 1}, \ \text{ и } \ \exists\lim_{ x \to a } {\frac{\varphi(x)}{\psi(x)}}}$, то:
$$\displaylines{
\lim_{ x \to a } {\frac{f(x)}{g(x)}} = \lim_{ x \to a } {\frac{\varphi(x)}{\psi(x)}}
}$$
**Сравнение бесконечно малых в окрестности нуля:**
Пусть ${\displaystyle x^{ n }, \ n \in \mathbb{N}}$ бесконечно малая функция при ${\displaystyle x \to 0}$. Если ${\displaystyle n > m}$ то ${\displaystyle x^{ n } = o(x^{ m })}$. Это значит, что ${\displaystyle x^{ n }}$ стремится к нулю быстрее, чем ${\displaystyle x^{ m }}$
Пример: ${\displaystyle x^{ 2 } = o(x), \ x^{ 3 } = o(x^{ 2 }), \ x \to 0}$

Найдем предел ${\displaystyle \lim_{ x \to 0 } {\left( x \cdot \sin{\left( \frac{1}{x} \right)} \right)}}$
$$\displaylines{
-1\leq \sin{\left( \frac{1}{x} \right)} \leq 1 \\
-x \leq x \cdot  \sin{\left( \frac{1}{x} \right)}\leq x \\
}$$
Так как ${\displaystyle  x \to 0}$ по теореме о двух милиционерах ${\displaystyle x \cdot \sin{\left( \frac{1}{x} \right)} \to 0}$. Значит предел ${\displaystyle \lim_{ x \to 0 } {\left( x \cdot \sin{\left( \frac{1}{x} \right)} \right)} = 0}$ 