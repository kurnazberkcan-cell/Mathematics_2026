# Problem 2. Formula for a 2x2 Matrix

## Question

Find the inverse of

$$
A=
\begin{pmatrix}
3 & 2 \\
5 & 4 \\
\end{pmatrix}
$$

using the formula for a $2\times2$ matrix. At the end, check the result by computing one product with $A$.

## Solution

For $A=\begin{pmatrix}a&b\\c&d\end{pmatrix}$ with $\det A=ad-bc\neq0$ the inverse is obtained by swapping $a$ and $d$, changing the signs of $b$ and $c$, and dividing by the determinant.

The determinant is

$$
\det A = 3\cdot4-2\cdot5 = 2.
$$

Since $\det A\neq0$, the inverse exists:

$$
A^{-1}=\frac{1}{2}
\begin{pmatrix}
4 & -2 \\
-5 & 3 \\
\end{pmatrix}
$$

$$
A^{-1}=
\begin{pmatrix}
2 & -1 \\
-\frac{5}{2} & \frac{3}{2} \\
\end{pmatrix}.
$$

Verification:

$$
AA^{-1}=
\begin{pmatrix}
6-5 & -3+3 \\
10-10 & -5+6 \\
\end{pmatrix}
$$

$$
AA^{-1}=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}.
$$
