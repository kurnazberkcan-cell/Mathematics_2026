# Exercise 5. Determinant by Row Operations

## Question

Compute the determinant of the matrix using row operations. Show each operation and explain how it affects the determinant.

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 1 & 0 \\
-1 & 4 & 2
\end{pmatrix}
$$

## Solution

Start with the given matrix:

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 1 & 0 \\
-1 & 4 & 2
\end{pmatrix}
$$

First, apply the row operation

$$
R_2 \leftarrow R_2 - 2R_1.
$$

Adding a multiple of one row to another row does not change the determinant.

$$
\begin{pmatrix}
1 & 2 & 3 \\
2 & 1 & 0 \\
-1 & 4 & 2
\end{pmatrix}
\longrightarrow
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
-1 & 4 & 2
\end{pmatrix}
$$

Next, apply

$$
R_3 \leftarrow R_3 + R_1.
$$

This operation also preserves the determinant.

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
-1 & 4 & 2
\end{pmatrix}
\longrightarrow
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
0 & 6 & 5
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
0 & -3 & -6 \\
0 & 6 & 5
\end{pmatrix}
\longrightarrow
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
0 & 0 & -7
\end{pmatrix}
$$

The resulting matrix is upper triangular. Its determinant is the product of its diagonal entries.

$$
\det(A)=1\cdot(-3)\cdot(-7)
$$

$$
\det(A)=21
$$

All row operations used preserve the determinant. Therefore, the determinant of the original matrix is

$$
\boxed{\det(A)=21}
$$
