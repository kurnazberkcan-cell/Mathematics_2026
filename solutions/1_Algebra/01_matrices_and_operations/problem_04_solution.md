# Problem 4. Matrix Multiplication and Noncommutativity

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
2 & 0 \\
3 & 1 \\
\end{pmatrix}.
$$

Compute $AB$ and $BA$. Is $AB=BA$? Use this example to explain what noncommutativity of matrix multiplication means.

## Solution

Each entry of a product is the dot product of a row of the left matrix with a column of the right matrix.

$$
AB=
\begin{pmatrix}
1\cdot2+2\cdot3 & 1\cdot0+2\cdot1 \\
0\cdot2+1\cdot3 & 0\cdot0+1\cdot1 \\
\end{pmatrix}
$$

$$
AB=
\begin{pmatrix}
8 & 2 \\
3 & 1 \\
\end{pmatrix}
$$

$$
BA=
\begin{pmatrix}
2\cdot1+0\cdot0 & 2\cdot2+0\cdot1 \\
3\cdot1+1\cdot0 & 3\cdot2+1\cdot1 \\
\end{pmatrix}
$$

$$
BA=
\begin{pmatrix}
2 & 4 \\
3 & 7 \\
\end{pmatrix}
$$

Since $AB\neq BA$ (for example, the entries in position $(1,1)$ are $8$ and $2$), the two products differ.

Both products are defined here, yet they are different matrices. This is what noncommutativity means: the order of the factors matters, and in general $AB\neq BA$, unlike multiplication of numbers.
