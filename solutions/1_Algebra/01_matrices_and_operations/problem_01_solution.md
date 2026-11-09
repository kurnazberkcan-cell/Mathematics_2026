# Problem 1. Matrix Size and Entries

## Question

Given

$$
A=
\begin{pmatrix}
2 & -1 & 3 \\
0 & 4 & 5 \\
\end{pmatrix},
$$

$$
B=
\begin{pmatrix}
1 & 0 \\
-2 & 3 \\
4 & 1 \\
\end{pmatrix}.
$$

1. State the sizes of matrices $A$ and $B$.
2. Read off the entries $a_{12}$, $a_{23}$, $b_{21}$, and $b_{32}$.
3. Write the second row of $A$ and the first column of $B$ as vectors.

## Solution

The size of a matrix is given as (number of rows) $\times$ (number of columns). The entry $a_{ij}$ lies in row $i$ and column $j$.

Part 1: the matrix $A$ has $2$ rows and $3$ columns, so $A$ is a $2\times3$ matrix. The matrix $B$ has $3$ rows and $2$ columns, so $B$ is a $3\times2$ matrix.

Part 2: we read each entry by its row index first and its column index second.

- $a_{12}$ is in row $1$, column $2$ of $A$, so $a_{12}=-1$.
- $a_{23}$ is in row $2$, column $3$ of $A$, so $a_{23}=5$.
- $b_{21}$ is in row $2$, column $1$ of $B$, so $b_{21}=-2$.
- $b_{32}$ is in row $3$, column $2$ of $B$, so $b_{32}=1$.

Part 3: the second row of $A$ is the row vector

$$
\begin{pmatrix}
0 & 4 & 5 \\
\end{pmatrix}.
$$

The first column of $B$ is the column vector

$$
\begin{pmatrix}
1 \\
-2 \\
4 \\
\end{pmatrix}.
$$

Verification: the second row of $A$ has $3$ entries, which matches the $3$ columns of $A$. The first column of $B$ has $3$ entries, which matches the $3$ rows of $B$.
