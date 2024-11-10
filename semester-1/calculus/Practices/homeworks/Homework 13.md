# Part 2 
**Point 1:**
$$\displaylines{
\lim_{ x \to 3 } \frac{x + 2}{x - 1} = A \\ 
\forall x_{ n } \underset{ \neq }{ \to } 3 \implies \lim_{ n \to \infty } \frac{x_{ n } + 2}{x_{ n } - 1} = \left[ \frac{3 + 2}{3 - 1} \right] = \frac{5}{2} \implies A = \frac{5}{2}
}$$

**Point 2:**
$$\displaylines{
\lim_{ x \to 4 } \frac{x}{x - 4} = A \\ 
\forall x_{ n } \underset{ \neq }{ \to } 4 \implies \lim_{ n \to \infty } \frac{x_{ n }}{x_{ n } - 4} = \left[ \frac{4}{4 - 4} \right] = \infty \implies A = \infty
}$$

**Point 3:**
$$\displaylines{
\lim_{ x \to -2 }  \frac{x^{2} + 3x - 2}{x^{2} - 4} \\ 
\forall x_{ n } \underset{ \neq }{ \to } -2 \implies \lim_{ n \to \infty } \frac{x_{ n }^{2} + 3x_{ n } -2}{x_{ n }^{2} - 4} = \left[ \frac{4 - 6 - 2}{4 - 4} = - \frac{4}{0} \right] = -\infty \implies A = -\infty
}$$

# Part 3
**Point 1:**
$$\displaylines{
f(x) = \tan\left( \frac{1}{x} \right) \\ 
x_{ 0 } = 0 \\ 
x_{ n } = \frac{1}{n} \underset{ \neq }{ \to } 0 \\ 
\lim_{ n \to \infty } \tan\left( \frac{1}{x_{ n }} \right) = \lim_{ n \to \infty } \tan\left( \frac{1}{\frac{1}{n}} \right) = \lim_{ n \to \infty } \tan(n) = \frac{\pi}{2} \\ 
y_{ n } = -\frac{1}{n} \underset{ \neq }{ \to } 0 \\ 
\lim_{ n \to \infty } \left( \frac{1}{x_{ n }} \right) = \lim_{ n \to \infty } \tan\left( \frac{1}{-\frac{1}{n}} \right) = \lim_{ n \to \infty } \tan(-n) = - \frac{\pi}{2} \\ 
\frac{\pi}{2} \neq \left( -\frac{\pi}{2} \right) \implies \not \exists \lim_{ x \to 0 } \tan\left( \frac{1}{x} \right)
}$$

# Part 4
## Level 1
**Point 1:**
$$\displaylines{
\begin{aligned}
\lim_{ x \to +\infty } (3x^{3} - 2x \cdot (x - 1)^{2} + x^{2} \cdot (2 - \sqrt[3]{ x } + x)) &= \lim_{ x \to +\infty } (3x^{3} - 2x^{ 3 } + x^{ 3 }) \\
&= \lim_{ x \to +\infty } (2x^{ 3 }) \\
&= +\infty 
\end{aligned}
}$$

**Point 2:** 
$$\displaylines{
\dots
}$$

**Point 3:**
$$\displaylines{
\begin{aligned}
\lim_{ x \to +\infty } \frac{\sqrt[3]{ x^{ 6 } - 2x } - \sqrt{ 4x^{ 4 } + x + 1 }}{3 \cdot \sqrt{ x^{ 4 } - 1 } - \sqrt[5]{ x^{ 10 } + 11x^{ 9 } }} &= \lim_{ x \to +\infty } \frac{x^{2} - 2x^{2}}{3x^{2} - x^{2}} \\
&= \lim_{ x \to +\infty } \frac{-x^{2}}{2x^{2}} \\ 
&= - \frac{1}{2}
\end{aligned}
}$$

## Level 2
**Point 1:**
$$\displaylines{
\begin{aligned}
\lim_{ x \to +\infty } (\sqrt{ x + 4x^{2} } - \sqrt{ 4x^{2} - 5x - 1 }) &= \lim_{ x \to +\infty } \frac{x + 4x^{2} - 4x^{2} + 5x + 1}{\sqrt{ x + 4x^{2} } + \sqrt{ 4x^{2} - 5x - 1}} \\ 
&= \lim_{ x \to +\infty } \frac{6x}{4x} \\ 
&= \frac{6}{4} = \frac{3}{2}
\end{aligned}
}$$

