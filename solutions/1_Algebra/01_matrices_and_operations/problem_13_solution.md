## Results

```math
F^2 =
\begin{pmatrix}
2 & 1 \\
1 & 1
\end{pmatrix}
```

```math
F^3 =
\begin{pmatrix}
3 & 2 \\
2 & 1
\end{pmatrix}
```

```math
F^4 =
\begin{pmatrix}
5 & 3 \\
3 & 2
\end{pmatrix}
```

```math
F^5 =
\begin{pmatrix}
8 & 5 \\
5 & 3
\end{pmatrix}
```

### Relationship with the Fibonacci sequence

With $F_0 = 0, F_1 = 1, F_2 = 1, F_3 = 2, F_4 = 3, F_5 = 5, F_6 = 8, \ldots$, the pattern is:

```math
F^n =
\begin{pmatrix}
F_{n+1} & F_n \\
F_n & F_{n-1}
\end{pmatrix}
```

For example, $F^5$ contains $F_6 = 8$, $F_5 = 5$, and $F_4 = 3$.

### One recurrence step

```math
F
\begin{pmatrix}
a \\
b
\end{pmatrix}
=
\begin{pmatrix}
a + b \\
a
\end{pmatrix}
```

The first entry $a + b$ is the sum of the two consecutive terms, which is the next term of the sequence. The second entry $a$ is the larger of the two old terms, kept for the next step. So if $(a, b) = (F_{k+1}, F_k)$, then

```math
F
\begin{pmatrix}
F_{k+1} \\
F_k
\end{pmatrix}
=
\begin{pmatrix}
F_{k+2} \\
F_{k+1}
\end{pmatrix}
```

and applying $F$ repeatedly generates the whole sequence.
