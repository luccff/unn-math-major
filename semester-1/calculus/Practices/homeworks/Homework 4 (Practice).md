# Exercise 20 
## Exercise 20.3
$$\displaylines{
\begin{aligned}
(a + b)^6 &= \binom{6}{0}a^6b^0 + \binom{6}{1}a^5b^1 + \binom{6}{2}a^4b^2 + \binom{6}{3}a^3b^3 \\
&\quad + \binom{6}{4}a^2b^4 + \binom{6}{5}a^1b^5 + \binom{6}{6}a^0b^6 \\
&= 1a^6 + 6a^5b + 15a^4b^2 + 20a^3b^3 + 15a^2b^4 + 6ab^5 + 1b^6 \\
&= a^6 + 6a^5b + 15a^4b^2 + 20a^3b^3 + 15a^2b^4 + 6ab^5 + b^6
\end{aligned}
}$$

## Exercise 20.4
$$\displaylines{
\begin{aligned}
(x + y)^7 &= \binom{7}{0}x^7y^0 + \binom{7}{1}x^6y^1 + \binom{7}{2}x^5y^2 + \binom{7}{3}x^4y^3 \\
&\quad + \binom{7}{4}x^3y^4 + \binom{7}{5}x^2y^5 + \binom{7}{6}x^1y^6 + \binom{7}{7}x^0y^7 \\
&= 1x^7 + 7x^6y + 21x^5y^2 + 35x^4y^3 + 35x^3y^4 + 21x^2y^5 + 7xy^6 + 1y^7 \\
&= x^7 + 7x^6y + 21x^5y^2 + 35x^4y^3 + 35x^3y^4 + 21x^2y^5 + 7xy^6 + y^7
\end{aligned}
}$$

## Exercise 20.5 
$$\displaylines{
\begin{aligned}
(a - b)^8 &= \binom{8}{0}a^8(-b)^0 + \binom{8}{1}a^7(-b)^1 + \binom{8}{2}a^6(-b)^2 + \binom{8}{3}a^5(-b)^3 \\
&\quad + \binom{8}{4}a^4(-b)^4 + \binom{8}{5}a^3(-b)^5 + \binom{8}{6}a^2(-b)^6 + \binom{8}{7}a^1(-b)^7 + \binom{8}{8}a^0(-b)^8 \\
&= 1a^8 - 8a^7b + 28a^6b^2 - 56a^5b^3 + 70a^4b^4 - 56a^3b^5 + 28a^2b^6 - 8ab^7 + b^8 \\
&= a^8 - 8a^7b + 28a^6b^2 - 56a^5b^3 + 70a^4b^4 - 56a^3b^5 + 28a^2b^6 - 8ab^7 + b^8
\end{aligned}
}$$

# Exercise 25.1 
$$\displaylines{
(\sqrt{2} + \sqrt[3]{5})^5 = \sum_{k=0}^{5} \binom{5}{k} (\sqrt{2})^{5-k} (\sqrt[3]{5})^k \\
1. \ \ k = 0: \binom{5}{0} (\sqrt{2})^5 (\sqrt[3]{5})^0 = 4\sqrt{2} \\
2. \ \ k = 1: \binom{5}{1} (\sqrt{2})^4 (\sqrt[3]{5})^1 = 20\sqrt[3]{5} \\ 
3. \ \ k = 2: \binom{5}{2} (\sqrt{2})^3 (\sqrt[3]{5})^2 = 10 \cdot 2\sqrt{2} \cdot 5^{2/3} \\
4. \ \ k = 3 \binom{5}{3} (\sqrt{2})^2 (\sqrt[3]{5})^3 = 100 \\
5. \ \ k = 4 \binom{5}{4} (\sqrt{2})^1 (\sqrt[3]{5})^4 = 5\sqrt{2} \cdot 5^{4/3} \\
6. \ \ k = 5 \binom{5}{5} (\sqrt{2})^0 (\sqrt[3]{5})^5 = 3125 \\
\text{Answer: } 100, \ 3125
}$$

# Exercise 26 
## Exercise 26.1
$$\displaylines{
\left( \frac{1}{4} + \frac{3}{4} \right)^{ 4 }
}$$

$$\displaylines{
\left( \frac{1}{4} + \frac{3}{4} \right)^4 \\ 
(a + b)^n = \sum_{k=0}^{n} \binom{n}{k} a^{n-k} b^k \\ 
\left( \frac{1}{4} + \frac{3}{4} \right)^4 = \sum_{k=0}^{4} \binom{4}{k} \left( \frac{1}{4} \right)^{4-k} \left( \frac{3}{4} \right)^k \\ 
T_k = \binom{4}{k} \cdot \frac{1^{4-k} \cdot 3^k}{4^4} \\
\begin{aligned}
T_0 &: \binom{4}{0} \cdot 3^0 = 1 \cdot 1 = 1 \\
T_1 &: \binom{4}{1} \cdot 3^1 = 4 \cdot 3 = 12 \\
T_2 &: \binom{4}{2} \cdot 3^2 = 6 \cdot 9 = 54 \\
T_3 &: \binom{4}{3} \cdot 3^3 = 4 \cdot 27 = 108 \\
T_4 &: \binom{4}{4} \cdot 3^4 = 1 \cdot 81 = 81
\end{aligned} \\ 
\text{Answer: 108}
}$$

## Exercise 26.2
$$\displaylines{
\left( \frac{1}{3} + \frac{2}{3}x \right)^{10} = \sum_{k=0}^{10} \binom{10}{k} \left( \frac{1}{3} \right)^{10-k} \left( \frac{2}{3}x \right)^k \\ 
\begin{align}
&T_k = \binom{10}{k} \cdot \frac{1^{10-k} \cdot 2^k}{3^{10}} x^k \\ 
&T_0: \binom{10}{0} \cdot 2^0 = 1 \\
&T_1: \binom{10}{1} \cdot 2^1 = 10 \cdot 2 = 20 \\
&T_2: \binom{10}{2} \cdot 2^2 = 45 \cdot 4 = 180 \\
&T_3: \binom{10}{3} \cdot 2^3 = 120 \cdot 8 = 960 \\
&T_4: \binom{10}{4} \cdot 2^4 = 210 \cdot 16 = 3360 \\ 
&T_5: \binom{10}{5} \cdot 2^5 = 252 \cdot 32 = 8064 \\
&T_6: \binom{10}{6} \cdot 2^6 = 210 \cdot 64 = 13440 \\
&T_7: \binom{10}{7} \cdot 2^7 = 120 \cdot 128 = 15360 \\ 
&T_8: \binom{10}{8} \cdot 2^8 = 45 \cdot 256 = 11520 \\ 
&T_9: \binom{10}{9} \cdot 2^9 = 10 \cdot 512 = 5120 \\
&T_{10}: \binom{10}{10} \cdot 2^{10} = 1 \cdot 1024 = 1024 \\
\end{align} \\
\text{Answer: } 15360
}$$
