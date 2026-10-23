## Problem 1

**Question:** Use the formula $\det\begin{pmatrix} a & b \\ c & d \end{pmatrix} = ad - bc$ to compute the determinant of each matrix below. State whether each matrix is invertible.

$$
M_1 = \begin{pmatrix} 3 & -2 \\ 5 & 4 \end{pmatrix}, \qquad
M_2 = \begin{pmatrix} 1 & 7 \\ 2 & 14 \end{pmatrix}
$$

### Solution

**Matrix $M_1$:**

$$
\det(M_1) = 3 \cdot 4 - (-2)\cdot 5 = 12 + 10 = 22
$$

**Matrix $M_2$:**

$$
\det(M_2) = 1 \cdot 14 - 7 \cdot 2 = 14 - 14 = 0
$$

The second determinant is $0$ because the second row is $2$ times the first row, so the rows are linearly dependent.

### Conclusion

- $\det(M_1) = 22 \neq 0$, so $M_1$ is **invertible**.
- $\det(M_2) = 0$, so $M_2$ is **not invertible**.
