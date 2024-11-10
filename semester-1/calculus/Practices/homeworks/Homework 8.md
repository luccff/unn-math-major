# Part 1 
**Exercise 1:** 
$$\displaylines{
\lim_{ n \to \infty } \frac{n^{2} + n^{ 3 } - 44n}{3n \cdot (n + 1) - n^{2} + 1} = \frac{\infty - \infty}{\infty - \infty} = (*) \\ 
\begin{aligned}
(*) &= \lim_{ n \to \infty } \frac{n^{ 3 }}{3n^{2} + 3n - n^{2} + 1} \\ 
&= \lim_{ n \to \infty } \frac{n^{ 3 }}{2n^{2} + 3n + 1} \\
&= \lim_{ n \to \infty } \frac{n^{ 3 }}{n^{2}} \\ 
&= \lim_{ n \to \infty } n = \infty
\end{aligned}
}$$

**Exercise 2:**
$$\displaylines{
\lim_{ n \to \infty } \frac{2n^{ 4 } + 2n^{ 3 } \cdot (3 - n) - n \cdot (n^{2} + 3)}{(n + 1)^{ 5 } - n - 5n^{ 4 } - n^{ 5 } + 1} =  \text{indeterminate form} = (*) \\ 
\begin{aligned}
(*) &= \lim_{ n \to \infty } \frac{6n^{ 3 } - n^{ 3 }}{10n^{ 3 }} \\ 
&= \lim_{ n \to \infty } \frac{5n^{ 3 }}{10n^{ 3 }} = \frac{1}{2}
\end{aligned}
}$$

# Part 2 
**Exercise 1.1:**
$$\displaylines{
\lim_{ n \to \infty } \frac{2n^{2} + \sqrt[3]{ 27n^{ 6 } + n }}{\sqrt[3]{ n^{ 7 } + 2 } - 3n \cdot (n + 1)} = \frac{\infty}{\infty - \infty} = (*) \\ 
\begin{aligned}
(*) &= \lim_{ n \to \infty } \frac{2n^{2} + 3n^{2}}{n^{ \frac{7}{3} }} \\ 
&= \lim_{ n \to \infty } \frac{5n^{2}}{n^{ \frac{7}{3} }} = 0
\end{aligned}
}$$

**Exercise 1.2:** 
$$\displaylines{
\lim_{ n \to \infty } \frac{\sqrt[]{ 4n^{ 4 } - n } - \sqrt[3]{ 27n^{ 6 } + 3n }}{\sqrt[]{ n^{ 4 } + 1 } - 3n^{2}} = \text{indeterminate form} = (*) \\ 
\begin{aligned}
(*) &= \lim_{ n \to \infty } \frac{2n^{2} - 3n^{2}}{n^{2} - 3n^{2}} \\
&= \lim_{ n \to \infty } \frac{-n^{2}}{-2n^{2}} = \frac{1}{2}
\end{aligned}
}$$

**Exercise 2.1:** 
$$\displaylines{
\lim_{ n \to \infty } \sqrt[]{ n + 1 } - \sqrt[]{ n - 1 } = \infty - \infty = (*) \\ 
\begin{aligned}
(*) &= \lim_{ n \to \infty } \frac{n + 1 - n + 1}{\sqrt[]{ n + 1 } + \sqrt[]{ n - 1 }} \\ 
&= \lim_{ n \to \infty } \frac{1}{\infty} = 0
\end{aligned}
}$$

**Exercise 2.2:** 
$$\displaylines{
\lim_{ n \to \infty } \sqrt[]{ n^{2} + 4n } - \sqrt[]{ n^{2} + n } = \infty - \infty = (*) \\ 
\begin{aligned}
(*) &= \lim_{ n \to \infty } \frac{n^{2} + 4n - n^{2} - n}{\sqrt[]{ n^{2} + 4n } + \sqrt[]{ n^{2} + n }} \\ 
&= \lim_{ n \to \infty } \frac{3n}{n + n} \\ 
&= \lim_{ n \to \infty } \frac{3n}{2n} = \frac{3}{2}
\end{aligned}
}$$

