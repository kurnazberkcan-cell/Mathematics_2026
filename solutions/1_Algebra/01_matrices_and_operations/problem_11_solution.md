## Results

$$
A^2=
\begin{pmatrix}
1 & 2 \\
0 & 1
\end{pmatrix},
\qquad
A^3=
\begin{pmatrix}
1 & 3 \\
0 & 1
\end{pmatrix},
\qquad
A^4=
\begin{pmatrix}
1 & 4 \\
0 & 1
\end{pmatrix}
$$

### Conjecture

$$
A^n=
\begin{pmatrix}
1 & n \\
0 & 1
\end{pmatrix}
\quad \text{for all } n \ge 1.
$$

### Inductive step

Assume $A^n=\begin{pmatrix}1 & n \\ 0 & 1\end{pmatrix}$. Then

$$
A^{n+1}=A^nA=
\begin{pmatrix}
1 & n \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
=
\begin{pmatrix}
1\cdot 1 + n\cdot 0 & 1\cdot 1 + n\cdot 1 \\
0\cdot 1 + 1\cdot 0 & 0\cdot 1 + 1\cdot 1
\end{pmatrix}
=
\begin{pmatrix}
1 & n+1 \\
0 & 1
\end{pmatrix}.
$$

This is exactly the formula for $n+1$. The base case $A^1 = A$ matches $n=1$, so by induction the formula holds for all $n \ge 1$.

### Why it works

Multiplying by $A$ leaves the diagonal entries at $1$ and the lower-left entry at $0$. In the upper-right entry, the existing $n$ is unchanged and a new $1$ is added, which increases it from $n$ to $n+1$.
