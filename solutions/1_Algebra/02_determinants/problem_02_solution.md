**Solution (Sarrus' rule):** Repeat the first two columns to the right of the matrix:

$$
\begin{array}{ccc|cc}
1 & 2 & -1 & 1 & 2 \\
0 & 3 & 4 & 0 & 3 \\
2 & 1 & 5 & 2 & 1
\end{array}
$$

Sum of the products along the down-right diagonals:

$$
1\cdot 3\cdot 5 + 2\cdot 4\cdot 2 + (-1)\cdot 0\cdot 1 = 15 + 16 + 0 = 31
$$

Sum of the products along the up-right diagonals:

$$
(-1)\cdot 3\cdot 2 + 1\cdot 4\cdot 1 + 2\cdot 0\cdot 5 = -6 + 4 + 0 = -2
$$

Therefore:

$$
\det A = 31 - (-2) = 33
$$

**Check (property used: adding a multiple of one row to another does not change the determinant):**

Apply $R_3 \to R_3 - 2R_1$:

$$
\det A =
\det\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 4 \\
0 & -3 & 7
\end{pmatrix}
$$

Expanding along the first column:

$$
= 1\cdot\det\begin{pmatrix} 3 & 4 \\ -3 & 7 \end{pmatrix}
= 1\cdot\bigl(3\cdot 7 - 4\cdot(-3)\bigr)
= 21 + 12
= 33
$$

Both methods agree:

$$
\boxed{\det A = 33}
$$
