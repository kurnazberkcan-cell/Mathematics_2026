# Exercise 11. A Parameter in a System of Three Equations

## Solution

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 1 \\
1 & t & 1 & \mid & 2 \\
1 & 1 & t & \mid & 3 \\
\end{pmatrix}
$$

Apply $R_2\to R_2-R_1$ and $R_3\to R_3-R_1$:

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 1 \\
0 & t-1 & 0 & \mid & 1 \\
0 & 0 & t-1 & \mid & 2 \\
\end{pmatrix}
$$

The next steps divide by $t-1$, which is valid only for $t\neq1$.

**Case $t\neq1$.** Then

$$
y=\frac{1}{t-1},\qquad z=\frac{2}{t-1},
$$

$$
x=1-y-z=1-\frac{3}{t-1}=\frac{t-4}{t-1}
$$

There is exactly one solution. Check for $t=2$, which gives $(x,y,z)=(-2,1,2)$:

$$
-2+1+2=1,
$$

$$
-2+2+2=2,
$$

$$
-2+1+4=3
$$

**Case $t=1$.** The matrix becomes

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 1 \\
0 & 0 & 0 & \mid & 1 \\
0 & 0 & 0 & \mid & 2 \\
\end{pmatrix}
$$

Row 2 says $0=1$, which is a contradiction, so there is **no solution**.

**Conclusion.** For $t\neq1$ there is exactly one solution, and for $t=1$ there is none. Infinitely many solutions never occur.
