# Problem 11. Parameter and Invertibility

## Question

For

$$
A(t)=
\begin{pmatrix}
1 & t \\
t & 1 \\
\end{pmatrix}
$$

find all $t$ for which the matrix is invertible, and then give a formula for $A(t)^{-1}$. Explain what happens to this formula at the excluded values.

## Solution

The determinant is

$$
\det A(t)=1-t^2.
$$

The matrix is invertible exactly when $1-t^2\neq0$, that is, for $t\neq1$ and $t\neq-1$.

For such $t$ the $2\times2$ formula gives

$$
A(t)^{-1}=\frac{1}{1-t^2}
\begin{pmatrix}
1 & -t \\
-t & 1 \\
\end{pmatrix}.
$$

Verification:

$$
A(t)A(t)^{-1}=\frac{1}{1-t^2}
\begin{pmatrix}
1-t^2 & -t+t \\
t-t & -t^2+1 \\
\end{pmatrix}
$$

$$
A(t)A(t)^{-1}=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}.
$$

At the excluded values the denominator $1-t^2$ equals $0$, so the formula is undefined. This is not just a defect of the formula: for $t=1$ the two rows are equal, and for $t=-1$ the two rows are opposite. In both cases the rows are linearly dependent, $\det A(t)=0$, and the inverse does not exist.
