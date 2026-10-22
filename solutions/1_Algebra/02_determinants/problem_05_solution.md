**Solution:** Use row operations to reduce $A$ to an upper triangular matrix. Recall that adding a multiple of one row to another row does not change the determinant.

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 1 & 0 \\
-1 & 4 & 2
\end{pmatrix}
$$

**Step 1:** $R_2 \to R_2 - 2R_1$. This adds a multiple of another row, so the determinant **does not change**.

$$
\det A =
\det\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
-1 & 4 & 2
\end{pmatrix}
$$

**Step 2:** $R_3 \to R_3 + R_1$. This adds a multiple of another row, so the determinant **does not change**.

$$
\det A =
\det\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
0 & 6 & 5
\end{pmatrix}
$$

**Step 3:** $R_3 \to R_3 + 2R_2$. This adds a multiple of another row, so the determinant **does not change**.

$$
\det A =
\det\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
0 & 0 & -7
\end{pmatrix}
$$

**Result:** The matrix is now upper triangular, so its determinant is the product of the diagonal entries:

$$
\det A = 1\cdot(-3)\cdot(-7) = 21
$$

Since no row swaps or row scalings were used, the determinant stayed the same at every step.

**Check (cofactor expansion along the first row):**

$$
\det A = 1\cdot\det\begin{pmatrix} 1 & 0 \\ 4 & 2 \end{pmatrix}
- 2\cdot\det\begin{pmatrix} 2 & 0 \\ -1 & 2 \end{pmatrix}
+ 3\cdot\det\begin{pmatrix} 2 & 1 \\ -1 & 4 \end{pmatrix}
= 2 - 2\cdot 4 + 3\cdot 9 = 21
$$

$$
\boxed{\det A = 21}
$$
