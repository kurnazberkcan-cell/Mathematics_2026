# Problem 10. Inverse of a Diagonal Matrix

## Question

Given

$$
D=
\begin{pmatrix}
2 & 0 & 0 \\
0 & -3 & 0 \\
0 & 0 & 5 \\
\end{pmatrix},
$$

$$
E=
\begin{pmatrix}
2 & 0 & 0 \\
0 & 0 & 0 \\
0 & 0 & 5 \\
\end{pmatrix}.
$$

Without using Gauss-Jordan elimination, decide which matrix is invertible. For the invertible matrix, give the inverse and check the result by multiplication.

## Solution

The determinant of a diagonal matrix is the product of its diagonal entries. Hence $\det D=2\cdot(-3)\cdot5=-30\neq0$, so $D$ is invertible. For $E$ we get $\det E=2\cdot0\cdot5=0$; moreover $E$ has a zero row, so $E$ is not invertible.

The inverse of the invertible diagonal matrix $D$ is the diagonal matrix of reciprocals:

$$
D^{-1}=
\begin{pmatrix}
\frac{1}{2} & 0 & 0 \\
0 & -\frac{1}{3} & 0 \\
0 & 0 & \frac{1}{5} \\
\end{pmatrix}.
$$

Verification:

$$
DD^{-1}=
\begin{pmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1 \\
\end{pmatrix}.
$$

Each diagonal entry of the product is $d_i\cdot\frac{1}{d_i}=1$, and all other entries are $0$.
