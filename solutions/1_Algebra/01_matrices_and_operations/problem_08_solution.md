# Problem 8. Row Operations and Their Reversibility

## Question

Given

$$
A=
\begin{pmatrix}
1 & 2 & -1 \\
2 & 4 & 1 \\
-1 & 1 & 3 \\
\end{pmatrix}
$$

perform, in order:

1. $R_2\leftarrow R_2-2R_1$,
2. $R_3\leftarrow R_3+R_1$,
3. interchange $R_2$ and $R_3$.

Write the matrix after each step. Then, for each of the three operations, state an operation that reverses it.

## Solution

Step 1: $R_2\leftarrow R_2-2R_1$. The new second row is $(2,4,1)-2(1,2,-1)=(0,0,3)$.

$$
\begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 3 \\
-1 & 1 & 3 \\
\end{pmatrix}
$$

Step 2: $R_3\leftarrow R_3+R_1$. The new third row is $(-1,1,3)+(1,2,-1)=(0,3,2)$.

$$
\begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 3 \\
0 & 3 & 2 \\
\end{pmatrix}
$$

Step 3: interchange $R_2$ and $R_3$.

$$
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 2 \\
0 & 0 & 3 \\
\end{pmatrix}
$$

Reversing operations:

- Step 1 is reversed by $R_2\leftarrow R_2+2R_1$, since $R_1$ is unchanged and we add back what was subtracted.
- Step 2 is reversed by $R_3\leftarrow R_3-R_1$.
- Step 3 is reversed by interchanging $R_2$ and $R_3$ again.

To undo the whole sequence, the reversing operations are applied in the opposite order: first the interchange, then $R_3\leftarrow R_3-R_1$, then $R_2\leftarrow R_2+2R_1$. This returns the original matrix $A$.
