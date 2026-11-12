# Exercise 13. Does Every Equation Add New Information?

## Solution

Augmented matrix in the unknowns $(x_1,x_2,x_3)$:

$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 10 \\
0 & 1 & 1 & \mid & 8 \\
1 & 0 & -1 & \mid & 2 \\
\end{pmatrix}
$$

Apply $R_3\to R_3-R_1$:

$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 10 \\
0 & 1 & 1 & \mid & 8 \\
0 & -1 & -1 & \mid & -8 \\
\end{pmatrix}
$$

Apply $R_3\to R_3+R_2$:

$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 10 \\
0 & 1 & 1 & \mid & 8 \\
0 & 0 & 0 & \mid & 0 \\
\end{pmatrix}
$$

The variable $x_3$ is free. Put $x_3=t$: then $x_2=8-t$ and $x_1=10-x_2=2+t$.

$$
(x_1,x_2,x_3)=(2+t,\;8-t,\;t),\qquad t\in\mathbb{R}
$$

The zero row shows that the third equation is redundant. Directly:

$$
(x_1+x_2)-(x_2+x_3)=x_1-x_3,
$$

and the right-hand sides satisfy $10-8=2$. So equation 3 equals equation 1 minus equation 2, and it adds no new information. The solution set is already determined by the first two equations.
