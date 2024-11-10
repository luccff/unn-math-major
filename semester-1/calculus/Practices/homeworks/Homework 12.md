# Exercise 117
**Point 2:**
$$\displaylines{
\text{Sequence: } x_{ n } = (-1)^{ n } \cdot \frac{3n - 1}{n + 2} \\ 
\text{Subsequences: } \\ 
x_{ 2k } = \frac{6k - 1}{2k + 2} \to 3 \\ 
x_{ 2k - 1 } = - \frac{6k - 4}{2k + 1} \to -3 \\ 
L(x_{ n }) = \{ -3, 3 \} \\ 
\sup x_{ n } = 3 \\ 
\inf x_{ n } = -3
}$$

**Point 4:**
$$\displaylines{
\text{Sequence: } x_{ n } = \frac{((-1)^{ n } - 1) \cdot n^{2} + n + 1}{n} \\ 
\text{Subsequences: } \\ 
x_{ 2k } = \frac{2k + 1}{2k} \to 1 \\ 
x_{ 2k - 1 } = \frac{-2 \cdot (2k - 1)^{2} + 2k}{2k - 1} = -\infty \\ 
L(x_{ n }) = \{ -\infty, 1 \} \\ 
\sup x_{ n } = \infty \\ 
\inf x_{ n } = -\infty
}$$

# Exercise 123
**Point 2:**
$$\displaylines{
x_{ n } = \frac{1 + (-1)^{ n } \cdot n}{n} \\ 
x_{ 2k } = \frac{1 + 2k}{2k} \to 1 \\ 
x_{ 2k - 1 } = \frac{1 - (2k - 1)}{2k - 1} = \frac{-2k + 2}{2k - 1} = -1 \\ 
L(x_{ n }) = \{ -1, 1 \} \\ 
\lim_{ n \to \infty } \sup x_{ n } = \sup L(x_{ n }) = 1 \\ 
\lim_{ n \to \infty } \inf x_{ n } = \inf L(x_{ n }) = -1 \\ 
\sup x_{ n } = 1.5 \\ 
\inf x_{ n } = -1 
}$$

**Point 4:**
$$\displaylines{
x_{ n } = \frac{1}{n} + \sin\left( \frac{\pi \cdot n}{3} \right) = \frac{1}{n} + \sin\left( \frac{2\pi \cdot n}{6} \right) \\ 
x_{ 6k } = \frac{1}{6k} + \sin\left( \frac{2\pi \cdot 6k}{6} \right) = \frac{1}{6k} \to 0 \\
x_{ 6k - 1 } = \frac{1}{6k - 1} + \sin\left( \frac{2\pi \cdot (6k - 1)}{6} \right) = \frac{1}{6k - 1} - \frac{\sqrt{ 3 }}{2} \to -\frac{\sqrt{ 3 }}{2} \\ 
x_{ 6k - 2 } = \frac{1}{6k - 2} + \sin\left( \frac{2\pi \cdot (6k - 2)}{6} \right) = \frac{1}{6k - 2} - \frac{\sqrt{ 3 }}{2} \to -\frac{\sqrt{ 3 }}{2} \\ 
x_{ 6k - 3 } = \frac{1}{6k - 3} + \sin\left( \frac{2\pi \cdot (6k - 3)}{6} \right) = \frac{1}{6k - 3} \to 0 \\
x_{ 6k - 4 } = \frac{1}{6k - 4} + \sin\left( \frac{2\pi \cdot (6k - 4)}{6} \right) = \frac{1}{6k - 4} + \frac{\sqrt{ 3 }}{2} \to \frac{\sqrt{ 3 }}{2} \\ 
x_{ 6k - 5 } = \frac{1}{6k - 5} + \sin\left( \frac{2\pi \cdot (6k - 5)}{6} \right) = \frac{1}{6k - 5} + \frac{\sqrt{ 3 }}{2} \to \frac{\sqrt{ 3 }}{2} \\ 
L(x_{ n }) = \left\{  -\frac{\sqrt{ 3 }}{2}, 0, \frac{\sqrt{ 3 }}{2}  \right\} \\ 
\lim_{ n \to \infty } \sup x_{ n } = \sup L(x_{ n }) = \frac{\sqrt{ 3 }}{2} \\ 
\lim_{ n \to \infty } \inf x_{ n } = \inf L(x_{ n }) = -\frac{\sqrt{ 3 }}{2} \\ 
\sup x_{ n }
}$$

