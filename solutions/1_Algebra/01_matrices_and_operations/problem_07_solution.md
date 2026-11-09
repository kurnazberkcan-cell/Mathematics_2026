# Problem 7. Identity Matrix, Zero Matrix, and Powers

## Question

For

$$
A=
\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}
$$

compute $AI$, $IA$, $A+0$, $A^2$, $A^3$. Explain the roles of the matrices $I$ and $0$, and describe the pattern you observe in successive powers of $A$.

## Solution

Here $I$ is the $2\times2$ identity matrix and $0$ is the $2\times2$ zero matrix.

$$
I=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix},
$$

$$
0=
\begin{pmatrix}
0 & 0 \\
0 & 0 \\
\end{pmatrix}
$$

Multiplying by $I$ on either side leaves $A$ unchanged, and adding $0$ leaves $A$ unchanged:

$$
AI=IA=A=
\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix},
$$

$$
A+0=A
$$

So $I$ is the neutral element of multiplication and $0$ is the neutral element of addition.

Powers:

$$
A^2=A\cdot A=
\begin{pmatrix}
4 & 2+2 \\
0 & 4 \\
\end{pmatrix}
$$

$$
A^2=
\begin{pmatrix}
4 & 4 \\
0 & 4 \\
\end{pmatrix}
$$

$$
A^3=A^2A=
\begin{pmatrix}
8 & 4+8 \\
0 & 8 \\
\end{pmatrix}
$$

$$
A^3=
\begin{pmatrix}
8 & 12 \\
0 & 8 \\
\end{pmatrix}
$$

Pattern: the diagonal entries are $2^n$ and the upper-right entry is $n\cdot2^{n-1}$:

$$
A^n=
\begin{pmatrix}
2^n & n2^{n-1} \\
0 & 2^n \\
\end{pmatrix}.
$$

Check: for $n=2$ we get $2\cdot2=4$, and for $n=3$ we get $3\cdot4=12$, which agrees with the computed powers.
