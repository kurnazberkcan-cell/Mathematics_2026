# Problem 7. Inverse of a Product

## Question

For

$$
A=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix},
$$

$$
B=
\begin{pmatrix}
2 & 0 \\
0 & 3 \\
\end{pmatrix}
$$

compute $(AB)^{-1}$ and $B^{-1}A^{-1}$. Check that the results are the same and explain the meaning of the reversed order.

## Solution

First the product:

$$
AB=
\begin{pmatrix}
2 & 3 \\
0 & 3 \\
\end{pmatrix}.
$$

Its determinant is $\det(AB)=6$, so

$$
(AB)^{-1}=\frac{1}{6}
\begin{pmatrix}
3 & -3 \\
0 & 2 \\
\end{pmatrix}
$$

$$
(AB)^{-1}=
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & \frac{1}{3} \\
\end{pmatrix}.
$$

The individual inverses are

$$
A^{-1}=
\begin{pmatrix}
1 & -1 \\
0 & 1 \\
\end{pmatrix},
$$

$$
B^{-1}=
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & \frac{1}{3} \\
\end{pmatrix}.
$$

Then

$$
B^{-1}A^{-1}=
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & \frac{1}{3} \\
\end{pmatrix}.
$$

The two results coincide: $(AB)^{-1}=B^{-1}A^{-1}$.

Meaning of the reversed order: $AB$ means first applying $B$ and then $A$. To undo this, the last operation must be undone first, so we apply $A^{-1}$ first and then $B^{-1}$, which is the product $B^{-1}A^{-1}$. Algebraically,

$$
(AB)(B^{-1}A^{-1})=A(BB^{-1})A^{-1}=AA^{-1}=I.
$$
