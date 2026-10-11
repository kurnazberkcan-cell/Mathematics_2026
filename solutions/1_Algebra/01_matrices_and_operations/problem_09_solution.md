## Results

$$
Sx=
\begin{pmatrix}
2 \\
2
\end{pmatrix},
\qquad
RSx=
\begin{pmatrix}
-2 \\
2
\end{pmatrix}
$$

$$
Rx=
\begin{pmatrix}
-2 \\
1
\end{pmatrix},
\qquad
SRx=
\begin{pmatrix}
-4 \\
1
\end{pmatrix}
$$

### Comparison

$$
RSx =
\begin{pmatrix}
-2 \\
2
\end{pmatrix}
\neq
\begin{pmatrix}
-4 \\
1
\end{pmatrix}
= SRx
$$

Hence $RS \neq SR$.

### Geometric explanation

- $RSx$: $x$ is first stretched along the $x$-axis, then the stretched vector is rotated by $90^\circ$.
- $SRx$: $x$ is first rotated by $90^\circ$, then the result is stretched along the $x$-axis.
- Scaling acts on fixed coordinate axes. Rotating first changes which component of the vector lies along the stretched axis, so the stretch affects a different component. Therefore the order matters.
