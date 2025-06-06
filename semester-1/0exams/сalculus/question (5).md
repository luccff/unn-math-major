### Числовая последовательность. Предел последовательности (конечный), определение через окрестности и неравенства и геометрическая интерпретация. Единственность предела последовательности (доказать). Сходящиеся и расходящиеся последовательности. Примеры.
---

*Определение*. **Числовая последовательность** - это упорядоченный набор чисел, где каждому натуральному номеру ${n}$ соответствует элемент последовательности ${ x_{n}}$.
Пример не сходящейся последовательности.
![[Pasted image 20250102010006.png | 400 ]] 

Пример сходящейся последовательности.
![[Pasted image 20250104195829.png | 400]]

*Определение*. Последовательность ${x_{n}}$ имеет конечный предел, равный ${a}$, т.е.
$$\displaylines{
\lim_{ n \to \infty } {x_{n}} = a, \ \text{ если } \forall{\varepsilon}>0 \ \exists N = N(\varepsilon): \ \forall{n>N} \ |x_{n}-a| < \varepsilon
}$$
*Теорема о единственности предела последовательности.*
Если ${\displaystyle \lim_{ n \to \infty } {x_{n} = a}}$ и ${\displaystyle\lim_{ n \to \infty } {x_{n}} = b}$, то ${a = b}$.

*Доказательство* (от противного). Пусть ${a\neq b, \ a< b}$. Возьмем ${\varepsilon = \cfrac{b-a}{2}}$, тогда
$$\displaylines{
\forall{\varepsilon >0} \ \exists N_{ a } = N_{ a }(\varepsilon) : \forall{n}>N_{ a } \ |x_{ n } - a| < \frac{b-a}{2} \\
\forall{\varepsilon >0} \ \exists N_{ b } = N_{ b }(\varepsilon) : \forall{n}>N_{ b } \ |x_{ n } - b| < \frac{b-a}{2} \\ \\
\begin{matrix}
\cfrac{a-b}{2} < x_{n}-a< \cfrac{b-a}{2}  &  & \cfrac{a-b}{2}<x_{n} - b < \cfrac{b-a}{2}  \\
\cfrac{3a-b}{2} < \boxed{x_{n} < \cfrac{a+b}{2}}  & \text{ противоречие } & \boxed{ \cfrac{a+b}{2}<x_{n}}< \cfrac{3b-a}{2}  
\end{matrix} 
}$$

*Определение*. Последовательность ${\{ x_{n} \}^{ \infty }_{ 0 }}$ называется **сходящейся**, если существует конечный предел ${\displaystyle\lim_{ n \to \infty } {x_{n} = a}}$.
Пример: ${\displaystyle \lim_{ n \to \infty } {\frac{1}{n}}}$ сходится к нулю, так как при увеличении ${n}$ последовательность ${ x_{n} }$ становится всё ближе к нулю.

Интересный факт: если пространство снабжено антидискретной топологией, то пределом любой последовательности будет любой элемент пространства, так как любая последовательность сходится к любой точке пространства, поскольку единственная окрестность любой точки (всё пространство) всегда содержит почти все элементы последовательности.

Антидискретная топология (или тривиальная, или топология слипшихся точек) -  семейство подмножеств ${\mathcal{T} = \{ X, \ \emptyset \}}$, где ${X}$ произвольное множество. В ней все точки "слипшиеся", то есть топологически неразличимы.

*Определение*. Последовательность $\{ {x_{n}} \}^{ \infty }_{ 0 }$ называется **расходящейся**, если она не имеет конечного предела.
Пример: ${x_{n} = (-1)^{ n }}$, ${\cancel\exists \lim_{ n \to \infty } {x_{n}}} = a$.