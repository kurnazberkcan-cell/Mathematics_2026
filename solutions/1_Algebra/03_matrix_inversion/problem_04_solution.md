# Problem 4. Gauss-Jordan

## Question

Find $A^{-1}$ using the Gauss-Jordan method for

$$
A=
\begin{pmatrix}
1 & 2 \\
3 & 5 \\
\end{pmatrix}.
$$

Show the augmented matrix $[A\mid I]$ after successive operations and explain why obtaining $I$ on the left gives the inverse on the right.

## Solution

We start with the augmented matrix.

$$
\begin{pmatrix}
1 & 2 & \mid & 1 & 0 \\
3 & 5 & \mid & 0 & 1 \\
\end{pmatrix}
$$

Operation $R_2\leftarrow R_2-3R_1$:

$$
\begin{pmatrix}
1 & 2 & \mid & 1 & 0 \\
0 & -1 & \mid & -3 & 1 \\
\end{pmatrix}
$$

Operation $R_2\leftarrow -R_2$:

$$
\begin{pmatrix}
1 & 2 & \mid & 1 & 0 \\
0 & 1 & \mid & 3 & -1 \\
\end{pmatrix}
$$

Operation $R_1\leftarrow R_1-2R_2$:

$$
\begin{pmatrix}
1 & 0 & \mid & -5 & 2 \\
0 & 1 & \mid & 3 & -1 \\
\end{pmatrix}
$$

Hence

$$
A^{-1}=
\begin{pmatrix}
-5 & 2 \\
3 & -1 \\
\end{pmatrix}.
$$

Why this works: every row operation is multiplication on the left by an invertible elementary matrix. If $E_k\cdots E_1A=I$, then $E_k\cdots E_1=A^{-1}$. The same operations applied to $I$ give $E_k\cdots E_1I=A^{-1}$, so the right block becomes $A^{-1}$ at the moment the left block becomes $I$.

Verification:

$$
AA^{-1}=
\begin{pmatrix}
-5+6 & 2-2 \\
-15+15 & 6-5 \\
\end{pmatrix}
$$

$$
AA^{-1}=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}.
$$
