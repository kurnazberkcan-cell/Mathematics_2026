## Exercise 14. A System of Equations and the Determinant

Given

$$
A=
\begin{pmatrix}
1 & 2 \\
k & 4 \\
\end{pmatrix}
$$

The determinant is

$$
\det A=1\cdot4-2k=4-2k
$$

The system has exactly one solution for every $b$ if and only if the matrix is invertible.

Therefore,

$$
4-2k\neq0
$$

$$
k\neq2
$$

Hence, the system has exactly one solution for every $b$ when

$$
\boxed{k\neq2}
$$

### Exceptional case: $k=2$

When $k=2$, the system becomes

$$
\begin{cases}
x+2y=b_1, \\
2x+4y=b_2.
\end{cases}
$$

**Example with infinitely many solutions:**

Choose

$$
b=
\begin{pmatrix}
1 \\
2 \\
\end{pmatrix}
$$

The system becomes

$$
\begin{cases}
x+2y=1, \\
2x+4y=2.
\end{cases}
$$

The second equation is twice the first. Therefore, both equations represent the same line, and there are infinitely many solutions.

**Example with no solution:**

Choose

$$
b=
\begin{pmatrix}
1 \\
0 \\
\end{pmatrix}
$$

The system becomes

$$
\begin{cases}
x+2y=1, \\
2x+4y=0.
\end{cases}
$$

The second equation contradicts the first because its left-hand side is twice the first equation, but its right-hand side is not twice the first right-hand side.

Therefore, the system has no solution.
