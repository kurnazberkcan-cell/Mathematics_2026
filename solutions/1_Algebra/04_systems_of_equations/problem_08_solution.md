# Exercise 8. Two Systems with the Same Coefficient Matrix

## Solution

First system:

$$
\begin{pmatrix}
2 & 1 & \mid & 5 \\
1 & -1 & \mid & 1 \\
\end{pmatrix}
$$

Swap $R_1$ and $R_2$:

$$
\begin{pmatrix}
1 & -1 & \mid & 1 \\
2 & 1 & \mid & 5 \\
\end{pmatrix}
$$

Apply $R_2\to R_2-2R_1$:

$$
\begin{pmatrix}
1 & -1 & \mid & 1 \\
0 & 3 & \mid & 3 \\
\end{pmatrix}
$$

So $y=1$ and $x=1+y=2$. Solution: $(x,y)=(2,1)$.

Second system, with the same steps:

$$
\begin{pmatrix}
1 & -1 & \mid & 4 \\
2 & 1 & \mid & 1 \\
\end{pmatrix}
$$

Apply $R_2\to R_2-2R_1$:

$$
\begin{pmatrix}
1 & -1 & \mid & 4 \\
0 & 3 & \mid & -7 \\
\end{pmatrix}
$$

So $y=-\tfrac73$ and $x=4+y=\tfrac53$. Solution: $(x,y)=\left(\tfrac53,\;-\tfrac73\right)$.

Check:

$$
2\cdot\tfrac53-\tfrac73=1,
$$

$$
\tfrac53+\tfrac73=4
$$

**What is the same.** The row operations (swap, then $R_2\to R_2-2R_1$) and the resulting coefficient part

$$
\begin{pmatrix}
1 & -1 \\
0 & 3 \\
\end{pmatrix}
$$

are identical in both cases. The multipliers are chosen using only the coefficients, so they depend on the matrix and not on the right-hand side. Only the last column differs.
