# Exercise 3. Inconsistent System

## Solution

$$
\begin{pmatrix}
1 & 2 & \mid & 3 \\
2 & 4 & \mid & 7 \\
\end{pmatrix}
$$

Apply $R_2\to R_2-2R_1$:

$$
\begin{pmatrix}
1 & 2 & \mid & 3 \\
0 & 0 & \mid & 1 \\
\end{pmatrix}
$$

The second row says $0\cdot x+0\cdot y=1$, i.e. $0=1$, which is impossible. The system has no solution.

Interpretation: the left-hand side of the second equation is twice the left-hand side of the first, but the right-hand side $7$ is not $2\cdot3=6$. The two equations contradict each other. Geometrically, the lines $x+2y=3$ and $x+2y=\tfrac72$ are parallel and distinct.