**Exercise 2.3:** 
$$\displaylines{
\lim_{ n \to \infty } \frac{\sqrt[]{ n^{2} - n } - \sqrt[]{ n^{2} + n }}{\sqrt[]{ n^{2} + n } - n} = \text{indeterminate form} = (*) \\ 
\begin{aligned}
(*) &= \lim_{ n \to \infty } \frac{\sqrt{ n^{2} - n } - \sqrt{ n^{2} + n }}{\sqrt{ n^{2} + n } - n } \mid \cdot \frac{(\sqrt{ n^{2} - n } + \sqrt{ n^{2} + n }) \cdot (\sqrt{ n^{2} + n } + n)}{(\sqrt{ n^{2} - n } + \sqrt{ n^{2} + n }) \cdot (\sqrt{ n^{2} + n } + n)} \\ 
&= \lim_{ n \to \infty } \frac{(n^{2} - n - n^{2} - n) \cdot (\sqrt{ n^{2} + n } + n)}{(n^{2} + n - n^{2}) \cdot (\sqrt{ n^{2} - n } + \sqrt{ n^{2} + n })} \\ 
&= \lim_{ n \to \infty } \frac{-2n \cdot (\sqrt{ n^{2} + n } + n)}{n \cdot (\sqrt{ n^{2} - n } + \sqrt{ n^{2} + n })} \\ 
&= \lim_{ n \to \infty } \frac{-2n \cdot (n + n)}{n \cdot (n + n)} = -2 
\end{aligned}
}$$

**Exercise 3.1:**
$$\displaylines{
\lim_{ n \to \infty } \sqrt[3]{ n^{ 3 } + 3n^{2} } - \sqrt[3]{ n^{ 3 } - n } = \infty - \infty = (*) \\ 
\begin{aligned}
(*) &= \lim_{ n \to \infty } \frac{n^{ 3 } + 3n^{2} - n^{ 3 } + n}{\sqrt[3]{ (n^{ 3 } + 3n^{ 2 })^{2} } + \sqrt[3]{ (n^{ 3 } + 3n^{2}) \cdot (n^{ 3 } - n) } + \sqrt[3]{ (n^{ 3 } - n)^{2} }} \\ 
&= \lim_{ n \to \infty } \frac{3n^{2} }{n^{2} + n^{2} + n^{2} } = \lim_{ n \to \infty } \frac{3n^{2}}{3n^{2}} = 1
\end{aligned}
}$$

**Exercise 3.2:**
$$\displaylines{
\lim_{ n \to \infty } \sqrt[3]{ n^{ 6 } + n^{ 4 } } - \sqrt[3]{ n^{ 6 } - 2n^{ 4 } } = \infty - \infty = (*) \\
\begin{aligned}
(*) &= \lim_{ n \to \infty }  \frac{n^{ 6 } + n^{ 4 } - n^{ 6 } + 2n^{ 4 }}{\sqrt[3]{ (n^{ 6 } + n^{ 4 })^{ 2 } } + \sqrt[3]{ (n^{ 6 } + n^{ 4 }) \cdot (n^{ 6 } - 2n^{ 4 }) } + \sqrt[3]{ (n^{ 6 } - 2n^{ 4 })^{2} }} \\ 
&= \lim_{ n \to \infty } \frac{3n^{ 4 }}{\sqrt[3]{ n^{ 12 } + 2 \cdot n^{ 6 } \cdot n^{ 4 } + n^{ 8 } } + \sqrt[3]{ n^{ 12 } - 2n^{ 10 } + n^{ 10 } -2n^{ 8 } } + \sqrt[3]{ n^{ 12 } - 4 \cdot n^{ 6 } \cdot n^{ 4 } + 4n^{ 8 } }} \\ 
&= \lim_{ n \to \infty } \frac{3n^{ 4 }}{n^{ 4 } + n^{ 4 } + n^{ 4 }} = \frac{3n^{ 4 }}{3n^{ 4 } } = 1
\end{aligned}
}$$

# Part 3 
**Exercise 39.2:**
$$\displaylines{
a^{ 3 } - b^{ 3 } = (a - b) \cdot (a^{2} + ab + b^{2}) \\
\lim_{ n \to \infty } \frac{(n^{2} + 3n + 4)^{ 3 } - (n^{2} + 3n - 4)^{ 3 }}{(n^{2} + 5n + 6)^{ 3 } - (n^{2} + 5n - 6)^{ 3 }} = \text{indeterminate form} = (*) \\ 
\begin{aligned}
(*) &= \dots 
\end{aligned}
}$$


