## Problem 5

**Question:** Let

$$
A = \begin{pmatrix} 1 & 2 & 3 \\ 2 & 1 & 0 \\ -1 & 4 & 2 \end{pmatrix}.
$$

Compute $\det A$ by reducing $A$ to an upper triangular matrix using row operations. Keep track of each row operation and state how it affects the determinant.

### Solution

Use row operations to reduce $A$ to an upper triangular matrix. Recall that adding a multiple of one row to another row does not change the determinant.

$$
A = \begin{pmatrix} 1 & 2 & 3 \\ 2 & 1 & 0 \\ -1 & 4 & 2 \end{pmatrix}
$$

**Step 1:** $R_2 \to R_2 - 2R_1$. This adds a multiple of another row, so the determinant does not change.

$$
\det A = \det\begin{pmatrix} 1 & 2 & 3 \\ 0 & -3 & -6 \\ -1 & 4 & 2 \end{pmatrix}
$$

**Step 2:** $R_3 \to R_3 + R_1$. This adds a multiple of another row, so the determinant does not change.

$$
\det A = \det\begin{pmatrix} 1 & 2 & 3 \\ 0 & -3 & -6 \\ 0 & 6 & 5 \end{pmatrix}
$$

**Step 3:** $R_3 \to R_3 + 2R_2$. This adds a
