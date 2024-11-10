# Part 1

## Identify Indeterminate Form 
**Exercise 1:** 
$$\displaylines{
\lim_{ n \to \infty } \ln n - n = \infty - \infty 
}$$

**Exercise 2:**
$$\displaylines{ 
\lim_{ n \to \infty } \sqrt[n]{ n + 3 } = \infty^{ \frac{1}{\infty} } = \infty^{ 0 }
}$$

**Exercise 3:**
$$\displaylines{
\lim_{ n \to \infty } \left( 1 - \frac{2}{n} \right)^{ n } = 1^{ \infty }
}$$

**Exercise 4:**
$$\displaylines{
\lim_{ n \to \infty } \frac{n + n^{2}}{n! + n}  = \frac{\infty}{\infty}
}$$

**Exercise 5:**
$$\displaylines{
\lim_{ n \to \infty } \frac{\frac{1}{n} + \frac{2}{\sqrt{ n }}}{ \frac{2}{5^{ n }} } = \frac{0}{0}
}$$

**Exercise 6:**
$$\displaylines{
\lim_{ n \to \infty } \left( 1 - \frac{1 + n}{n} \right)^{ \frac{1}{n + \sqrt{ n }} } = \lim_{ n \to \infty } \left( \frac{1}{n} \right)^{ \frac{1}{n + \sqrt{ n }} } = 0^{ 0 }
}$$

## Solve Indeterminate Form 
**Exercise 1:**
$$\displaylines{
\begin{aligned}
\lim_{ n \to \infty } (2n^{ 3 } - 5n^{ 4 }\sqrt{ n } - 2n) &= \lim_{ n \to \infty } \left( 2n^{ 3 } - 5n^{ 3 + \frac{3}{2} } - 2n \right) \\ 
&= \lim_{ n \to \infty } n^{ 3 } \cdot \left( 2 - 5n^{ \frac{3}{2} } - \frac{2}{n^{2}} \right) \\ 
&= \lim_{ n \to \infty } n^{ 3 } \cdot \lim_{ n \to \infty } \left( 2 - 5n^{ \frac{3}{2} } - \frac{2}{n^{2}} \right) \\ 
&= \infty \cdot (2 - \infty) = \infty \cdot (-\infty) = -\infty
\end{aligned}
}$$

**Exercise 2:** 
$$\displaylines{
\begin{aligned}
\lim_{ n \to \infty } \left( \sqrt{ n } \cdot \sqrt[3]{ n } - 2 \cdot \frac{n}{\sqrt[4]{ n \cdot \sqrt{ n }}} + \sqrt[5]{ n^{ 4 } } \right) &= \lim_{ n \to \infty } \left( n^{ \frac{5}{6} } - 2 \cdot n^{ \frac{5}{8} } + n^{ \frac{4}{5} } \right) \\ 
&= \lim_{ n \to \infty } n^{ \frac{5}{6} } \cdot \lim_{ n \to \infty } \left( 1 - 2 \cdot n^{ -\frac{5}{24} } + n^{ - \frac{1}{30} } \right) \\ 
&= \lim_{ n \to \infty } n^{ \frac{5}{6} } \cdot \lim_{ n \to \infty } \left( 1 - \frac{2}{n^{ \frac{5}{24} }} + \frac{1}{n^{ \frac{1}{30} }} \right) \\ 
&= 1 \cdot \infty = \infty
\end{aligned}
}$$

**Exercise 3:**
$$\displaylines{
\begin{aligned}
\lim_{ n \to \infty } \left( n^{ 3 } \cdot (n^{2} - 2n + 3) - n^{ 4 } \cdot \left( n - 2 + \frac{1}{n} \right) - 3n^{2} \right) &= \lim_{ n \to \infty } (2n^{ 3 } - 3n^{2}) \\
&= \lim_{ n \to \infty } n^{ 3 } \cdot \left( 2 - \frac{3}{n} \right) \\ 
&= \lim_{ n \to \infty } n^{ 3 } \cdot \lim_{ n \to \infty } \left( 2 - \frac{3}{n} \right) \\ 
&= 2 \cdot \infty = \infty 
\end{aligned}
}$$

# Part 2 
## Calculate The Limit 
**Exercise 1:**
$$\displaylines{
\lim_{ n \to \infty } \frac{2 + \frac{1}{n} + \frac{3}{n^{2}}}{4 - \frac{2}{n} - \frac{5}{n^{ 3 }}} = \frac{1}{2}
}$$

**Exercise 2:**
$$\displaylines{
\lim_{ n \to \infty } \frac{5 + \frac{3n - 2}{n} - \frac{3}{n^{2}} \cdot n}{4 - \left( \frac{2}{n} + 3 \right) \cdot \left( 2 - \frac{3}{2^{ n }} \right) - \frac{5}{n!}} = \frac{8}{-2} = -4
}$$

**Exercise 3:** 
$$\displaylines{
\lim_{ n \to \infty } \frac{2 + \frac{1}{\sqrt{ n }} + \left( 2 + \frac{100}{n^{ n }} \right)^{ 2 - \frac{5}{n} }}{1 - \frac{2}{n^{ 3 }} - \frac{5}{e^{ n }}} = 6
}$$

**Exercise 4:**
$$\displaylines{
\lim_{ n \to \infty } \left( 3 + \frac{2}{n!} - \frac{\sin n}{\sqrt[9]{ n }} \right)^{ \frac{3}{n} - 1 } = \frac{1}{3}
}$$

**Exercise 5:** 
$$\displaylines{
\lim_{ n \to \infty } \left( \frac{3}{4^{ n }} + \frac{2}{n!} \right)^{ 5 - \frac{1}{n} } = 0
}$$

## Calculate The Limit 
**Exercise 1:**
$$\displaylines{
\lim_{ n \to \infty } \frac{n + \frac{1}{n} + 2}{4 - \frac{2}{n}} = \infty 
}$$

**Exercise 2:**
$$\displaylines{
\lim_{ n \to \infty } \left( n^{2} + n - 7 - \frac{10}{\sqrt[7]{ n^{ 3 } }} \right)^{2} = \infty
}$$

**Exercise 3:**
$$\displaylines{
\lim_{ n \to \infty } \left( 3 - n^{2} + \frac{4 \cdot (-1)^{ n }}{1.2^{ n }} \right) = -\infty 
}$$

**Exercise 4:**
$$\displaylines{
\lim_{ n \to \infty } \left( n + 1 + \frac{2 \cos n}{n^{ n }} \right)^{ \frac{3}{7n} -2 } = \infty^{ -2 } = 0
}$$

**Exercise 5:**
$$\displaylines{
\lim_{ n \to \infty } \left( 2^{ n } - 1000 + \frac{2}{n!} \right)^{ \frac{3}{n} - 2n } = \infty^{ -\infty } = 0
}$$

**Exercise 6:**
$$\displaylines{
\lim_{ n \to \infty } \left( \frac{3 - \frac{\sin 2n}{3 + n!}}{\frac{1}{n} + \frac{2}{n^{2}} + \frac{3}{n + n!}} \right)^{ 2 - \frac{4}{n} } = \infty
}$$

