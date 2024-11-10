# Exercise 1.1
1. $b \subseteq \{ a, b \}$ - false
2. $b \in \{ a, b \}$ - true
3. $\{ b \} \subseteq \{ a, b \}$ - true 
4. $\{ b \} \in \{ a, b \}$ - false
5. $b \subseteq \{ a, \{ b \} \}$ - false 
6. $b \in \{ a, \{ b \} \}$ - false 
7. $\{  b \} \subseteq \{ a, \{ b \} \}$ - false 
8. $\{ b \} \in \{ a, \{ b \} \}$ - true
9. $\emptyset \in \{ \emptyset \}$ - true 
10. $\emptyset \subseteq \{ \emptyset \}$ - true 
11. $\emptyset \in \emptyset$ - false 
12. $\emptyset \subseteq \emptyset$ - false 

# Exercise 1.2 
1. $A = \{ 1, 2, 3, \{ 1, 2, 3 \} \}, \ \ |A| = 4$
2. $A = \{ 1, \{ 1 \}, 2, \{ 1, \{ 2, 3 \} \}, \emptyset \}, \ \ |A| = 5$
3. $|\emptyset| = 0$ 
4. $A = \{ \emptyset \}, \ \ |A| = 1$
5. $A = \{ \emptyset, \{ \emptyset \} \}, \ \ |A| = 2$
6. $A = \{ \{ \emptyset, \{ \emptyset \} \} \}, \ \ |A| = 1$

# Exercise 1.3 
$$\displaylines{
a \in A \text{ and } a \in B \text{, } a \not\in C \\ 
1. \ \ a \in (B - C) \\ 
2. \ \ a \not\in (C - B) \\ 
3. \ \ a \in A \text{ and } a \in (B \cup C) \implies a \not\in A - (B \cup C) \\ 
4. \ \ a \in (A \cup B) \text{ and } a \not\in C \implies a \in (A \cup B) \Delta C \\ 
5. \ \ a \in B \Delta C \\ 
6. \ \ a \not\in A \Delta B \\ 
7. \ \ a \in (A \cap B) \text{ and } a \not\in C \implies a \in (A \cap B) \Delta C \\ 
8. \ \ a \in B \text{ and } a \in (A - C) \implies a \in B \cap (A - C)
}$$

# Exercise 1.4 
$$\displaylines{
U = \{ 1, 2, 3, 4, 5, 6, 7, 8 \} \\ 
A = \{ x \mid 2 < x \leq 6 \} = \{ 3, 4, 5, 6 \} \\ 
B = \{ x \mid \text{x is even} \} = \{ 2, 4, 6, 8 \} \\ 
C = \{ x \mid x \geq 4 \} = \{ 4, 5, 6, 7, 8 \} \\ 
D = \{ 1, 2, 4 \} \\ \\ 

1. \ \ A \cup B = \{ 3, 4, 5, 6 \} \cup \{ 2, 4, 6, 8 \} = \{ 3, 4, 5, 6, 2, 8 \} \\ 
2. \ \ C \cap D = \{ 4, 5, 6, 7, 8 \} \cap \{ 1, 2, 4 \} = \{ 4 \} \\ 
3. \ \ B \Delta C = \{ 2, 4, 6, 8 \} \Delta \{ 4, 5, 6, 7, 8 \} = \{ 2, 8, 5, 7 \} \\ 
4. \ \ \overline{A} \cap (\overline{B \cap D}) = \{ 1, 2, 7, 8 \} \cap \{ 1, 3, 5, 6, 7, 8 \} = \{ 1, 7, 8 \}\\ 
\overline{A} = \{ 1, 2, 7, 8 \} \\ 
B \cap D = \{ 2, 4 \} \\ 
\overline{B \cap D} = \{ 1, 3, 5, 6, 7, 8 \} \\ 
5. \ \ (A - B) \cup (C - D) = \{ 3, 5 \} \cup \{ 5, 6, 7, 8 \} = \{ 3, 5, 6, 7, 8 \}\\ 
A - B = \{ 3, 5 \} \\ 
C - D = \{ 5, 6, 7, 8 \} \\ 
6. \ \ \overline{\overline{A} \cup \overline{B} \cup \overline{C}} = \overline{\{ 1, 2, 3, 5, 7, 8 \}} = \{ 4, 6 \} \\
\overline{A} = \{ 1, 2, 7, 8 \} \\ 
\overline{B} = \{ 1, 3, 5, 7 \} \\ 
\overline{C} = \{ 1, 2, 3 \} \\ 
7. \ \ 2^{ A } \cap 2^{ B } \text{ (It was solved by me in the class)} \\ 
8. \ \ 2^{ D } - 2^{ B } = \{\{ \emptyset \}, \{ 1 \}, \{ 2 \}, \{ 4 \}, \{ 1, 2 \}, \{ 1, 4 \}, \{ 2, 4 \}, \{ 1, 2, 4 \} \} - 2^{ B \text{ (even numbers)} } = \\
= \{ \{ 1 \}, \{ 1, 2 \}, \{ 1, 4 \}, \{ 1, 2, 4 \} \}
}$$

