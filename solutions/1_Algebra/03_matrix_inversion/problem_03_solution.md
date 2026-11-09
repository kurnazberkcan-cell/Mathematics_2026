# Problem 3. When Does the Inverse Not Exist?

## Question

For

$$
A=
\begin{pmatrix}
2 & 4 \\
1 & 2 \\
\end{pmatrix}
$$

explain in two ways why $A^{-1}$ does not exist: using the determinant and using dependence between the rows.

## Solution

Method 1: determinant. We have

$$
\det A = 2\cdot2-4\cdot1 = 0.
$$

The inverse formula for a $2\times2$ matrix requires division by $\det A$, which is impossible here. A square matrix is invertible if and only if its determinant is nonzero, so $A^{-1}$ does not exist.

Method 2: dependence of rows. The first row is twice the second row:

$$
(2,4)=2\cdot(1,2).
$$

The rows are linearly dependent. Row operations can therefore produce a zero row. Indeed, $R_1\leftarrow R_1-2R_2$ gives

$$
\begin{pmatrix}
0 & 0 \\
1 & 2 \\
\end{pmatrix}.
$$

A matrix with a zero row cannot be transformed into $I$, and for any matrix $X$ the first row of $AX$ would be a combination of... in fact the product $AX$ always has its first row equal to twice its second row, so $AX=I$ is impossible, because $I$ does not have this property.

Both arguments agree: dependent rows correspond to $\det A=0$, and such a matrix is not invertible.
