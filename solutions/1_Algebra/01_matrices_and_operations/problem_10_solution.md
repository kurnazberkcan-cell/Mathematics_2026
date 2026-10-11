## Results

$$
b_1=
\begin{pmatrix}
1 \\
-1 \\
3
\end{pmatrix},
\qquad
b_2=
\begin{pmatrix}
2 \\
0 \\
1
\end{pmatrix}
$$

$$
Ab_1=
\begin{pmatrix}
-1 \\
2
\end{pmatrix},
\qquad
Ab_2=
\begin{pmatrix}
2 \\
1
\end{pmatrix}
$$

$$
AB=
\begin{pmatrix}
-1 & 2 \\
2 & 1
\end{pmatrix}
=
\begin{pmatrix}
Ab_1 & Ab_2
\end{pmatrix}
$$

### Explanation

By the definition of matrix multiplication, the $j$-th column of $AB$ is $A$ times the $j$-th column of $B$:

$$
AB = A\begin{pmatrix} b_1 & b_2 \end{pmatrix} = \begin{pmatrix} Ab_1 & Ab_2 \end{pmatrix}.
$$

The entry in row $i$, column $j$ of $AB$ is (row $i$ of $A$) $\cdot$ (column $j$ of $B$), which is exactly the $i$-th entry of $Ab_j$. So the columns of $AB$ are exactly $Ab_1$ and $Ab_2$.
