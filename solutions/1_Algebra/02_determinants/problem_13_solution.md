## Exercise 13. Determinant by Elimination

Given

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 5 & 7 \\
1 & 0 & 2 \\
\end{pmatrix}
$$

Perform the row operations

$$
R_2\leftarrow R_2-2R_1
$$

$$
R_3\leftarrow R_3-R_1
$$

Both operations preserve the determinant.

The resulting matrix is

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & -2 & -1 \\
\end{pmatrix}
$$

Next, perform

$$
R_3\leftarrow R_3+2R_2
$$

This operation also preserves the determinant.

The matrix becomes

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 0 & 1 \\
\end{pmatrix}
$$

The matrix is now upper triangular. Its determinant is the product of the diagonal entries.

$$
\det A=1\cdot1\cdot1=1
$$

Therefore,

$$
\boxed{\det A=1}
$$
