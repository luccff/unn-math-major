# Part 1 (Exercise 77)
**Point 1:** 
$$\displaylines{
\lim_{ n \to \infty } \sqrt[3n]{ n } = \lim_{ n \to \infty } n^{ \frac{1}{3n} } = \infty^{ 0 } = (*) \\ 
(*) = \lim_{ n \to \infty } n^{ \frac{1}{3n} } = \lim_{ n \to \infty } e^{ \frac{\ln(n)}{3n} } = e^{ 0 } = 1
}$$

**Point 2:** 
$$\displaylines{
\lim_{ n \to \infty } n^{ \frac{p}{n^{ k }} } = \infty^{ 0 } = (*) \\ 
(*) = \lim_{ n \to \infty } n^{ \frac{p}{n^{ k }} } = \lim_{ n \to \infty } e^{ \frac{\ln(n) \cdot p}{n^{ k }} } = e^{ 0 } = 1
}$$

**Point 3:** 
$$\displaylines{
\lim_{ n \to \infty } \sqrt[n]{ n + a } = \lim_{ n \to \infty } (n + a)^{ \frac{1}{n} } = \infty^{ 0 } = (*) \\ 
(*) = \lim_{ n \to \infty } e^{ \frac{\ln(n + a)}{n} } = e^{ 0 } = 1
}$$

**Point 4:** 
$$\displaylines{
\lim_{ n \to \infty } \sqrt[n]{ an + b } = \lim_{ n \to \infty } (an + b)^{ \frac{1}{n} } = \infty^{ 0 } = (*) \\ 
(*) = \lim_{ n \to \infty } e^{ \frac{\ln(an + b)}{n} } = \lim_{ n \to \infty } e^{ \frac{\ln(a) + \ln(n)}{n} } = e^{ 0 } = 1
}$$

**Point 5:** 
$$\displaylines{
\lim_{ n \to \infty } \sqrt[n]{ n^{ 3 } - 3n + 1 } = \lim_{ n \to \infty } (n^{ 3 } - 3n + 1)^{ \frac{1}{n} } = \infty^{ 0 } = (*) \\ 
(*) = \lim_{ n \to \infty } (n^{ 3 } - 3n + 1)^{ \frac{1}{n} } = \lim_{ n \to \infty } e^{ \frac{\ln(n^{ 3 } - 3n + 1)}{n} } = \lim_{ n \to \infty } e^{ \frac{\ln(n^{ 3 })}{n} } = \lim_{ n \to \infty } e^{ \frac{3 \cdot \ln(n)}{n} } = e^{ 0 } = 1
}$$

**Point 6:** 
$$\displaylines{
\lim_{ n \to \infty } \sqrt[2n]{ n^{2} - 1 } = \lim_{ n \to \infty } (n^{2} - 1)^{ \frac{1}{2n} } = \infty^{ 0 } = (*) \\ 
(*) = \lim_{ n \to \infty } (n^{2} - 1)^{ \frac{1}{2n} } = \lim_{ n \to \infty } e^{ \frac{\ln(n^{2} - 1)}{2n} } = \lim_{ n \to \infty } e^{ \frac{2 \cdot \ln(n)}{2n} } = e^{ 0 } = 1
}$$

**Point 7:**
$$\displaylines{
\lim_{ n \to \infty } \sqrt[n]{ 2^{ n } \cdot n^{2} + 2n - 1 } = \lim_{ n \to \infty } (2^{ n } \cdot n^{2} + 2n - 1)^{ \frac{1}{n} } = \infty^{ 0 } = (*) \\ 
(*) = \lim_{ n \to \infty } e^{ \frac{\ln(2^{ n } \cdot n^{2} + 2n - 1)}{n} } = \lim_{ n \to \infty } e^{ \frac{\ln(2^{ n } \cdot n^{2})}{n} } = \lim_{ n \to \infty } e^{ \frac{n \cdot \ln(2) + 2 \cdot \ln(n)}{n} } = e^{ \ln(2) } = 2
}$$

**Point 8:**
$$\displaylines{
\lim_{ n \to \infty } \sqrt[n]{ \frac{1}{n} - \frac{1}{2^{ n }} } = \lim_{ n \to \infty } \left( \frac{1}{n} - \frac{1}{2^{ n }}\right)^{ \frac{1}{n} } = 0^{ 0 } = (*) \\ 
(*) = \lim_{ n \to \infty } \left( \frac{1}{n} - \frac{1}{2^{ n }} \right)^{ \frac{1}{n} } = \lim_{ n \to \infty } e^{ \frac{\ln\left( \frac{1}{n} - \frac{1}{2^{ n }} \right)}{n} } = \lim_{ n \to \infty } e^{ \frac{\ln\left( \frac{1}{n} \right)}{n} } = e^{ 0 } = 1
}$$

