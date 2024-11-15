# Supremum and Infinum
## Exercise 1 
$$\displaylines{
A = \left\{  -1 - \frac{6}{n + 1}  \mid n \in \mathbb{N} \right\} \\ 
1. \ \ -7 = \inf A \Leftrightarrow 
\begin{cases}
\forall x \in A \implies -7 \leq x \\
\forall \epsilon > 0 \ \ \exists x \in A \implies -7 + e > x \\ 
\end{cases} \\ 
2. \ \ 
\begin{cases}
-7 = \inf A \\
-7 \in A, \ \ n = 0 
\end{cases} \implies -7 = \min A \\ 
3. \ \ -1 = \sup A \Leftrightarrow 
\begin{cases}
\forall x \in A \implies x < -1 \\
\forall \epsilon > 0 \ \ \exists x(\epsilon) \in A \implies -1 - \epsilon < x(\epsilon)
\end{cases} \\ 
-1 - \epsilon < - 1 - \frac{6}{n + 1} \\ 
\epsilon > \frac{6}{n + 1} \\ 
(n + 1) \cdot \epsilon > 6 \\ 
n + 1 > \frac{6}{\epsilon} \\ 
n > \frac{6 - \epsilon}{\epsilon} \\ 
n(\epsilon) = \left[ \frac{6 - \epsilon}{\epsilon} \right] + 1 \\ 
x(\epsilon) = -1 - \frac{6}{n(\epsilon) + 1} = -1 - \frac{6}{\left[ \frac{6 - \epsilon}{\epsilon} \right] + 2} \\
4. \ \ 
\begin{cases}
-1 = \sup A \\
-1 \not\in A
\end{cases} \implies \not \exists \max A
}$$

## Exercise 2 
$$\displaylines{
A = [2; 10) \\ 
1. \ \ 2 = \inf A \implies 
\begin{cases}
\forall x \in A \implies 2 \leq x \\
\forall \epsilon > 0 \ \ \exists x \in A \implies 2 + \epsilon > x 
\end{cases} \\ 
2. \ \ 2 = \min A \Leftrightarrow 
\begin{cases}
2 = \inf A \\
2 \in A
\end{cases} \\ 
3. \ \ 10 = \sup A \Leftrightarrow 
\begin{cases}
\forall x \in A \implies x < 10 \\
\forall \epsilon > 0 \ \ \exists x(\epsilon) \implies 10 - \epsilon < x(\epsilon)
\end{cases} \\ 
x(\epsilon) > 10 - \epsilon \\ 
x(\epsilon) = 
\begin{cases}
x(\epsilon) = 2, \ \ \epsilon \geq 8 \\ \\
x(\epsilon) = 10 - \frac{\epsilon}{2}, \ \ \epsilon < 8
\end{cases} \\ 
4. \ \ 
\begin{cases}
10 = \sup A \\
10 \not\in A
\end{cases} \implies \not \exists \max A
}$$

# Mathematical Induction 
## Exercise 1 
$$\displaylines{
n \in \mathbb{N} \\ 
1 \cdot 2 + 2 \cdot 5 + \dots + n(3n - 1) = n^{2} \cdot (n + 1) \\ 
1. \ \ n = 1 \implies 
\begin{matrix}
1 \cdot (3 - 1) = 2 \\
1^{2} \cdot (1 + 1) = 2
\end{matrix} \implies \text{При } n = 1 \text{ формула верна.} \\ 
2. \ \ n = k \implies 1 \cdot 2 + 2 \cdot 5 + \dots + k \cdot (3k - 1) = k^{2} \cdot (k + 1) \\ 
3. \ \ n = k + 1 \implies 1 \cdot 2 + 2 \cdot 5 + \dots + k \cdot (3k - 1) + (k + 1) \cdot (3k + 2) = (k + 1)^{2} \cdot (k + 2) \\ 
k^{2} \cdot (k + 1) + (k + 1) \cdot (3k + 2) = (k + 1)^{2} \cdot (k + 2) \\ 
(k + 1) \cdot (k^{2} + 3k + 2) = (k + 1) \cdot (k + 1) \cdot (k + 2) = (k + 1)^{2} \cdot (k + 2) \\
(k + 1)^{2} \cdot (k + 2) = (k + 1)^{2} \cdot (k + 2) \implies \text{ Формула верна для всех } n \in \mathbb{N}
}$$

