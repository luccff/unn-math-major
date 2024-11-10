# Part 1
## Calculate Limits At $x \to -\infty$
**Point 1:**
$$\displaylines{
\begin{aligned}
\lim_{ x \to -\infty } \left( \frac{2^{ x } + \frac{3}{x^{ 3 }} + 6}{3^{ x } + 3} \right)^{2} &= \lim_{ t \to +\infty } \left( \frac{2^{ -t } + \frac{3}{-t^{ 3 }} + 6}{3^{ -t } + 3} \right)^{2} \\ 
&= \lim_{ t \to +\infty } \left( \frac{\frac{1}{2^{ t }} + \frac{3}{-t^{ 3 }} + 6}{\frac{1}{3^{ t }} + 3} \right)^{2} \\
&= \left( \frac{6}{3} \right)^{2} = 2^{2} = 4
\end{aligned}
}$$

**Point 2:**
$$\displaylines{
\begin{aligned}
\lim_{ x \to -\infty } \frac{x + \sqrt{ 9x^{2} + x }}{3x + \sqrt{ x^{2} + 1 }} 
&= \lim_{ t \to +\infty } \frac{-t + \sqrt{ 9t^{2} - t }}{-3t + \sqrt{ t^{2} + 1 }} \\
&= \lim_{ t \to +\infty } \frac{-t + 3t}{-3t + t} \\ 
&= \lim_{ t \to +\infty } \frac{3t - t}{-(3t - t)} = -1
\end{aligned}
}$$

**Point 3:**
$$\displaylines{
\begin{aligned}
\lim_{ x \to -\infty } (\sqrt{ 5x + 4x^{2} } + 2x) 
&= \lim_{ t \to +\infty } (\sqrt{ 4t^{2} - 5t } - 2t) \\
&= \lim_{ t \to +\infty } \frac{4t^{2} - 5t - 4t^{2}}{\sqrt{ 4t^{2} - 5t } + 2t} \\
&= \lim_{ t \to +\infty } \frac{-5t}{2t + 2t} \\
&= -\lim_{ t \to +\infty } \frac{5t}{4t} = -\frac{5}{4}
\end{aligned}
}$$

**Point 4:**
$$\displaylines{
\begin{aligned}
\lim_{ x \to -\infty } \left( \frac{2x + 4}{2x + 1} \right)^{ 3x } 
&= \lim_{ t \to +\infty } \left( \frac{-2t + 4}{-2t + 1} \right)^{ -3t } \\
&= \lim_{ t \to +\infty } \left( 1 + \frac{3}{-2t + 1} \right)^{ -3t } \\
&= \lim_{ t \to +\infty } \left( 1 + \frac{1}{\frac{-2t + 1}{3}} \right)^{ -3t } \\ 
&= \lim_{ t \to +\infty } e^{ \frac{3}{-2t + 1} \cdot (-3t) } \\ 
&= \lim_{ t \to +\infty } e^{ \frac{9t}{2t} } = e^{ \frac{9}{2} }
\end{aligned}
}$$

## Calculate Limits At $x \to \infty$
**Point 1:**
$$\displaylines{
\lim_{ x \to \infty } \frac{5x^{ 3 } + 2x - 1}{6x - x^{2} + 2} = \lim_{ x \to \infty } \frac{5x^{ 3 }}{-x^{2}} = \infty
}$$

**Point 2:**
$$\displaylines{
\begin{aligned}
\lim_{ x \to \infty } \frac{5x^{ 7 } - 3x \cdot (x^{ 6 } - 2)}{x^{2} + 1 - x^{ 8 }} 
&= \lim_{ x \to \infty } \frac{5x^{ 7 } - 3x^{ 7 }}{-x^{ 8 }} \\
&= \lim_{ x \to \infty } \frac{2x^{ 7 }}{-x^{ 8 }} = 0
\end{aligned}
}$$

**Point 3:**
$$\displaylines{
\begin{aligned}
\lim_{ x \to \infty } \frac{x^{ 4 } + x \cdot (x - x^{ 3 } - 3x^{2})}{6x^{ 3 } - x \cdot (x^{2} + 2x)}
&= \lim_{ x \to \infty } \frac{x^{ 4 } - x^{ 4 } - 3x^{ 3 }}{6x^{ 3 } - x^{ 3 }} = \lim_{ x \to \infty } \frac{-3x^{ 3 }}{5x^{ 3 }} = -\frac{3}{5}
\end{aligned}
}$$

**Point 4:**
$$\displaylines{
\begin{aligned}
\lim_{ x \to \infty } \frac{5^{ x } - x^{2} + 1}{25^{ x + 1 } + 2x^{2}} 
&= \lim_{ x \to \infty } \frac{5^{ x }}{25^{ x + 1 }} \\
&= \lim_{ x \to \infty } \frac{5^{ x }}{25 \cdot 5^{ x } \cdot 5 ^{ x }} \\ 
&= \lim_{ x \to \infty } \frac{1}{25 \cdot 5^{ x }} = 0
\end{aligned}
}$$

**Point 5:**
$$\displaylines{
\begin{aligned}
\lim_{ x \to \infty } \sqrt{ x^{2} + x } - x 
&= \lim_{ x \to \infty } \frac{x^{2} + x - x^{2}}{\sqrt{ x^{2} + x } + x} \\ 
&= \lim_{ x \to \infty } \frac{x}{x + x} = \frac{1}{2}
\end{aligned}
}$$

# Part 2 
**Definition Of A Limit:**
$$\displaylines{
\lim_{ x \to a } = A \Leftrightarrow \forall \epsilon > 0 \ \ \exists \delta > 0 \ \ \forall x \in D_{ f } \cap U_{ \delta }^{ o }(a) \implies f(x) \in U_{ \epsilon }(A)
}$$

