# Exercise 11. Shortening the Calculation with Row Operations

## Question

Compute the determinant of the following matrix:

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
1 & 3 & 4 \\
1 & 4 & 6 \\
\end{pmatrix}
$$

Perform row operations to create as many zeros as possible before calculating the determinant.

State which row operations leave the determinant unchanged and explain their effect on the calculation.

## Solution

Start with:

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
1 & 3 & 4 \\
1 & 4 & 6 \\
\end{pmatrix}
$$

**Step 1:** Apply $R_2\rightarrow R_2-R_1$.

Adding a multiple of one row to another does not change the determinant.

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
1 & 4 & 6 \\
\end{pmatrix}
$$

**Step 2:** Apply $R_3\rightarrow R_3-R_1$.

This operation also preserves the determinant.

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 2 & 3 \\
\end{pmatrix}
$$

**Step 3:** Apply $R_3\rightarrow R_3-2R_2$.

This operation also preserves the determinant.

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 0 & 1 \\
\end{pmatrix}
$$

The resulting matrix is upper triangular. Its determinant is the product of its diagonal entries.

$$
\det A=1\cdot1\cdot1=1
$$

Therefore, the determinant of the original matrix is $\det A=1$.

**Conclusion:**

All three operations involved adding a multiple of one row to another. Therefore, none of them changed the determinant.

Creating zeros below the main diagonal transformed the matrix into upper triangular form and simplified the determinant calculation.

---
