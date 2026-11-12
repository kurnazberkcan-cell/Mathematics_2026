# Exercise 14. A Small Change in the Right-Hand Side

## Solution

Consider the system with third equation $3x=c$:

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
2 & -1 & \mid & 1 \\
3 & 0 & \mid & c \\
\end{pmatrix}
$$

Apply $R_2\to R_2-2R_1$ and $R_3\to R_3-3R_1$:

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & -3 & \mid & -3 \\
0 & -3 & \mid & c-6 \\
\end{pmatrix}
$$

Apply $R_3\to R_3-R_2$:

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & -3 & \mid & -3 \\
0 & 0 & \mid & c-3 \\
\end{pmatrix}
$$

**First system, $c=3$.** The last row is $0=0$, so the system is consistent. Then $y=1$ and $x=1$, giving the unique solution $(1,1)$. Check: $1+1=2$, $2-1=1$, $3\cdot1=3$.

**Second system, $c=3.1$.** The last row is $0=0.1$, a contradiction, so the system has **no solution**. Check directly: the third equation gives $x=\tfrac{31}{30}$, the first then gives $y=\tfrac{29}{30}$, and the second equation would need $2x-y=\tfrac{33}{30}=1.1$, not $1$.

There are $3$ equations and only $2$ unknowns, so the three lines must pass through one common point for the system to be consistent. For $c=3$ they all pass through $(1,1)$. Changing $c$ moves the vertical line $x=\tfrac c3$ away from that point, so the three lines no longer meet at a single point and the system becomes inconsistent.
