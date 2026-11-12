# Exercise 2. Gaussian Elimination, One Solution

## Solution

Augmented matrix:

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 6 \\
2 & -1 & 1 & \mid & 3 \\
1 & 2 & -1 & \mid & 2 \\
\end{pmatrix}
$$

Apply $R_2\to R_2-2R_1$ and $R_3\to R_3-R_1$:

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 6 \\
0 & -3 & -1 & \mid & -9 \\
0 & 1 & -2 & \mid & -4 \\
\end{pmatrix}
$$

Swap $R_2$ and $R_3$:

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 6 \\
0 & 1 & -2 & \mid & -4 \\
0 & -3 & -1 & \mid & -9 \\
\end{pmatrix}
$$

Apply $R_3\to R_3+3R_2$:

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 6 \\
0 & 1 & -2 & \mid & -4 \\
0 & 0 & -7 & \mid & -21 \\
\end{pmatrix}
$$

Back substitution: $z=3$, then $y-2\cdot3=-4$ gives $y=2$, then $x=6-2-3=1$.

$$
(x,y,z)=(1,2,3)
$$

Check:

$$
1+2+3=6,
$$

$$
2-2+3=3,
$$

$$
1+4-3=2
$$

All three equations hold.
