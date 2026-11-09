# Problem 14. A Matrix That Is Its Own Inverse

## Question

Assume that a square matrix $A$ satisfies $A^2=I$. Show that $A^{-1}=A$. Then give an example of a $2\times2$ matrix different from $I$ and $-I$ that satisfies this condition, and verify it by multiplication.

## Solution

Proof. The inverse of $A$ is the matrix $X$ with $AX=XA=I$. The assumption $A^2=I$ says $AA=I$, which is exactly this condition for $X=A$ (both products are $AA$). By uniqueness of the inverse, $A^{-1}=A$.

Example: take the matrix that swaps coordinates,

$$
A=
\begin{pmatrix}
0 & 1 \\
1 & 0 \\
\end{pmatrix}.
$$

It is different from $I$ and from $-I$. Verification:

$$
A^2=
\begin{pmatrix}
0\cdot0+1\cdot1 & 0\cdot1+1\cdot0 \\
1\cdot0+0\cdot1 & 1\cdot1+0\cdot0 \\
\end{pmatrix}
$$

$$
A^2=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}=I.
$$

Geometrically, swapping the coordinates twice returns every vector to its original position, so the transformation is its own inverse.
