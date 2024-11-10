*Exercise 3*
$$\displaylines{
\text{Solve the equation.}
}
$$
$$\displaylines{
\text{Problem 20.} \\ 
(A \cup \overline{X}) \otimes B = A-B \\ 
(A\cup\overline X)\otimes B \otimes A\overline B = \emptyset \\
1) \ (A\cup\overline X) \otimes B = ((A\cup\overline X) - B)\cup(B - (A\cup\overline X)) =  A\overline B \cup \overline X \ \overline{B} \cup B\overline AX\\
2) \ (A\overline B \cup \overline X \ \overline{B} \cup B\overline AX)\otimes A\overline{B} = \emptyset \\ 
((A\overline{B} \cup \overline{X} \ \overline{B} \cup B\overline{A}X) \cap (\overline{A} \cup B)) \cup (A\overline{B} \cap \overline{(A\overline{B} \cup \overline{X} \ \overline{B} \cup B\overline{A}X)}) = \emptyset \\
\text{ 1 скобка: } \ A\overline{B} \cap (\overline{A} \cup B) = \emptyset ; \ \overline{X} \ \overline{B} \cap (\overline{A} \cup B) = \overline{X} \ \overline{B} \ \overline{A}; \ \\ B\overline{A}X \cap (\overline{A} \cup B) = B\overline{A}X \\
\text{ 2 скобка: } \ \overline{(A\overline{B} \cup \overline{X} \ \overline{B} \cup B\overline{A}X)} = (\overline{A} \cup B) \cap (X \cup B) \cap ( \overline{B} \cup A \cup \overline{X}) =  \\ = (\overline{A}X \cup \overline{A}B \cup BX \cup B)(\overline{B} \cup A \cup \overline{X}) = \overline{A}X\overline{B} \cup \overline{A}B\overline{X} \cup BXA \cup BA \cup B \overline{X}  \\
\implies (B\overline{A}X) \cup ((\overline{A}\ \overline{X} B \cup \overline{A} X B \cup BXA \cup BA \cup B\overline{X} ) \cap A\overline{B})  = B\overline{A}X \cup \overline{X} \ \overline{B} \ \overline{A}\\

\\

\begin{cases}
B\overline{A}X  = \emptyset\\
\overline{X} \ \overline{B} \ \overline{A} = \emptyset
\end{cases} \iff \boxed{\overline{A} \ \overline{B} \subseteq X \subseteq A \cup \overline{B}}
} 
$$



