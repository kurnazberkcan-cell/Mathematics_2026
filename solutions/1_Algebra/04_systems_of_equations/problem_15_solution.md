# Exercise 15. Classifying Three Systems

## Solution

**System 1.**

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
1 & -1 & \mid & 0 \\
\end{pmatrix}
$$

Apply $R_2\to R_2-R_1$:

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & -2 & \mid & -2 \\
\end{pmatrix}
$$

There are two pivots and two unknowns, so there is **exactly one solution**: $y=1$, $x=1$.

**System 2.**

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
2 & 2 & \mid & 4 \\
\end{pmatrix}
$$

Apply $R_2\to R_2-2R_1$:

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & 0 & \mid & 0 \\
\end{pmatrix}
$$

The zero row is consistent and there is one pivot for two unknowns, so there are **infinitely many solutions**: $(x,y)=(2-t,\;t)$.

**System 3.**

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
2 & 2 & \mid & 5 \\
\end{pmatrix}
$$

Apply $R_2\to R_2-2R_1$:

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & 0 & \mid & 1 \\
\end{pmatrix}
$$

The last row says $0=1$, so there is **no solution**.
