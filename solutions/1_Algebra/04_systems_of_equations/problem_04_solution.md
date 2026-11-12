# Exercise 4. Infinitely Many Solutions

## Solution

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 2 \\
2 & 2 & 2 & \mid & 4 \\
1 & -1 & 1 & \mid & 0 \\
\end{pmatrix}
$$

Apply $R_2\to R_2-2R_1$ and $R_3\to R_3-R_1$:

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 2 \\
0 & 0 & 0 & \mid & 0 \\
0 & -2 & 0 & \mid & -2 \\
\end{pmatrix}
$$

Swap $R_2$ and $R_3$:

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 2 \\
0 & -2 & 0 & \mid & -2 \\
0 & 0 & 0 & \mid & 0 \\
\end{pmatrix}
$$

From row 2, $y=1$. From row 1, $x+z=1$. The variable $z$ has no pivot, so it is free. Put $z=t$:

$$
(x,y,z)=(1-t,\;1,\;t),\qquad t\in\mathbb{R}
$$

Check for $t=2$, which gives $(-1,1,2)$:

$$
-1+1+2=2,
$$

$$
2(-1)+2\cdot1+2\cdot2=4,
$$

$$
-1-1+2=0
$$

All three equations hold.