# Exercise 1.5 
... 

# Exercise 1.6 
$$\displaylines{
|B| = 16, \ \ |B \cap C| = 9, \ \ |A \cap B \cap C| = 5 \\ 
1. \ \ |B - A \cap C| = 16 - 5 = 11 \\ 
2. \ \ |(A \cup (B \Delta C)) \cap B| = 16 - 9 = 7 
}$$

# Exercise 1.7
$$\displaylines{
M_{2} = \{ x \mid x \ \ \vdots \ \ 2 \} \\ 
M_{3} = \{ x \mid x \ \ \vdots \ \ 3 \} \\ 
M_{ 5 } = \{ x \mid x \ \ \vdots \ \ 5 \} \\ 
1. \ \ M_{2} \cap M_{3} \\ 
2. \ \ \overline{M_{2} \cup M_{3} \cup M_{5}} \\ 
3. \ \ M_{2} \cap M_{5} - M_{3} \\ 
4. \ \ 45 \in (M_{3} \cap M_{5}) \\ 
5. \ \ 42 \in (M_{2} \cap M_{3} - M_{5}) \\ 
6. \ \ \{ 8, 9, 10 \} \subseteq (M_{2} \cup M_{3} \cup M_{5}) - (M_{2} \cap M_{3})
}$$

# Exercise 1.8 
**Difference:** 
$$\displaylines{
A - B \stackrel{?}{=} B - C \\ 
\text{Suppose } A = \{ 1, 2, 3, 4, 5 \} \text{ and } B = \{ 3, 4, 5, 6 \} \\
\begin{matrix}
A - B = \{ 1, 2, 5 \} \\ 
B - A = \{ 6 \}
\end{matrix} \implies 
A - B \not= B - A \\ \\ 

A - (B - C) \stackrel{?}{=} (A - B) - C \\ 
\begin{matrix}
A - (B - C) \text{ includes elements in A, but not in B, unless they are in C} \\ 
(A - B) - C \text{ includes elements in A that are neither in B nor in C}
\end{matrix} \implies A - (B - C) \neq (A - B) - C
}$$

**Symmetric Difference:**
$$\displaylines{
A \Delta B \stackrel{?}{=} B \Delta A \\ 
A \Delta B = (A - B) \cup (B - A) \\
B \Delta A = (B - A) \cup (A - B) \\ 
(A - B) \cup (B - A) = (B - A) \cup (A - B) \implies A \Delta B = B \Delta A \\ \\ 

A \Delta (B \Delta C) \stackrel{?}{=} (A \Delta B) \Delta C \\ 
1. \ \ \text{Left side:} \\ 
\begin{matrix}
A \Delta (B \Delta C) \Leftrightarrow x \in A \text{ or } x \in B \Delta C \text{, but not in both.} \\ 
B \Delta C \Leftrightarrow x \in B \text{ or } x \in C \text{, but not in both}
\end{matrix} \implies \text{x strictly belongs to one of the sets} \\ 
2. \ \ \text{Right side:} \\ 
\begin{matrix}
(A \Delta B) \Delta C \Leftrightarrow x \in (A \Delta B) \text{ or } x \in C \text{, but not in both} \\
A \Delta B \Leftrightarrow x \in A \text{ or } x \in B \text{, but not in both}
\end{matrix} \implies \text{x strictly belongs to one of the sets} \\ 
\text{Left side = Right side} \implies A \Delta (B \Delta C) = (A \Delta B) \Delta C \\ 
}$$

# Exercise 1.9 
$$\displaylines{
A - (B \cup C) = (A - B) \cup (A - C)
}$$
$$\displaylines{
A - (B \cap C) = (A - B) \cap (A - C)
}$$
$$\displaylines{
A \cap (B \Delta C) = (A \cap B) \Delta (A \cap C)
}$$
$$\displaylines{
A \cup (B \Delta C) = (A \cup B) \Delta (A \cup C)
}$$
... 

# Exercise 1.10
**Identity 1:**
$$\displaylines{
A \cup AB = A \\ 
A \cup AB = AU \cup AB \\ 
A(U \cup B) \\ 
A \cap U = A 
}$$

**Identity 2:**
$$\displaylines{
A(A \cup B) = A \\ 
A(A \cup B) = AA \cup AB = A \cup AB = A 
}$$

