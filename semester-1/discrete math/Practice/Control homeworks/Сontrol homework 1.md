
*Exercise 1*

$$\displaylines{ \text{A universal set is given} \ U = \{1, 2, 3, 4, 5, 6, 7, 8\}, \text{and it contains subsets} \\ A=\{x|x \leq{4}\}, \ B = \{2, 4, 5, 6\}, \ C = \{1, 3, 5, 6\} \ and \ D = \{1, 2, 6, 7\}
}
$$
$$\displaylines{
\text{Problems 20.} \\ \\ 1) \ (\overline{B}D \ \cup \ A)  \ \otimes \ BC \ = \ ?
\\ \text{a)} \ \overline{B} = \set{1, 3, 7, 8} \\ \text{b)} \ \ \overline{B}\cap{D} =  \set{1, 3, 7, 8} \cap{\set{1, 2, 6, 7}} = \set{1, 7} \\
\text{c)} \ \overline{B}D \ \cup \ A = \set{1, 7} \cup{\set{1, 2, 3, 4}} = \set{1, 2, 3, 4, 7} \\ \text{d)} \ BC = \set{2, 4, 5, 6}\cap{\set{1, 3, 5, 6}} = \set{5, 6} \\ \text{e) } (\overline{B}D \ \cup \ A)  \ \otimes \ BC \ = (\set{1, 2, 3, 4, 7}\setminus{\set{5, 6}})\cup(\set{5, 6}\setminus{\set{1, 2, 3, 4, 7}}) = \\ =\set{1, 2, 3, 4, 7}\cup\set{5, 6} = \set{1, 2, 3, 4, 5, 6, 7}\\\text{The answer is: }\ \set{1,2,3,4,5,6,7}\\\\\text{2)} \ (D -(A\cup{C}))\times{BC} = \ ? \\ \text{a)} \ A\cup{C} = \set{1, 2, 3, 4} \cup{\set{1,3,5,6}} = \set{1,2,3,4,5,6} \\\text{b)} \ D -(A\cup{C}) = \set{1,2,6,7} \ - \ \set{1,2,3,4,5,6} = \set{7} \\ \text{c)} \ B\cap{C} = \set{2,4,5,6}\cap{\set{1,3,5,6}} = \set{5,6} \\ \text{e)} \ (D -(A\cup{C}))\times{BC} = \set{7}\times{\set{5,6}} = \set{(7,5),(7,6)} \\\text{The answer is: }\set{(7,5),(7,6)} \\\\\text{3)} \ 2^{A\overline{D}}\cup{2^{A\overline{B}C}} = \ ? \\\text{a)} \ A\cap{\overline{D}} = \set{1,2,3,4}\cap{\set{3,4,5,8}} = \set{3,4} \\\text{b)} \ A\overline{B}C = \set{1,2,3,4}\cap{\set{1,3,7,8}}\cap{\set{1,3,5,6}} = \set{1,3} \\\text{c)} \ 2^{\set{3,4}} = \set{\emptyset, \{3\}, \{4\}, \{3,4\}}\\\text{d)} \ 2^{\set{1,3}} = \set{\emptyset, \{1\}, \{3\}, \{1,3\}} \\\text{e)} 2^{\set{3,4}} \cup 2^{\set{1,3}} = \set{\emptyset,\{1\}, \{3\}, \{4\}, \{1, 3\}, \{3, 4\}} \\\text{The answer is:} \set{\emptyset,\{1\}, \{3\}, \{4\}, \{1, 3\}, \{3, 4\}}

}
$$


*Exercise 2*
$$\displaylines{
\text{Need to convert a formula to an equivalent one that contains only union}\\\text{intersection, and complement operations and does not contain
parentheses.}
}
$$
$$\displaylines{
\text{Problem 20.} \\ (A-(B-C))\otimes{\overline{B}}\\ A-(B-C) = A \overline{(B\overline{C})} = A (\overline B \ \cup C) = (A \overline B)\cup(A C) \\ ((A \overline{B}) \cup (A  C)) \otimes \overline{B} = (((A  \overline{B}) \cup (A  C))  B) \cup (\overline{B}  \overline{((A  \overline{B}) \cup (A  C))}) \\ \overline{((A  \overline{B}) \cup (A  C))} = \overline{(A  \overline{B})}  \overline{(A  C)} \\ \overline{(A  \overline{B})} = \overline{A} \cup B \\\overline{(A  C)} = \overline{A} \cup \overline{C} \\ \overline{((A \ \overline{B}) \cup (A  C))} = (\overline{A} \cup B)  (\overline{A} \cup \overline{C}) \\ ((A  \overline{B}) \cup (A  C)) \otimes \overline{B} = (A  C B) \cup (\overline{BA}) \\ \text{The answer is: }A C  B \cup \overline{BA}

}
$$

