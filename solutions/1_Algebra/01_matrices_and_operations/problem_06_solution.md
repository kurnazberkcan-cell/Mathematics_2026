# Problem 6. Transpose

## Question

For

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
\end{pmatrix},
$$

$$
B=
\begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3 \\
\end{pmatrix}
$$

compute $A^T$, $B^T$, and $AB$. Then verify in this example that $(AB)^T=B^TA^T$.

## Solution

The transpose turns rows into columns.

$$
A^T=
\begin{pmatrix}
1 & 4 \\
2 & 5 \\
3 & 6 \\
\end{pmatrix}
$$

$$
B^T=
\begin{pmatrix}
1 & 2 & -1 \\
0 & 1 & 3 \\
\end{pmatrix}
$$

The product $AB$ is defined, since $A$ is $2\times3$ and $B$ is $3\times2$, and it has size $2\times2$.

$$
AB=
\begin{pmatrix}
1+4-3 & 0+2+9 \\
4+10-6 & 0+5+18 \\
\end{pmatrix}
$$

$$
AB=
\begin{pmatrix}
2 & 11 \\
8 & 23 \\
\end{pmatrix}
$$

Left-hand side:

$$
(AB)^T=
\begin{pmatrix}
2 & 8 \\
11 & 23 \\
\end{pmatrix}
$$

Right-hand side: $B^T$ is $2\times3$ and $A^T$ is $3\times2$, so $B^TA^T$ is $2\times2$.

$$
B^TA^T=
\begin{pmatrix}
1+4-3 & 4+10-6 \\
0+2+9 & 0+5+18 \\
\end{pmatrix}
$$

$$
B^TA^T=
\begin{pmatrix}
2 & 8 \\
11 & 23 \\
\end{pmatrix}
$$

Both sides are equal, so $(AB)^T=B^TA^T$ holds in this example.

The order of the factors is reversed. The product $A^TB^T$ is also defined here, because $A^T$ is $3\times2$ and $B^T$ is $2\times3$, but it has size $3\times3$ and is a different matrix from $(AB)^T$, which is $2\times2$.

$$
A^TB^T=
\begin{pmatrix}
1 & 6 & 11 \\
2 & 9 & 13 \\
3 & 12 & 15 \\
\end{pmatrix}
$$

So $(AB)^T\neq A^TB^T$ in this example, and the order cannot be kept.
