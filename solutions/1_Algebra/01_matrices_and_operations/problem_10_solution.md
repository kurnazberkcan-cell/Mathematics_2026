# Problem 10. Columns of a Matrix Product

## Question

Given

$$
A=
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1 \\
\end{pmatrix},
$$

$$
B=
\begin{pmatrix}
1 & 2 \\
-1 & 0 \\
3 & 1 \\
\end{pmatrix}.
$$

Denote the columns of $B$ by $b_1,b_2$.

1. Compute $Ab_1$ and $Ab_2$.
2. Compute the matrix $AB$.
3. Compare the results and explain why the columns of $AB$ are exactly the vectors $Ab_1$ and $Ab_2$.

## Solution

The columns of $B$ are

$$
b_1=
\begin{pmatrix}
1 \\
-1 \\
3 \\
\end{pmatrix},
$$

$$
b_2=
\begin{pmatrix}
2 \\
0 \\
1 \\
\end{pmatrix}.
$$

Part 1:

$$
Ab_1=
\begin{pmatrix}
1-2+0 \\
0-1+3 \\
\end{pmatrix}
=
\begin{pmatrix}
-1 \\
2 \\
\end{pmatrix},
$$

$$
Ab_2=
\begin{pmatrix}
2+0+0 \\
0+0+1 \\
\end{pmatrix}
=
\begin{pmatrix}
2 \\
1 \\
\end{pmatrix}.
$$

Part 2:

$$
AB=
\begin{pmatrix}
1-2+0 & 2+0+0 \\
0-1+3 & 0+0+1 \\
\end{pmatrix}
$$

$$
AB=
\begin{pmatrix}
-1 & 2 \\
2 & 1 \\
\end{pmatrix}
$$

Part 3: the first column of $AB$ is $(-1,2)^T=Ab_1$ and the second column is $(2,1)^T=Ab_2$.

This is not a coincidence. The entry of $AB$ in row $i$ and column $j$ is the dot product of row $i$ of $A$ with column $j$ of $B$. Collecting these entries for a fixed $j$ gives exactly the dot products of all rows of $A$ with $b_j$, which is by definition the vector $Ab_j$. Hence $AB=(Ab_1\ \ Ab_2)$.
