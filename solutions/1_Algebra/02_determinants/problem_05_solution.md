# Exercise 5. Row Operations

## Question

Consider the matrix:

\[
A=
\begin{pmatrix}
1 & 2 & 3\\
2 & 1 & 0\\
-1 & 4 & 2
\end{pmatrix}
\]

Find \(\det A\) by simplifying the matrix using elementary row operations.

At each step, indicate whether and how the determinant changes.

## Solution

Start with:

\[
A=
\begin{pmatrix}
1 & 2 & 3\\
2 & 1 & 0\\
-1 & 4 & 2
\end{pmatrix}
\]

**Step 1:** Apply \(R_2\rightarrow R_2-2R_1\).

Adding a multiple of one row to another does not change the determinant.

\[
\begin{pmatrix}
1 & 2 & 3\\
0 & -3 & -6\\
-1 & 4 & 2
\end{pmatrix}
\]

**Step 2:** Apply \(R_3\rightarrow R_3+R_1\).

This operation also does not change the determinant.

\[
\begin{pmatrix}
1 & 2 & 3\\
0 & -3 & -6\\
0 & 6 & 5
\end{pmatrix}
\]

**Step 3:** Apply \(R_3\rightarrow R_3+2R_2\).

This operation also preserves the determinant.

\[
\begin{pmatrix}
1 & 2 & 3\\
0 & -3 & -6\\
0 & 0 & -7
\end{pmatrix}
\]

The resulting matrix is upper triangular. Its determinant is the product of its diagonal entries.

\[
\det A=1\cdot(-3)\cdot(-7)
\]

\[
\boxed{\det A=21}
\]

**Conclusion:**

All three row operations involved adding a multiple of one row to another. These operations do not change the determinant. Therefore, the determinant of the original matrix is \(21\).
