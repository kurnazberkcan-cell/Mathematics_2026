# Problem 5. Matrix Times Vector

## Question

Let

$$
A=
\begin{pmatrix}
2 & -1 \\
1 & 3 \\
\end{pmatrix},
$$

$$
x=
\begin{pmatrix}
4 \\
2 \\
\end{pmatrix}.
$$

Compute $Ax$. Then express $Ax$ as a linear combination of the columns of $A$, with coefficients coming from the vector $x$.

## Solution

Row by row:

$$
Ax=
\begin{pmatrix}
2\cdot4+(-1)\cdot2 \\
1\cdot4+3\cdot2 \\
\end{pmatrix}
$$

$$
Ax=
\begin{pmatrix}
6 \\
10 \\
\end{pmatrix}
$$

The product $Ax$ equals $x_1$ times the first column of $A$ plus $x_2$ times the second column of $A$. Here $x_1=4$ and $x_2=2$:

$$
Ax=4
\begin{pmatrix}
2 \\
1 \\
\end{pmatrix}
+2
\begin{pmatrix}
-1 \\
3 \\
\end{pmatrix}
$$

Verification:

$$
4
\begin{pmatrix}
2 \\
1 \\
\end{pmatrix}
+2
\begin{pmatrix}
-1 \\
3 \\
\end{pmatrix}
=
\begin{pmatrix}
8 \\
4 \\
\end{pmatrix}
+
\begin{pmatrix}
-2 \\
6 \\
\end{pmatrix}
$$

$$
\begin{pmatrix}
8 \\
4 \\
\end{pmatrix}
+
\begin{pmatrix}
-2 \\
6 \\
\end{pmatrix}
=
\begin{pmatrix}
6 \\
10 \\
\end{pmatrix}
$$

Both methods give the same vector.