*Exercise 3*
$$\displaylines{
\text{Solve the equation.}
}
$$
$$\displaylines{
\text{Problem 20.} \\ 
(A \cup \overline{X}) \otimes B = A-B \\ 
(A\cup\overline X)\otimes B \otimes A\overline B = \emptyset \\
1) \ (A\cup\overline X) \otimes B = ((A\cup\overline X) - B)\cup(B - (A\cup\overline X)) = A\overline B \cup \overline{XB} \cup B\overline AX \\
2) \ (A\overline B \cup \overline X \ \overline B \cup B\overline AX) \otimes A\overline B = (A\overline{B} \otimes A\overline{B}) \cup (\overline{XB} \otimes A\overline{B}) \cup (\overline{A}BX \otimes A\overline{B}) = \\
= \emptyset \cup (\overline{XB} - A\overline{B}) \cup (\overline{A}BX - A\overline{B}) = \overline{XB} \cup \overline{A}BX
\\
\overline{XB} \cup \overline{A}BX= \emptyset\\
\begin{cases}
\overline X\overline B = \emptyset\\
\overline{A}BX= \emptyset\\
\end{cases} \iff 

\begin{cases}
X \supseteq \overline{B} \\
X \subseteq A \cup \overline{B}\\
\end{cases} \iff \boxed {\overline{B} \subseteq X \subseteq A \overline B} 
} 
$$



*Exercise 4*
$$\displaylines{
\text{Do I need to find out if the system of conditions is equivalent?}
}
$$
$$\displaylines{
\text{Problem 20.} \\ \begin{cases} XZ = YW;\\XY\cup ZW = \overline{YW};\\ Z \subseteq W; \end{cases} \iff \begin{cases} X = Y; \\ X = Z = \overline{W} \end{cases} \\ 
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
	((XY \cup ZW) \cap YW) \cup ([ \overline{Y}\cup(\overline{W}\cap \overline{X})] \cap (\overline{Z}\cup \overline{W})) = \emptyset\\
	((XY \cup ZW) \cap YW) \cup ([ \overline{Y} \cap (\overline{Z} \cup \overline{W})] \cup [(\overline{W}\cap \overline{X}) \cap (\overline{Z}\cup \overline{W})] = \emptyset\\
	XYW \cup YZW \cup [\overline{YZ} \cup \overline{YW}] \cup [\overline{WXZ} \cup \overline{WX}] = \emptyset
}$$
$$\displaylines{
\text{Let's combine everything into one system:} \\
\begin{cases} 
XZ\overline Y = \emptyset \\
YW\overline X = \emptyset \\
YW\overline Z = \emptyset \\
XYW = \emptyset \\
YZW = \emptyset \\
\overline{YZ} = \emptyset \\
\overline{YW} = \emptyset \\
\overline{WXZ} = \emptyset  \\
\overline{WX} = \emptyset \\
Z\overline{W} = \emptyset
\end{cases} \\\\
}$$
$$\displaylines{
\text{Consider the second system:} \\
1) \ X = Y \iff X\otimes Y = \emptyset \\
2) \ X = Z = \overline W \iff (X\otimes Z) \cup (Z\otimes \overline W) = \emptyset \\\\
\text{Let's solve it sequentially: }\\
1. \ X\otimes Y = \emptyset \\
	X\overline Y \cup Y \overline X = \emptyset \\
2. \ (X\otimes Z) \cup (Z\otimes \overline W) = \emptyset \\
	X\overline Z \cup Z\overline X\cup ZW\cup \overline {WZ} = \emptyset \\ 

}$$
$$\displaylines{
\text{Let's combine everything into one system:} \\ 
\begin{cases} 
X\overline Y = \emptyset \\
Y\overline X = \emptyset \\
X\overline Z = \emptyset \\
Z\overline X = \emptyset \\
ZW = \emptyset \\
\overline {WZ} = \emptyset \\
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
\overline{W} & \emptyset & \emptyset& \emptyset& \emptyset& \overline{Z} \\
\hline
 & X & \overline{X} & X & \overline{X} & \\
\end{array} \ \ \ \ \ \
2) \ \ \ \begin{array}{c|c}
 & Y & Y & \overline{Y} & \overline{Y} & \\
 \hline
 W & \emptyset & \emptyset & \emptyset &\emptyset & Z \\
 \hline
 W &\emptyset &\emptyset &\emptyset & & \overline Z\\
 \hline
 \overline W & &\emptyset &\emptyset &\emptyset & Z\\
 \hline 
 \overline W &\emptyset &\emptyset &\emptyset &\emptyset & \overline Z\\
 \hline
 & X & \overline X & X & \overline X& \\
\end{array}\\\\
\text{We see that they are not the same,} \implies \text{the systems are not equivalent. } \\ \text{ The second system contains all the conditions of the first system and additional conditions,} \\ \text{which under normal conditions would imply that the second system is more stringent and follows from the first.
} \\ \text{However, both systems are incompatible, which means there are no common solutions.}
}$$
