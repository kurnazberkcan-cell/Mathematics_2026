# Problem 15. Two Methods for Solving the Same System

## Question

For

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
7 \\
8 \\
\end{pmatrix}
$$

solve $Ax=b$ in two ways:

1. using $A^{-1}b$,
2. using Gaussian elimination.

Compare both solutions, the number of essential steps, and state which method was simpler in this example.

## Solution

Method 1: inverse. We have $\det A=6-1=5$, so

$$
A^{-1}=\frac{1}{5}
\begin{pmatrix}
3 & -1 \\
-1 & 2 \\
\end{pmatrix}.
$$

Then

$$
x=A^{-1}b=\frac{1}{5}
\begin{pmatrix}
21-8 \\
-7+16 \\
\end{pmatrix}
$$

$$
x=
\begin{pmatrix}
\frac{13}{5} \\
\frac{9}{5} \\
\end{pmatrix}.
$$

Method 2: Gaussian elimination. The augmented matrix is

$$
\begin{pmatrix}
2 & 1 & \mid & 7 \\
1 & 3 & \mid & 8 \\
\end{pmatrix}.
$$

Interchange $R_1$ and $R_2$:

$$
\begin{pmatrix}
1 & 3 & \mid & 8 \\
2 & 1 & \mid & 7 \\
\end{pmatrix}
$$

Operation $R_2\leftarrow R_2-2R_1$:

$$
\begin{pmatrix}
1 & 3 & \mid & 8 \\
0 & -5 & \mid & -9 \\
\end{pmatrix}
$$

From the second row, $-5x_2=-9$, so $x_2=\frac{9}{5}$. Back substitution into the first row gives

$$
x_1=8-3\cdot\frac{9}{5}=\frac{13}{5}.
$$

Verification:

$$
Ax=
\begin{pmatrix}
\frac{26}{5}+\frac{9}{5} \\
\frac{13}{5}+\frac{27}{5} \\
\end{pmatrix}
$$

$$
Ax=
\begin{pmatrix}
7 \\
8 \\
\end{pmatrix}=b.
$$

Comparison: both methods give $x=\left(\frac{13}{5},\frac{9}{5}\right)^T$. The inverse method needs the determinant, the inverse matrix, and a matrix-vector product. Gaussian elimination needs one row interchange, one row operation, and back substitution, so it is shorter here. The inverse is useful when the same matrix $A$ must be used with many different right-hand sides $b$, but for a single system elimination is simpler.