**Point 9:** 
$$\displaylines{
\lim_{ n \to \infty } \frac{\sqrt[n]{ n^{ 4 } } + 2\sqrt[n]{ n^{2} } - 3}{\sqrt[n]{ n^{2} } - 3\sqrt{ n } + 2} = \lim_{ n \to \infty } \frac{\sqrt[n]{ n^{ 4 } }}{\sqrt[n]{ n^{2} } - 3\sqrt{ n }} = \lim_{ n \to \infty } \frac{n^{ \frac{4}{n} }}{n^{ \frac{2}{n} } - 3 \cdot n^{ \frac{1}{2} }} = \lim_{ n \to \infty } \frac{n^{ \frac{1}{4} }}{-3 \cdot n^{ \frac{1}{2} }} = -\frac{1}{3} \cdot \lim_{ n \to \infty } n^{ \frac{1}{4} - \frac{1}{2} } = -\frac{1}{3} \cdot \lim_{ n \to \infty } n^{ -\frac{1}{4} } = -\frac{1}{3} \cdot 0 = 0
}$$

**Point 10:** 
$$\displaylines{
\sqrt[3n]{ \frac{n^{ 4 } - 2n + 3}{n^{2} + 1} } \\ 
\dots
}$$
# Part 2
## Exercise 162
**Point 1:** 
$$\displaylines{
x_{ n } = \frac{n^{ 3 }}{10^{ n }} \\ 
\frac{x_{ n + 1}}{x_{ n }} = \frac{(n + 1)^{ 3 }}{10^{ n + 1 }} : \frac{n^{ 3 }}{10^{ n }} = \frac{(n + 1)^{ 3 } \cdot 10^{ n }}{10^{ n + 1 } \cdot n^{ 3 }} = \frac{(n + 1)^{ 3 }}{10 \cdot n^{ 3 }} = \left( \frac{n + 1}{n} \right)^{ 3 } \cdot \frac{1}{10} = \left( 1 + \frac{1}{n} \right)^{ 3 } \cdot \frac{1}{10} \leq \frac{8}{10} < 1 \implies x_{ n } \downarrow \\ 
x_{ n } = \frac{n^{ 3 } > 0}{10^{ n } > 0} \implies x_{ n } > 0 \\ 
\begin{matrix}
x_{ n } \downarrow  \\
x_{ n } > 0 
\end{matrix} \implies x_{ n } \text{ converges} \\ 
\lim_{ n \to \infty } \frac{n^{ 3 }}{10^{ n }} = 0
}$$

**Point 2:**
$$\displaylines{
x_{ n } = \frac{2000^{ n }}{n!} \\ 
\frac{x_{ n + 1 }}{x_{ n }} = \frac{2000^{ n + 1 }}{(n + 1)!} : \frac{2000^{ n }}{n!} = \frac{2000^{ n + 1 } \cdot n!}{(n + 1)! \cdot 2000^{ n }} = \frac{2000 \cdot 2000^{ n } \cdot n!}{n! \cdot (n + 1) \cdot 2000^{ n }} = \frac{2000}{n + 1} < 1 \text{ (starting from n = 2000)} \\ 
x_{ n } = \frac{2000^{ n } > 0}{n! > 0} \implies x_{ n } > 0 \\ 
\begin{matrix}
x_{ n } \downarrow \text{ (starting from n = 2000)}  \\
x_{ n } > 0
\end{matrix} \implies x_{ n } \text{ converges} \\ 
\lim_{ n \to \infty } \frac{2000^{ n }}{n!} = 0
}$$

**Point 3:**
$$\displaylines{
x_{ n } = \prod_{ i = 1 }^{ n } \frac{3n + 5}{6n - 5} \\ 
\begin{aligned}
\frac{x_{ n + 1 }}{x_{ n }} &= \prod_{ i = 1 }^{ n } \frac{3n + 5}{6n - 5} \cdot \frac{3 \cdot (n + 1) + 5}{ 6 \cdot (n + 1) - 5} : \prod_{ i = 1 }^{ n } \frac{3n + 5}{6n - 5} \\
&= \frac{3 \cdot (n + 1) + 5}{6 \cdot (n + 1) - 5} = \underset{ n \to \infty }{ \frac{3n + 8}{6n + 1} } \approx \frac{1}{2} < 1 \implies x_{ n } \downarrow 
\end{aligned} \\ 
\frac{3n + 5 > 0}{6n - 5 > 0} \implies \frac{3n + 5}{6n - 5} > 0 \implies x_{ n } = \prod_{ i = 1 }^{ n } \frac{3n + 5}{6n - 5} > 0 \\ 
\begin{matrix}
x_{ n } \downarrow \\
x_{ n } > 0
\end{matrix} \implies x_{ n } \text{ converges} \\ 
\lim_{ n \to \infty } \prod_{ i = 1 }^{ n } \frac{3n + 5}{6n -5} = 0
}$$

