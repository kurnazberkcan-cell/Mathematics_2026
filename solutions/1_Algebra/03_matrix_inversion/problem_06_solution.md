# Problem 6. Solving a System Using the Inverse

## Question

Solve $Ax=b$, where

$$
A=
\begin{pmatrix}
2 & 1 \\
1 & 3 \\
\end{pmatrix},
$$

$$
b=
\begin{pmatrix}
5 \\
7 \\
\end{pmatrix},
$$

using $x=A^{-1}b$. Then substitute the resulting vector back into the equation and check the result.

## Solution

The determinant is $\det A=2\cdot3-1\cdot1=5\neq0$, so

$$
A^{-1}=\frac{1}{5}
\begin{pmatrix}
3 & -1 \\
-1 & 2 \\
\end{pmatrix}.
$$

Multiplying $Ax=b$ on the left by $A^{-1}$ gives $x=A^{-1}b$:

$$
x=\frac{1}{5}
\begin{pmatrix}
15-7 \\
-5+14 \\
\end{pmatrix}
$$

$$
x=
\begin{pmatrix}
\frac{8}{5} \\
\frac{9}{5} \\
\end{pmatrix}.
$$

Verification:

$$
Ax=
\begin{pmatrix}
\frac{16}{5}+\frac{9}{5} \\
\frac{8}{5}+\frac{27}{5} \\
\end{pmatrix}
$$

$$
Ax=
\begin{pmatrix}
5 \\
7 \\
\end{pmatrix}=b.
$$
