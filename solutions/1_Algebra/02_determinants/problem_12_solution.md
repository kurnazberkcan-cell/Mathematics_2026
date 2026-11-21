## Exercise 12. A Parameter Revealed by a Row Operation

Given

$$
A(t)=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 4 & t \\
0 & 1 & 1 \\
\end{pmatrix}
$$

Perform the row operation

$$
R_2\leftarrow R_2-2R_1
$$

This operation does not change the determinant.

The resulting matrix is

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 0 & t-6 \\
0 & 1 & 1 \\
\end{pmatrix}
$$

Expanding along the first column gives

$$
\det A(t)=
\begin{vmatrix}
0 & t-6 \\
1 & 1 \\
\end{vmatrix}
$$

$$
\det A(t)=0\cdot1-(t-6)\cdot1=6-t
$$

The matrix is not invertible when its determinant is zero.

$$
6-t=0
$$

$$
\boxed{t=6}
$$

For $t=6$, the second row becomes the zero row after the row operation. This means the original second row is twice the first row, so the rows are linearly dependent.

Therefore, the matrix is not invertible for $t=6$.
