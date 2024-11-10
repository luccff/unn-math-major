# Part 1 
## Paragraph 2, Exercise 10
### Exercise 10.1
$$\displaylines{
n \in \mathbb{N} \\
\frac{1}{n + 1} + \frac{1}{n + 2} + \dots + \frac{1}{3n + 1} > 1 \\ 
p(1) : \frac{1}{2} + \frac{1}{3} + \frac{1}{4} = \frac{13}{12} > 1 \text{ - true} \\ 
p(k) : \frac{1}{k + 1} + \dots + \frac{1}{3k + 1} > 1 \\ 
p(k + 1) : \frac{1}{k + 2} + \dots + \frac{1}{3k + 4} > 1 \\ 

\underbrace{ \underbrace{ \frac{1}{k + 1} + \dots + \frac{1}{3k + 1} }_{ \text{Left part p(k) > 1} } + \frac{1}{3k + 2} + \frac{1}{3k + 3} + \frac{1}{3k + 4} - \frac{1}{k + 1} }_{ \text{Left part p(k + 1)} } > 1 + \frac{1}{3k + 2} + \frac{1}{3k + 3} + \frac{1}{3k + 4} - \frac{1}{k + 1} = 1 + \underbrace{ \frac{2}{3 \cdot (k + 1) \cdot (3k + 2) \cdot (3k + 4)} }_{ > 0 } \\ 
\frac{1}{k + 2} + \dots + \frac{1}{3k + 4} > 1
}$$

### Exercise 10.2
$$\displaylines{
n \in \mathbb{N} \\ 
\frac{1}{n + 1} + \frac{1}{n + 2} + \dots + \frac{1}{2n} > \frac{13}{24} \\ 
p(1) : \frac{1}{2} > \frac{13}{24} \text{ - false}
}$$

### Exercise 10.3 
$$\displaylines{
n \in \mathbb{N} \\ 
\frac{1}{2} \cdot \frac{3}{4} \cdot \frac{5}{6} \cdot \dots \cdot \frac{2n - 1}{2n} < \frac{1}{\sqrt{ 3n + 1 }} \\ 
p(1) : \frac{1}{2} <  \frac{1}{\sqrt{ 4 }} \text{ - false}
}$$

### Exercise 10.4 
$$\displaylines{
n \in \mathbb{N} \\ 
\sqrt{ n } < 1 + \frac{1}{\sqrt{ 2 }} + \dots + \frac{1}{\sqrt{ n }} < 2 \sqrt{ n } \\ 
p(1) : \sqrt{ 1 } < 1 < 2 \text{ - false}
}$$

## Paragraph 2, Exercise 8 
### Exercise 8.3 
$$\displaylines{
n \in \mathbb{N} \\ 
6^{ 2n - 2 } + 3^{ n + 1 } + 3^{ n - 1 } \ \ \vdots \ \ 11 \\ 
p(1) : 1 + 9 + 1 = 11 \ \ \vdots \ \ 11 \text{ - true} \\ 
p(k) : 6^{ 2k - 2 } + 3^{ k + 1 } + 3^{ k - 1 } \ \ \vdots \ \ 11 \\ 
p(k + 1) : 6^{ 2k } + 3^{ k + 2 } + 3^{ k } \ \ \vdots \ \ 11 \\ 
6^{ 2k } + 3^{ k + 2 } + 3^{ k } = 6^{ 2k - 2 } \cdot 6^{2} + 3^{ k + 1 } \cdot 3 + 3^{ k - 1 } \cdot 3 = \\
= 3 \cdot (12 \cdot 6^{ 2k - 2 } + 3^{ k + 1 } + 3^{ k - 1 })
}$$

### Exercise 8.4 
$$\displaylines{
n \in \mathbb{N} \\ 
n^{ 5 } - n \ \ \vdots \ \ 5 \\ 
p(1) : 1 - 1 = 0 \ \ \vdots \ \ 5 \text{ - true} \\ 
p(k) : k^{ 5 } - k \ \ \vdots \ \ 5 \\ 
p(k + 1) : (k + 1)^{ 5 } - (k + 1) \ \ \vdots \ \ 5 \\ 
(k + 1)^{ 5 } - (k + 1) = k^{ 5 } + 5 k^{ 4 } + 10 k^{ 3 } + 10 k^{ 2 } + 4k = \\ 
= k^{ 5 }  - k + 5k^{ 4 } + 10k^{ 3 } + 10k^{2} + 5k = \\
= \underbrace{ (k^{ 5 }  - k) }_{ \ \ \vdots \ \ 5 } + \underbrace{ 5 \cdot (k^{ 4 } + 2k^{ 3 } + 2k^{2} + k) }_{ \ \ \vdots \ \ 5 } \ \ \vdots \ \ 5 
}$$

# Part 2 

## Exercise 2 
$$\displaylines{
1. \ \ 
\begin{pmatrix}
5 \\
3
\end{pmatrix} = \frac{5!}{3! \cdot 2!} = \frac{2 \cdot 3 \cdot 4 \cdot 5}{2 \cdot 2 \cdot 3} = \frac{4 \cdot 5}{2} = 10 \\ 
2. \ \ 
\begin{pmatrix}
6 \\
4
\end{pmatrix} = \frac{6!}{4! \cdot 2!} = \frac{2 \cdot 3 \cdot 4 \cdot 5 \cdot 6}{2 \cdot 2 \cdot 3 \cdot 4} = \frac{5 \cdot 6}{2} = 15 \\ 
3. \ \ 
\begin{pmatrix}
11 \\
5
\end{pmatrix} = \frac{11!}{5! \cdot 6!} = 462 \\ 
4. \ \ 
\begin{pmatrix}
3 \\
15
\end{pmatrix} = \frac{15!}{3! \cdot 12!} = 455
}$$