## Exercise 2
$$\displaylines{
1^{2} + 3^{2} + \dots + (2n - 1)^{2} = \frac{n \cdot (4n^{2} - 1 )}{3} \\ 
1. \ \ n = 1 \implies 1 = \frac{1 \cdot (4 - 1)}{3} = 1 \text{ при } n = 1 \text{ формула верна} \\ 
2. \ \ n = k \implies 1^{2} + 3^{2} + \dots + (2k - 1)^{2} = \frac{k \cdot (4k^{2} - 1)}{3} \\ 
3. \ \ n = (k + 1) \implies 1^{2} + 3^{2} + \dots + (2k - 1)^{2} + (2k + 1)^{2} = \frac{(k + 1) \cdot (4(k + 1)^{2}  - 1)}{3} \\ 
\frac{k \cdot (4k^{2} - 1)}{3} + (2k + 1)^{2} = \frac{(k + 1) \cdot (4(k + 1)^{2}  - 1)}{3} \\ 
\frac{k \cdot (2k - 1) \cdot (2k + 1)}{3} + (2k + 1)^{2} = \frac{2k + 1}{3} \cdot (k \cdot (2k - 1) + 3(2k + 1)) = \\
= \frac{2k + 1}{3} \cdot (2k + 3) \cdot (k + 1) = \frac{(2k + 1) \cdot (2k + 3) \cdot (k + 1)}{3} \implies \\ \implies \text{Формула верна для всех } n \in \mathbb{N}
}$$

## Exercise 3 
$$\displaylines{
\text{Equation:} \\ 
1 \cdot 2 + 2 \cdot 3 + 3 \cdot 4 + \dots + (n - 1) \cdot n = \frac{(n - 1) \cdot n \cdot (n  + 1)}{3}, \ \ n \in \mathbb{N} \\ 
1. \ \ n = 1 \implies 0 \cdot 1 = \frac{0}{3} \text{ - true} \\ 
2. \ \ n = k \implies 1 \cdot 2 + \dots + (k - 1) \cdot k = \frac{(k - 1) \cdot k \cdot (k+ 1)}{3} \\ 
3. \ \ n = k + 1 \implies 1 \cdot 2 + \dots + k \cdot (k + 1) = \frac{k \cdot (k + 1) \cdot (k + 2)}{3} \\ 
\frac{(k - 1) \cdot k \cdot (k + 1)}{3} + k \cdot (k + 1) = \frac{(k - 1) \cdot k \cdot (k + 1) + 3k \cdot (k + 1)}{3} = \\ 
= \frac{k^{3} + 3k^{2} + 2k}{3} = \frac{k \cdot (k + 1) \cdot (k + 2)}{3}
}$$

## Exercise 4 
$$\displaylines{
1^{3} + 2^{3} + 3^{3} + \dots + n^{3} = \left( \frac{n \cdot (n + 1)}{2} \right)^{2}, \ \ n \in \mathbb{N} \\ 
1. \ \ n = 0 \implies 0^{3} = \left( \frac{0}{2} \right)^{2} \text{ - true} \\ 
2. \ \ n = k \implies 1^{3} + \dots + k^{3} = \left( \frac{k \cdot (k + 1)}{2} \right)^{2} \\ 
3. \ \ n = k + 1 \implies 1^{3} + \dots + (k + 1)^{3} = \left( \frac{(k + 1) \cdot (k + 2)}{2} \right)^{2} \\ 
\left( \frac{k \cdot (k + 1)}{2} \right)^{2} + (k + 1)^{3} = \frac{k^{2} \cdot (k + 1)^{2} + 4(k + 1)^{3}}{4} = \frac{(k + 1)^{2} \cdot (k^{2} + 4(k  +1))}{4} = \\
= \frac{(k + 1)^{2} \cdot (k^{2} + 4k + 4)}{4} = \frac{(k + 1)^{2} \cdot (k + 2)^{2}}{4} = \left( \frac{(k + 1) \cdot (k + 2)}{2} \right)^{ 2 }
}$$

