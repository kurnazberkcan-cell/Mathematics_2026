# Exercise 12. A Parameter Revealed by a Row Operation

## Question

For the matrix

$$
A(t)=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 4 & t \\
0 & 1 & 1
\end{pmatrix}
$$

find all values of $t$ for which the matrix is not invertible.

Before computing the determinant, perform the row operation

$$
R_2 \leftarrow R_2 - 2R_1.
$$

Use the resulting matrix structure to determine the required values of $t$. At the end, explain what happens to the rows for the value of the parameter found.

## Solution

Apply the row operation

$$
R_2 \leftarrow R_2 - 2R_1.
$$

This operation does not change the determinant.

$$
\begin{pmatrix}
1 & 2 & 3 \\
2 & 4 & t \\
0 & 1 & 1
\end{pmatrix}
\longrightarrow
\begin{pmatrix}
1 & 2 & 3 \\
0 & 0 & t-6 \\
0 & 1 & 1
\end{pmatrix}
$$

Expanding the determinant along the second row gives

$$
\det A(t)=-(t-6)=6-t.
$$

The matrix is not invertible when its determinant is zero.

$$
6-t=0
$$

$$
t=6
$$

For $t=6$, the second row becomes

$$
(0,0,0).
$$

Therefore, the rows are linearly dependent, the determinant is zero, and the matrix is not invertible.

The only noninvertible value is $t=6$.
