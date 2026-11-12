# Exercise 9. A System from a Sum Condition

## Solution

$$
\begin{pmatrix}
1 & 1 & \mid & 10 \\
2 & 5 & \mid & 32 \\
\end{pmatrix}
$$

Apply $R_2\to R_2-2R_1$:

$$
\begin{pmatrix}
1 & 1 & \mid & 10 \\
0 & 3 & \mid & 12 \\
\end{pmatrix}
$$

So $y=4$ and $x=10-4=6$.

$$
(x,y)=(6,4)
$$

Check:

$$
6+4=10,
$$

$$
2\cdot6+5\cdot4=32
$$

Geometric reason for uniqueness: the line $x+y=10$ has slope $-1$, and the line $2x+5y=32$ has slope $-\tfrac25$. The slopes differ, so the lines are not parallel and meet in exactly one point, $(6,4)$.
