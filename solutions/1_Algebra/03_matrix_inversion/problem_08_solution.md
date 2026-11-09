# Problem 8. Inverse of a Transformation

## Question

The matrix

$$
S=
\begin{pmatrix}
2 & 0 \\
0 & \frac{1}{2} \\
\end{pmatrix}
$$

describes a scaling of the plane. Find $S^{-1}$ and explain geometrically what the inverse transformation does. Check the action of the pair $S,S^{-1}$ on one simple vector.

## Solution

$S$ is diagonal with nonzero diagonal entries, so its inverse is diagonal with the reciprocals of these entries:

$$
S^{-1}=
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & 2 \\
\end{pmatrix}.
$$

Geometric meaning: $S$ stretches the plane by the factor $2$ in the direction of the $x$-axis and shrinks it by the factor $\frac{1}{2}$ in the direction of the $y$-axis. The inverse $S^{-1}$ shrinks by $\frac{1}{2}$ along the $x$-axis and stretches by $2$ along the $y$-axis, so it undoes the original scaling.

Check on the vector $v=(1,1)^T$:

$$
Sv=
\begin{pmatrix}
2 \\
\frac{1}{2} \\
\end{pmatrix},
$$

$$
S^{-1}(Sv)=
\begin{pmatrix}
\frac{1}{2}\cdot2 \\
2\cdot\frac{1}{2} \\
\end{pmatrix}
$$

$$
S^{-1}(Sv)=
\begin{pmatrix}
1 \\
1 \\
\end{pmatrix}=v.
$$
