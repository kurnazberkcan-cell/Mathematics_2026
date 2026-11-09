# Problem 1. Definition of the Inverse

## Question

Given

$$
A=
\begin{pmatrix}
2 & 1 \\
1 & 1 \\
\end{pmatrix},
$$

$$
B=
\begin{pmatrix}
1 & -1 \\
-1 & 2 \\
\end{pmatrix}.
$$

Check, without using a formula, whether $B=A^{-1}$. Compute $AB$ and $BA$ and relate the result to the definition of the inverse.

## Solution

By definition, $B=A^{-1}$ exactly when $AB=I$ and $BA=I$.

$$
AB=
\begin{pmatrix}
2-1 & -2+2 \\
1-1 & -1+2 \\
\end{pmatrix}
$$

$$
AB=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
$$

$$
BA=
\begin{pmatrix}
2-1 & 1-1 \\
-2+2 & -1+2 \\
\end{pmatrix}
$$

$$
BA=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
$$

Both products equal $I$, so the definition is satisfied and $B=A^{-1}$.