**Point 2:**
$$\displaylines{
\begin{aligned}
\lim_{ x \to +\infty } (\sqrt[3]{ x^{ 6 } - 3x^{ 4 } } - \sqrt[3]{ x^{ 6 } + 2x^{ 3 } + x }) &= \lim_{ x \to \infty } \frac{x^{ 6 } - 3x^{ 4 } - x^{ 6 } - 2x^{ 3 } - x}{\sqrt[3]{ (x^{ 6 } - 3x^{ 4 })^{2} } + \sqrt[3]{ (x^{ 6 } - 3x^{ 4 }) \cdot (x^{ 6 } + 2x^{ 3 } + x) } + \sqrt[3]{ (x^{ 6 } + 2x^{ 3 } + x)^{2} }} \\ 
&= \lim_{ x \to +\infty } \frac{-3x^{ 4 }}{x^{ 4 } + x^{ 4 } + x^{ 4 }} \\
&= \lim_{ x \to +\infty } \frac{-3x^{ 4 }}{3x^{ 4 }} \\
&= -1
\end{aligned}
}$$

## Level 3
$$\displaylines{
\begin{aligned}
\lim_{ x \to +\infty } \left( \frac{3x^{ 5 } + 8^{ x } + 5 \cdot 6^{ x }}{64^{ \frac{x}{2} } + x^{ 6 } + 2^{ 3x - 2 }} - \frac{x^{ x } - 1000^{ x }}{2 - x^{ 3 } - x^{ x }} \right) &= \lim_{ x \to +\infty } \left( \frac{8^{ x }}{8^{ x }} - \frac{x^{ x }}{-x^{ x }}\right) \\
&= [1  + 1] \\ 
&= 2
\end{aligned}
}$$

## Level 4
**Point 1:**
$$\displaylines{
\begin{aligned}
\lim_{ x \to +\infty } \left( 1 - \frac{3x}{2x^{3} + 5} \right)^{ \frac{x^{ 3 } - 7x^{2}}{2x + 6} } &= \lim_{ x \to  +\infty } \left( \left( 1 + \frac{1}{-\frac{2x^{3} + 5}{3x}} \right)^{ -\frac{2x^{3} + 5}{3x} } \right) ^{ -\frac{3x}{2x^{3} + 5} \cdot \frac{x^{ 3 } - 7x^{2}}{2x + 6} } \\ 
&= \lim_{ x \to +\infty } e^{ -\frac{3x}{2x^{3} + 5} \cdot \frac{x^{ 3 } - 7x^{2}}{2x + 6} } \\ 
&= \lim_{ x \to +\infty } e^{ -\frac{3x^{ 4 }}{4x^{ 4 }} } \\ 
&= e^{ - \frac{3}{4} }
\end{aligned}
}$$

**Point 2:**
$$\displaylines{
\begin{aligned}
\lim_{ x \to +\infty } \left( \frac{3x^{ 6 } - 3x^{ 4 }}{3x^{ 6 } + 5x} \right)^{ 2x^{2} + x } &= 
\lim_{ x \to +\infty } \left( \frac{3x^{ 6 } + 5x - 3x^{ 4 } - 5x}{3x^{ 6 } + 5x} \right)^{ 2x^{2} + x } \\ 
&= \lim_{ x \to +\infty } \left( 1 + \frac{-3x^{ 4 } - 5x}{3x^{ 6 } + 5x} \right)^{ 2x^{2} + x } \\ 
&= \lim_{ x \to +\infty } e^{ - \frac{3x^{ 4 } + 5x}{3x^{ 6 } + 5x} \cdot 2x^{2}  + x } \\ 
&= \lim_{ x \to +\infty } e^{ - \frac{6x^{ 6 }}{3x^{ 6 }} } \\ 
&= e^{ -2 }
\end{aligned}
}$$

## Level 5
$$\displaylines{
\begin{aligned}
\lim_{ x \to +\infty } x^{ \frac{1}{x + 1} } &= \lim_{ x \to +\infty } e^{ \frac{1}{x + 1} \cdot \ln(x) } \\ 
&= \lim_{ x \to +\infty } e^{ 0 } = 1
\end{aligned}
}$$
