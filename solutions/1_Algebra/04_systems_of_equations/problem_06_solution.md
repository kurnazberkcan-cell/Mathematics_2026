# Exercise 6. A System with a Parameter

## Solution

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
a & a & \mid & 4 \\
\end{pmatrix}
$$

Apply $R_2\to R_2-aR_1$:

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & 0 & \mid & 4-2a \\
\end{pmatrix}
$$

- If $a\neq2$, the second row is $0=4-2a\neq0$, so there is **no solution**.
- If $a=2$, the second row is $0=0$. Then $x+y=2$, and with $y=t$ we get $(x,y)=(2-t,\;t)$, so there are **infinitely many solutions**.

**Exactly one solution never occurs.** The second row of the coefficient matrix is always $a$ times the first row, so elimination always produces a zero row in the coefficient part. There is at most one pivot but two unknowns, so there is always at least one free variable whenever the system is consistent.
