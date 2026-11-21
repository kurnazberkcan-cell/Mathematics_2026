## Exercise 11. Shortening the Calculation with Row Operations

Given

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
1 & 3 & 4 \\
1 & 4 & 6 \\
\end{pmatrix}
$$

Perform the row operations

$$
R_2\leftarrow R_2-R_1
$$

$$
R_3\leftarrow R_3-R_1
$$

These operations do not change the determinant because adding or subtracting a multiple of one row from another row preserves the determinant.

The resulting matrix is

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 2 & 3 \\
\end{pmatrix}
$$

Expanding along the first column gives

$$
\det A=
\begin{vmatrix}
1 & 1 \\
2 & 3 \\
\end{vmatrix}
$$

$$
\det A=1\cdot3-1\cdot2=1
$$

Therefore,

$$
\boxed{\det A=1}
$$