## Exercise 163
**Point 1:** 
$$\displaylines{
x_{ n } = \frac{(2n)!!}{(2n + 1)!!} \\ 
\frac{x_{ n + 1 }}{x_{ n }} = \frac{(2n + 2)!!}{(2n + 3)!!} : \frac{(2n)!!}{(2n + 1)!!} = \frac{(2n + 2)!! \cdot (2n + 1)!!}{(2n + 3)!! \cdot (2n)!!} = \frac{(2n)!! \cdot (2n + 2) \cdot (2n + 1)!!}{(2n + 1)!! \cdot (2n + 3) \cdot (2n)!!} = \frac{2n + 2}{2n + 3} = 1 - \frac{1}{2n + 3} < 1 \implies x_{ n } \downarrow \\ 
\frac{(2n)!! > 0}{(2n + 1)!! >0} \implies x_{ n } = \frac{(2n)!!}{(2n + 1)!!} > 0   \\
\begin{matrix}
x_{ n } \downarrow  \\
x_{ n } > 0
\end{matrix} \implies x_{ n } \text{ converges} 
}$$

**Point 3:**
$$\displaylines{
x_{ n } = 1 + \frac{1}{2^{2}} + \frac{1}{3^{2}} + \dots + \frac{1}{n^{2}} = \sum_{ i =1 }^{ n } \frac{1}{n^{2}} \\ 
\frac{x_{ n + 1 }}{x_{ n }} = \frac{\sum_{ i }^{ n } \frac{1}{(n + 1)^{2}}}{\sum_{ i }^{ n } \frac{1}{n^{2}}} = \frac{\sum_{ i }^{ n } \frac{1}{n^{2}} + \frac{1}{(n + 1)^{2}}}{\sum_{ i }^{ n } \frac{1}{n^{2}}} = 1 + \frac{1}{\sum_{ i }^{ n } \frac{1}{n^{2}} \cdot (n + 1)^{2}} > 1 \implies x_{ n } \uparrow \\ 
\dots 
}$$

# Part 3 (Exercise 143)
**Cauchy Criteria:**
$$\displaylines{
\forall \epsilon > 0 \ \ \exists N \in \mathbb{N} :  \forall n > N, \ \ \forall p \in \mathbb{N} \implies |x_{ n + p } - x_{ n } | < \epsilon
}$$

**Point 1:**  
$$\displaylines{
x_{ n } = \frac{\sin a}{2} + \frac{\sin 2a}{2^{2}} + \frac{\sin 3a}{2^{ 3 }} + \dots + \frac{\sin na}{2^{ n }}, \ \ a \in \mathbb{R} \\
|x_{ n + p } - x_{ n }| = |\sum_{ k = n + 1 }^{ n + p } \frac{\sin(ka)}{2^{ k }}| \leq \sum_{ k = n + 1 }^{ n + p } \frac{1}{2^{ k }} \\ 
\text{Geometric series: } S = a + a \cdot r + a \cdot r^{2} + a \cdot r^{ 3 } + \dots \\ 
S - S \cdot r = (a + a \cdot r + a \cdot r^{2} + \dots) - (a \cdot r + a \cdot r^{2} + \dots) = a \\ 
S - S \cdot r = a \\ 
S \cdot (1 - r) = a \\ 
S = \frac{a}{1 - r} \\ 
|x_{ n + p } - x_{ n }| = \sum_{ k = n + 1 }^{ n + p } \frac{1}{2^{ k }} = \frac{\frac{1}{2^{ n + 1 }}}{1 - \frac{1}{2}}
}$$

**Point 3:**
$$\displaylines{
x_{ n } = \frac{1}{1 \cdot 2} - \frac{1}{2 \cdot 3} + \dots + \frac{(-1)^{ n - 1 }}{n \cdot (n + 1)}
}$$
# Part 4
**Point 1:** 
$$\displaylines{
\lim_{ n \to \infty } (n^{ 3 } + 1)^{ \frac{1}{\sqrt{ n }} } = \lim_{ n \to \infty } e^{ \frac{\ln(n^{ 3 } + 1)}{\sqrt{ n }} } = \lim_{ n \to \infty } e^{ \frac{3 \cdot \ln(n)}{n^{ \frac{1}{2} }} } = e^{ 0 } = 1
}$$

**Point 2:**
$$\displaylines{
\lim_{ n \to \infty } (n^{2} + n)^{ \frac{1}{\ln(n) + 2} } = \lim_{ n \to \infty } e^{ \frac{\ln(n^{2} + n)}{\ln(n) + 2} } = \lim_{ n \to \infty } e^{ \frac{2 \cdot \ln(n)}{\ln(n)} } = e^{2}
}$$




$$\displaylines{

}$$