## Exercise 1. Matrix Size and Entries

Given

$$
A=
\begin{pmatrix}
2 & -1 & 3 \\
0 & 4 & 5
\end{pmatrix},
\qquad
B=
\begin{pmatrix}
1 & 0 \\
-2 & 3 \\
4 & 1
\end{pmatrix}.
$$

1. State the sizes of matrices $A$ and $B$.
2. Read off the entries $a_{12}$, $a_{23}$, $b_{21}$, and $b_{32}$.
3. Write the second row of $A$ and the first column of $B$ as vectors.

> **Why this exercise:** builds basic fluency with matrix notation, indices, rows, and columns.

---

### Solution

**1. Sizes**

A matrix with $m$ rows and $n$ columns has size $m \times n$.

- $A$ has 2 rows and 3 columns, so $A$ is a $2 \times 3$ matrix.
- $B$ has 3 rows and 2 columns, so $B$ is a $3 \times 2$ matrix.

**2. Entries**

The entry $x_{ij}$ is located in row $i$ and column $j$.

| Entry    | Position           | Value |
|----------|--------------------|-------|
| $a_{12}$ | row 1, column 2 of $A$ | $-1$ |
| $a_{23}$ | row 2, column 3 of $A$ | $5$  |
| $b_{21}$ | row 2, column 1 of $B$ | $-2$ |
| $b_{32}$ | row 3, column 2 of $B$ | $1$  |

**3. Row and column vectors**

Second row of $A$:

$$
\begin{pmatrix} 0 & 4 & 5 \end{pmatrix}
$$

First column of $B$:

$$
\begin{pmatrix} 1 \\ -2 \\ 4 \end{pmatrix}
$$
