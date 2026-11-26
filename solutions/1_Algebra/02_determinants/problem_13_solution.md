# Exercise 13. Determinant by Elimination

## Question

Compute the determinant of

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 5 & 7 \\
1 & 0 & 2
\end{pmatrix}
$$

using elimination. Record the effect of every row operation used on the value of the determinant.

## Solution

Start with

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 5 & 7 \\
1 & 0 & 2
\end{pmatrix}.
$$

First, apply

$$
R_2 \leftarrow R_2 - 2R_1.
$$

Adding a multiple of one row to another row does not change the determinant.

$$
\begin{pmatrix}
1 & 2 & 3 \\
2 & 5 & 7 \\
1 & 0 & 2
\end{pmatrix}
\longrightarrow
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
1 & 0 & 2
\end{pmatrix}
$$

Next, apply

$$
R_3 \leftarrow R_3 - R_1.
$$

This operation also preserves the determinant.

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
1 & 0 & 2
\end{pmatrix}
\longrightarrow
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & -2 & -1
\end{pmatrix}
$$

Finally, apply

$$
R_3 \leftarrow R_3 + 2R_2.
$$

This operation also preserves the determinant.

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & -2 & -1
\end{pmatrix}
\longrightarrow
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 0 & 1
\end{pmatrix}
$$

The resulting matrix is upper triangular. Its determinant is the product of its diagonal entries.

$$
\det A = 1 \cdot 1 \cdot 1
$$

$$
\det A = 1
$$

All row operations used preserve the determinant. Therefore, the determinant of the original matrix is

$$
\det A = 1.
$$
