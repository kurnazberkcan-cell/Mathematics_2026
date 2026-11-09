# Problem 9. Matrix Equation

## Question

Given

$$
A=
\begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix},
$$

$$
B=
\begin{pmatrix}
3 & 1 \\
2 & 4 \\
\end{pmatrix}.
$$

Solve the equation $AX=B$ for $X$. Before calculating, decide on which side of the equation $A^{-1}$ must be used. Then check the result by computing $AX$.

## Solution

In $AX=B$ the matrix $A$ stands on the left of $X$. To cancel it, $A^{-1}$ must multiply both sides from the left:

$$
A^{-1}AX=A^{-1}B,
$$

$$
X=A^{-1}B.
$$

Multiplying from the right would give $AXA^{-1}=BA^{-1}$, which does not isolate $X$, because matrix multiplication is not commutative.

The determinant is $\det A=1$, hence

$$
A^{-1}=
\begin{pmatrix}
1 & -2 \\
0 & 1 \\
\end{pmatrix}.
$$

Then

$$
X=A^{-1}B=
\begin{pmatrix}
3-4 & 1-8 \\
2 & 4 \\
\end{pmatrix}
$$

$$
X=
\begin{pmatrix}
-1 & -7 \\
2 & 4 \\
\end{pmatrix}.
$$

Verification:

$$
AX=
\begin{pmatrix}
-1+4 & -7+8 \\
2 & 4 \\
\end{pmatrix}
$$

$$
AX=
\begin{pmatrix}
3 & 1 \\
2 & 4 \\
\end{pmatrix}=B.
$$