**Identity 3:**
$$\displaylines{
A \cup \overline{A} B = A \cup B \\ 
A \cup B = (A \cup B) \cap U  = (A \cup B) \cap (A \cup \overline{A}) = \\ 
= \underset{ A }{ A \cup AB } \cup \overline{A}B = A \cup \overline{A}B 
}$$
**Identity 4:**
$$\displaylines{ 
A - (A - B) = AB \\ 
A - (A - B) = A \cap \overline{A \cap \overline{B}} = A \cap (\overline{A} \cup B) =  A \cap \overline{A} \cup AB = \emptyset \cup AB = AB
}$$

**Indentity 5:**
$$\displaylines{
A - A \cap B = A - B \\ 
\text{Right side: } A - B = A \cap \overline{B} \\ 
\text{Left side: } A \cap \overline{A \cap B} =  A \cap (\overline{A} \cup \overline{B}) = (A \cap \overline{A}) \cup (A \cap \overline{B}) = \emptyset \cup (A \cap \overline{B}) = A \cap \overline{B}
}$$

**Identity 6:**
$$\displaylines{
A \cup (B - A) = A \cup B \\ 
\text{Left side: } A \cup (B \cap \overline{A}) = (A \cup \overline{A}) \cap (A \cup B) = U \cap (A \cup B) = A \cup B
}$$

**Identity 7:**
$$\displaylines{
(A - B) - C = (A - C) - (B - C) = A - (B \cup C) \\ 
1. \ \ (A - B) - C = (A - C) - (B - C) \\ 
\text{Left side: } (A - B) - C = (A \cap \overline{B}) \cap \overline{C} = A \cap \overline{B} \cap \overline{C} \\ 
\text{Right side: } (A \cap \overline{C}) \cap \overline{(B \cap \overline{C})} = (A \cap \overline{C}) \cap (\overline{B} \cup C) = A \cap \overline{C} \cap (C \cup \overline{B}) = A \cap ((\overline{C} \cap C) \cup (\overline{C} \cap \overline{B})) = A \cap (\overline{C} \cap \overline{B})= A \cap \overline{B} \cap \overline{C} \\ 
2. \ \ (A - B) - C = A - (B \cup C) \\ 
\text{Left side: } A \cap \overline{B} \cap \overline{C} \\ 
\text{Right side: } A - (B \cup C) = A \cap \overline{B \cup C} = A \cap \overline{B} \cap \overline{C}
}$$

**Identity 8:**
$$\displaylines{
A \cup B = A \Delta AB \\ 
\text{Right side: } A \Delta AB = (A \cap \overline{AB}) \cup (\overline{ A } \cap AB) = \\
= (A \cap (\overline{A} \cup \overline{B})) \cup (\overline{A} \cap A \cap B) = \\ 
= (A \cap \overline{A}) \cup (A \cap \overline{B}) \cup (\overline{A} \cap A \cap B) = \\ 
= (A \cap \overline{B})
}$$

**Identity 9:**
$$\displaylines{
A \cup B = (A \Delta B) \cup A \cap B \\
\text{Right side: } (A \cap \overline{B}) \cup (\overline{A} \cap B) \cup (A \cap B) = (A \cap \overline{B}) \cup B \cap (A \cup \overline{A}) = \\ 
= (A \cap \overline{B}) \cup B = (B \cup \overline{B}) \cap (B \cup A) = (A \cup B) \cap U = A \cup B
}$$

**Identity 10:**
$$\displaylines{
A - (B \cup C) = (A - B) \cap (A - C) \\ 
\text{Left side: } A \cap \overline{B \cup C} = A \cap \overline{B} \cap \overline{C} \\ 
\text{Right side: } (A \cap \overline{B}) \cap (A \cap \overline{C}) = A \cap A \cap \overline{B} \cap \overline{C} = A \cap \overline{B} \cap \overline{C}
}$$

**Identity 11:**
$$\displaylines{
(A \cup B) - C = (A - C) \cup (B - C) \\ 
\text{Left side: } (A \cup B) \cap \overline{C} = (A \cap \overline{C}) \cup (B \cap \overline{C}) = (A - C) \cup (B - C)
}$$

**Identity 12:**
$$\displaylines{
A - BC = (A - B) \cup (A - C) = ABC \Delta A \\
1. \ \ A - BC = ABC \Delta A \\ 
\text{Right side: } ABC \Delta A = (ABC \cap \overline{A}) \cup (\overline{ABC} \cap A) = A \cap \overline{ABC} = \\
= A \cap (\overline{A} \cup (\overline{B} \cup \overline{C})) = (A \cap \overline{A}) \cup (A \cap (\overline{B} \cup \overline{C})) = \\ 
= A \cap (\overline{B} \cup \overline{C}) = A - BC \\ 
2. \ \ (A - B) \cup (A -C) = ABC \Delta A \\ 
\text{Right side: } ABC \Delta A = A \cap (\overline{B} \cup \overline{C}) = \\
= (A \cap \overline{B}) \cup (A \cap \overline{C}) = \\
= (A - B) \cup (A - C)
}$$