*Exercise 4*
$$\displaylines{
\text{Find out if the systems are equivalent.}
}
$$
$$\displaylines{
\text{Problem 20.} \\ \begin{cases} XZ = YW;\\XY\cup ZW = \overline{YW};\\ Z \subseteq W; \end{cases} \iff \begin{cases} X = Y; \\ Z = W \end{cases} \\ 
}
$$
$$\displaylines{
\text{Consider the first system:} \\
1) \ XZ = YW \iff XZ\otimes YW = \emptyset \\
2) \ XY \cup ZW = \overline{YW} \iff (XY \cup ZW) \otimes \overline{YW} = \emptyset\\
3) \ Z\subseteq W \iff Z\overline W = \emptyset \\ \\

}$$
$$\displaylines{
\text{Let's solve it sequentially:} \\ \\
1. \ XZ\otimes YW = \emptyset \\
	(XZ\overline{YW})\cup(YW\overline{XZ}) = \emptyset \\
	(XZ\cap(\overline Y \cup \overline W)) \cup (YW\cap(\overline X \cup \overline Z)) = \emptyset \\
	XZ\overline Y \cup YW\overline X \cup YW\overline Z = \emptyset \\ \\
}$$
$$\displaylines{
2. \ (XY \cup ZW) \otimes \overline{YW} = \emptyset \\
	((XY \cup ZW) - \overline{YW}) \cup (\overline{YW} \cap \overline{XY} \cap \overline{ZW}) = \emptyset \\
	((XY \cup ZW) \cap YW) \cup ((\overline{Y}\cup \overline{W})\cap(\overline{X}\cup \overline{Y})\cap(\overline{Z}\cup \overline{W})) = \emptyset \\
	XYW \cup YZW \cup ((\overline{X} \ \overline{Y} \cup \overline{Y} \cup \overline{W} \ \overline{X} \cup \overline{W} \ \overline{Y}) \cap(\overline{Z} \cup \overline{W})) = \emptyset \\
	XYW \cup YZW \cup \overline{X} \ \overline{Y} \ \overline{Z} \cup \overline{X} \ \overline{Y} \ \overline{W} \cup \overline{Y} \ \overline{Z} \cup \overline{Y} \ \overline{W} \cup \overline{W} \ \overline{X} \cup \overline{W} \ \overline{Y} = \emptyset
}$$
$$\displaylines{
\text{Let's combine everything into one system:} \\
\begin{cases} 
XZ\overline Y = \emptyset \\
YW\overline X = \emptyset \\
YW\overline Z = \emptyset \\
XYW = \emptyset \\
YZW = \emptyset \\
\overline{X} \ \overline{Y} \ \overline{Z} = \emptyset \\
 \overline{X} \ \overline{Y} \ \overline{W} = \emptyset \\
 \overline{Y} \ \overline{Z} = \emptyset \\
 \overline{Y} \ \overline{W} = \emptyset \\
 \overline{W} \ \overline{X} = \emptyset \\
 \overline{W} \ \overline{Y} = \emptyset  \\
Z\overline{W} = \emptyset
\end{cases} \\\\
}$$
$$\displaylines{
\text{Consider the second system:} \\
1) \ X = Y \iff X\otimes Y = \emptyset \\
2) \ Z = W  \iff Z \otimes W = \emptyset\\\\
\text{Let's solve it sequentially: }\\
1. \ X\otimes Y = \emptyset \\
	X\overline Y \cup Y \overline X = \emptyset \\
2. \ Z \otimes W = \emptyset \\ 
   Z\overline{W} \cup W\overline{Z} = \emptyset
}$$
$$\displaylines{
\text{Let's combine everything into one system:} \\ 
\begin{cases} 
X\overline Y = \emptyset \\
Y\overline X = \emptyset \\
Z\overline{W} = \emptyset \\
W \overline{Z} = \emptyset
\end{cases}
 }
$$
$$\displaylines{
\text{Let's make tables for the two received systems:} \\
1) \ \ \ \begin{array}{c|c}
 & Y & Y & \overline{Y} & \overline{Y} & \\
\hline
W & \emptyset & \emptyset & \emptyset & \ & Z \\
\hline
W & \emptyset & \emptyset & \emptyset & \emptyset& \overline{Z} \\
\hline
\overline{W} & \emptyset & \emptyset & \emptyset & \emptyset & Z \\
\hline
\overline{W} &  & \emptyset& \emptyset& \emptyset& \overline{Z} \\
\hline
 & X & \overline{X} & X & \overline{X} & \\
\end{array} \ \ \ \ \ \
2) \ \ \ \begin{array}{c|c}
 & Y & Y & \overline{Y} & \overline{Y} & \\
 \hline
 W &  & \emptyset & \emptyset & & Z \\
 \hline
 W &\emptyset &\emptyset &\emptyset & \emptyset & \overline Z\\
 \hline
 \overline W & \emptyset &\emptyset &\emptyset &\emptyset & Z\\
 \hline 
 \overline W & &\emptyset &\emptyset & & \overline Z\\
 \hline & X & \overline X & X & \overline X& \\
\end{array}\\\\
\text{We see that they are not the same,} \implies \text{the systems are not equivalent. } \\ \text{ The second system follows from the first.}
}$$

$$\displaylines{
A\overline{B} \cup \overline{B} \cap \overline{X}\cup B\overline{A}X =  \overline{A} B(U \cup X) \cup \overline{B} \cap \overline{X} = \overline{A} \cup \overline{B} \cap \overline{X}\\
A \cap(A\cup B) = A \\
A \cup ( A \cap B) = A
}$$