## Problem 3

**Question:** Let

$$
A = \begin{pmatrix} 1 & 2 & 0 \\ 0 & 3 & 1 \\ 2 & 1 & 1 \end{pmatrix}.
$$

Compute $\det A$. Let $B$ be the matrix obtained from $A$ by swapping the first and second rows ($R_1 \leftrightarrow R_2$). Predict $\det B$ using a determinant property, then verify your prediction by computing $\det B$ directly.

### Solution

**Computing $\det A$ (Sarrus' rule).** Repeat the first two columns to the right of the matrix:

$$
\begin{array}{ccc|cc}
1 & 2 & 0 & 1 & 2 \\
0 & 3 & 1 & 0 & 3 \\
2 & 1 & 1 & 2 & 1
\end{array}
$$

Sum of the products along the down-right diagonals:

$$
1\cdot 3\cdot 1 + 2\cdot 1\cdot 2 + 0\cdot 0\cdot 1 = 3 + 4 + 0 = 7
$$

Sum of the products along the up-right diagonals:

$$
0\cdot 3\cdot 2 + 1\cdot 1\cdot 1 + 2\cdot 0\cdot 1 = 0 + 1 + 0 = 1
$$

Therefore:

$$
\det A = 7 - 1 = 6
$$

**Matrix $B$.** Swap the first and second rows of $A$ ($R_1 \leftrightarrow R_2$):

$$
B = \begin{pmatrix} 0 & 3 & 1 \\ 1 & 2 & 0 \\ 2 & 1 & 1 \end{pmatrix}
$$

**Prediction.** Swapping two rows of a matrix multiplies the determinant by $-1$, so

$$
\det B = -\det A = -6
$$

**Verification.** Expanding along the first row:

$$
\det B = 0\cdot\det\begin{pmatrix} 2 & 0 \\ 1 & 1 \end{pmatrix}
- 3\cdot\det\begin{pmatrix} 1 & 0 \\ 2 & 1 \end{pmatrix}
+ 1\cdot\det\begin{pmatrix} 1 & 2 \\ 2 & 1 \end{pmatrix}
$$

$$
= 0 - 3\cdot(1\cdot 1 - 0\cdot 2) + 1\cdot(1\cdot 1 - 2\cdot 2)
= -3\cdot 1 + (1 - 4) = -3 - 3 = -6
$$

### Conclusion

The direct calculation matches the prediction:

$$
\det A = 6, \qquad \det B = -6
$$
