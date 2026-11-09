# Problem 9. Composing Transformations

## Question

Let

$$
S=
\begin{pmatrix}
2 & 0 \\
0 & 1 \\
\end{pmatrix},
$$

$$
R=
\begin{pmatrix}
0 & -1 \\
1 & 0 \\
\end{pmatrix}.
$$

The matrix $S$ describes nonuniform scaling, while $R$ describes a $90^\circ$ counterclockwise rotation. For

$$
x=
\begin{pmatrix}
1 \\
2 \\
\end{pmatrix}
$$

compute $RSx$ and $SRx$. Compare the results and explain geometrically why the order of these transformations matters.

## Solution

In $RSx$ the vector is first scaled by $S$ and then rotated by $R$. In $SRx$ it is first rotated and then scaled.

Computing $RSx$:

$$
Sx=
\begin{pmatrix}
2 \\
2 \\
\end{pmatrix}
$$

$$
RSx=R
\begin{pmatrix}
2 \\
2 \\
\end{pmatrix}
=
\begin{pmatrix}
-2 \\
2 \\
\end{pmatrix}
$$

Computing $SRx$:

$$
Rx=
\begin{pmatrix}
-2 \\
1 \\
\end{pmatrix}
$$

$$
SRx=S
\begin{pmatrix}
-2 \\
1 \\
\end{pmatrix}
=
\begin{pmatrix}
-4 \\
1 \\
\end{pmatrix}
$$

Verification through the products of matrices:

$$
RS=
\begin{pmatrix}
0 & -1 \\
2 & 0 \\
\end{pmatrix},
$$

$$
SR=
\begin{pmatrix}
0 & -2 \\
1 & 0 \\
\end{pmatrix}
$$

$$
RS
\begin{pmatrix}
1 \\
2 \\
\end{pmatrix}
=
\begin{pmatrix}
-2 \\
2 \\
\end{pmatrix},
$$

$$
SR
\begin{pmatrix}
1 \\
2 \\
\end{pmatrix}
=
\begin{pmatrix}
-4 \\
1 \\
\end{pmatrix}
$$

The results differ: $RSx=(-2,2)^T$ and $SRx=(-4,1)^T$, so $RS\neq SR$.

Geometric explanation: $S$ stretches only in the direction of the $x$-axis. If we scale first, the stretch acts on the original horizontal direction and then the stretched picture is rotated. If we rotate first, the horizontal direction has already become the vertical one, so $S$ now stretches the picture along the original vertical direction, which after rotation lies along the $x$-axis. Different directions are stretched, so the final images are different.
