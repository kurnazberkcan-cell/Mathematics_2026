# Exercise 10. Detecting Dependence

## Question

Consider the matrix:

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 4 & 6 \\
0 & 1 & 5 \\
\end{pmatrix}
$$

Without carrying out a full determinant calculation:

1. Identify a specific dependence between the rows of the matrix.
2. Explain why this dependence implies that $\det A=0$.
3. Explain why the matrix is not invertible.

## Solution

The rows of the matrix are:

$$
R_1=(1,2,3)
$$

$$
R_2=(2,4,6)
$$

$$
R_3=(0,1,5)
$$

The second row is exactly twice the first row:

$$
R_2=2R_1
$$

Therefore, the rows are linearly dependent.

A square matrix with linearly dependent rows has a determinant equal to zero.

$$
\det A=0
$$

**Explanation of noninvertibility:**

A square matrix is invertible if and only if its determinant is nonzero.

Since the determinant of this matrix is zero, it is not invertible.

$$
A^{-1}\text{ does not exist}
$$

**Conclusion:**

The second row is twice the first row, which means that the rows are linearly dependent. This makes the determinant zero and proves that the matrix is not invertible.

---
