# Exercise 12. Homogeneous System

## Solution

$$
\begin{pmatrix}
1 & 2 & -1 & \mid & 0 \\
2 & 4 & -2 & \mid & 0 \\
1 & -1 & 2 & \mid & 0 \\
\end{pmatrix}
$$

Apply $R_2\to R_2-2R_1$ and $R_3\to R_3-R_1$:

$$
\begin{pmatrix}
1 & 2 & -1 & \mid & 0 \\
0 & 0 & 0 & \mid & 0 \\
0 & -3 & 3 & \mid & 0 \\
\end{pmatrix}
$$

Swap $R_2$ and $R_3$, then apply $R_2\to-\tfrac13R_2$:

$$
\begin{pmatrix}
1 & 2 & -1 & \mid & 0 \\
0 & 1 & -1 & \mid & 0 \\
0 & 0 & 0 & \mid & 0 \\
\end{pmatrix}
$$

Row 2 gives $y=z$. Row 1 gives $x=-2y+z=-z$. The variable $z$ is free. Put $z=t$:

$$
(x,y,z)=(-t,\;t,\;t),\qquad t\in\mathbb{R}
$$

Check for the third equation: $-t-t+2t=0$.

The point $(0,0,0)$ always satisfies a homogeneous system because every equation has the form $a_1x_1+\dots+a_nx_n=0$, and substituting zeros makes the left-hand side $0$. It is the solution for $t=0$ here.
