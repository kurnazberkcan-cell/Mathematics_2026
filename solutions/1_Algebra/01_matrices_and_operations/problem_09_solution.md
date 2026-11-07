# Exercise 8. Row Operations and Their Reversibility

## Exercise Statement

Given:

\[
A=
\begin{pmatrix}
1&2&-1\\
2&4&1\\
-1&1&3
\end{pmatrix}
\]

Perform the following operations in order:

1. \(R_2\leftarrow R_2-2R_1\)
2. \(R_3\leftarrow R_3+R_1\)
3. Interchange \(R_2\) and \(R_3\).

Write the matrix after each step. Then, for each of the three operations, state an operation that reverses it.

## Solution

### Initial Matrix

\[
A=
\begin{pmatrix}
1&2&-1\\
2&4&1\\
-1&1&3
\end{pmatrix}
\]

### Step 1

Apply:

\[
R_2\leftarrow R_2-2R_1
\]

Calculate the second row:

\[
(2,4,1)-2(1,2,-1)
\]

\[
=(2,4,1)-(2,4,-2)
\]

\[
=(0,0,3)
\]

Therefore:

\[
A_1=
\begin{pmatrix}
1&2&-1\\
0&0&3\\
-1&1&3
\end{pmatrix}
\]

**Reverse operation:**

\[
R_2\leftarrow R_2+2R_1
\]

### Step 2

Apply:

\[
R_3\leftarrow R_3+R_1
\]

Calculate the third row:

\[
(-1,1,3)+(1,2,-1)
\]

\[
=(0,3,2)
\]

Therefore:

\[
A_2=
\begin{pmatrix}
1&2&-1\\
0&0&3\\
0&3&2
\end{pmatrix}
\]

**Reverse operation:**

\[
R_3\leftarrow R_3-R_1
\]

### Step 3

Interchange rows 2 and 3:

\[
R_2\leftrightarrow R_3
\]

Therefore:

\[
\boxed{
A_3=
\begin{pmatrix}
1&2&-1\\
0&3&2\\
0&0&3
\end{pmatrix}
}
\]

**Reverse operation:**

\[
R_2\leftrightarrow R_3
\]

### Explanation

Each elementary row operation is reversible.

- Adding a multiple of one row to another is reversed by subtracting the same multiple.
- Interchanging two rows is reversed by performing the same interchange again.

These operations are important in Gaussian elimination and solving systems of linear equations.
