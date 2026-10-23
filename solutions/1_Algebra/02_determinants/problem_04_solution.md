## Problem 4

**Question:** Compute the determinant of

$$
A = \begin{pmatrix} 2 & 4 & 1 \\ 0 & -3 & 5 \\ 0 & 0 & 7 \end{pmatrix}
$$

without expanding it in the usual full way, by using the structure of the matrix. Explain the general rule behind your computation.

### Rule

The determinant of a triangular matrix (upper or lower) is the product of its diagonal entries. For an $n \times n$ triangular matrix $T$ with diagonal entries $t_{11}, t_{22}, \dots, t_{nn}$:

$$
\det T = t_{11}\, t_{22} \cdots t_{nn}
$$

### Solution

The matrix $A$ is upper triangular, since all entries below the main diagonal are zero. Its diagonal entries are $2$, $-3$ and $7$, so

$$
\det A = 2\cdot(-3)\cdot 7 = -42
$$

**Why the rule works (using this example).** Expand along the first column. It contains only one nonzero entry, $2$, so

$$
\det A = 2\cdot\det\begin{pmatrix} -3 & 5 \\ 0 & 7 \end{pmatrix}
$$

Now expand the $2\times 2$ matrix along its first column. Again only the top entry survives:

$$
\det\begin{pmatrix} -3 & 5 \\ 0 & 7 \end{pmatrix} = (-3)\cdot 7 = -21
$$

Each step removes one row and one column and leaves only the diagonal entry, so the entries above the diagonal ($4$, $1$, $5$) never affect the result. The same argument works for any size, and for lower triangular matrices (expand along the first row instead).

### Conclusion

$$
\det A = 2\cdot(-3)\cdot 7 = -42
$$