**Exercise 39.3:**
$$\displaylines{
\lim_{ n \to \infty } \frac{n^{2}}{n + 1} - \frac{n^{ 3 }}{n^{2} + 1} = \infty - \infty = (*) \\ 
\begin{aligned}
(*) &= \lim_{ n \to \infty } \frac{n^{2} \cdot (n^{2} + 1) - n^{ 3 } \cdot (n + 1)}{(n^{2} + 1) \cdot (n + 1)} \\
&= \lim_{ n \to \infty } \frac{n^{ 4 } + n^{2} - n^{ 4 } - n^{ 3 }}{n^{ 3 }} \\ 
&= \lim_{ n \to \infty } \frac{-n^{ 3 }}{n^{ 3 }} = -1 
\end{aligned}
}$$

**Exercise 39.5:**
$$\displaylines{
\lim_{ n \to \infty } \frac{(2 + n)^{ 100 } - n^{ 100 } - 200n^{ 99 }}{n^{ 98 } - 10n^{2} + 1} = \text{indeterminate form} = (*) \\ 
(a + b)^{ n } = \sum_{ k = 0 }^{ n } \binom{n}{k} \cdot a^{ n - k } \cdot b^{ k } \\ 
(n + 2)^{ 100 } = n^{ 100 } + \binom{100}{1} \cdot n^{ 99 } \cdot 2 + \binom{100}{2} \cdot n^{ 98 } \cdot 2^{2} + \dots \\ 
\begin{matrix}\binom{100}{1} = \frac{100!}{1 \cdot 99!} = 100 & \binom{100}{2} = \frac{100!}{2 \cdot 98!} = 4950\end{matrix} \\ 
(n + 2)^{ 100 } = n^{ 100 } + 200 \cdot n^{ 99 } + 19800 \cdot n^{ 98 } + \dots \\ 
\lim_{ n \to \infty } \frac{19800 \cdot n^{ 98 }}{n^{ 98 }} = 19800
}$$

**Exercise 53.4:**
$$\displaylines{
\lim_{ n \to \infty } \sqrt[3]{ n^{ 3 } + n^{2} + 2002 } - n = \infty - \infty = (*) \\ 
\begin{aligned}
(*) &= \lim_{ m \to \infty } \sqrt[3]{ n^{ 3 } + n^{2} + 2002 } - \sqrt[3]{ n^{ 3 } } \\ 
&= \lim_{ n \to \infty } \frac{n^{ 3 } + n^{2} + 2002 - n^{ 3 }}{\sqrt[3]{ (n^{ 3 } + n^{2} + 2002)^{ 2 } } + \sqrt[3]{ (n^{ 3 } + n^{2} + 2002) \cdot n^{ 3 } } + \sqrt[3]{ (n^{ 3 })^{2} }} \\ 
&= \lim_{ n \to \infty } \frac{n^{2}}{n^{2} + n^{2} + n^{2}} \\ 
&= \lim_{ n \to \infty } \frac{n^{2}}{3n^{2}} = \frac{1}{3}
\end{aligned}
}$$

**Exercise 53.5:**
$$\displaylines{
\lim_{ n \to \infty } n^{ \frac{3}{2} } \cdot (\sqrt{ n + 1 } + \sqrt{ n - 1 } - 2\sqrt{ n }) = \infty - \infty = (*) \\ 
\begin{aligned}
(*) &= \lim_{ n \to \infty } n^{ \frac{3}{2} } \cdot (\sqrt{ n + 1 } + \sqrt{ n - 1 } - 2\sqrt{ n }) \\ 
&= \lim_{ n \to \infty } n^{ \frac{3}{2} } \cdot \lim_{ n \to \infty } (\sqrt{ n + 1 } + \sqrt{ n - 1 } - 2\sqrt{ n }) 
\end{aligned} \\ 
\begin{aligned}
\lim_{ n \to \infty } (\sqrt{ n + 1 } + \sqrt{ n - 1 } - 2\sqrt{ n } ) &= \lim_{ n \to \infty } \frac{(\sqrt{ n + 1 } + \sqrt{ n - 1 })^{2} - 4n}{\sqrt{ n + 1 } + \sqrt{ n - 1 } + 2\sqrt{ n }} \\ 
&= \lim_{ n \to \infty } \frac{-2n}{\sqrt{ n } + \sqrt{ n } + 2\sqrt{ n }} \\ 
&= \lim_{ n \to \infty } \frac{-2n}{4\sqrt{ n }}  \\
&= \lim_{ n \to \infty } - \frac{n}{2\sqrt{ n }} = - \infty
\end{aligned} \\
(*) = \infty \cdot (-\infty) = -\infty
}$$

