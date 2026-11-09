# Problem 12. Finding Inverses Without Starting from Scratch

## Question

It is known that

$$
A^{-1}=
\begin{pmatrix}
2 & -1 \\
-3 & 2 \\
\end{pmatrix}.
$$

Without finding $A$, compute $(3A)^{-1}$, $(A^T)^{-1}$, and $(A^2)^{-1}$. Justify each result using the appropriate property.

## Solution

Part 1: for a nonzero scalar $c$ we have $(cA)^{-1}=\frac{1}{c}A^{-1}$, because $(cA)\left(\frac{1}{c}A^{-1}\right)=AA^{-1}=I$. Hence

$$
(3A)^{-1}=\frac{1}{3}
\begin{pmatrix}
2 & -1 \\
-3 & 2 \\
\end{pmatrix}
$$

$$
(3A)^{-1}=
\begin{pmatrix}
\frac{2}{3} & -\frac{1}{3} \\
-1 & \frac{2}{3} \\
\end{pmatrix}.
$$

Part 2: transposition and inversion commute, $(A^T)^{-1}=(A^{-1})^T$, because $A^T(A^{-1})^T=(A^{-1}A)^T=I^T=I$. Hence

$$
(A^T)^{-1}=
\begin{pmatrix}
2 & -3 \\
-1 & 2 \\
\end{pmatrix}.
$$

Part 3: by the rule for the inverse of a product, $(A^2)^{-1}=(AA)^{-1}=A^{-1}A^{-1}=(A^{-1})^2$. Hence

$$
(A^2)^{-1}=
\begin{pmatrix}
2 & -1 \\
-3 & 2 \\
\end{pmatrix}
\begin{pmatrix}
2 & -1 \\
-3 & 2 \\
\end{pmatrix}
$$

$$
(A^2)^{-1}=
\begin{pmatrix}
4+3 & -2-2 \\
-6-6 & 3+4 \\
\end{pmatrix}
$$

$$
(A^2)^{-1}=
\begin{pmatrix}
7 & -4 \\
-12 & 7 \\
\end{pmatrix}.
$$
