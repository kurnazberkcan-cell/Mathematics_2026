## Results

```math
AI = A =
\begin{pmatrix}
2 & 1 \\
0 & 2
\end{pmatrix}
```

```math
IA = A =
\begin{pmatrix}
2 & 1 \\
0 & 2
\end{pmatrix}
```

```math
A + 0 = A =
\begin{pmatrix}
2 & 1 \\
0 & 2
\end{pmatrix}
```

```math
A^2 =
\begin{pmatrix}
4 & 4 \\
0 & 4
\end{pmatrix}
```

```math
A^3 =
\begin{pmatrix}
8 & 12 \\
0 & 8
\end{pmatrix}
```

### Roles of I and 0

- $I$ is the multiplicative identity: $AI = IA = A$.
- $0$ is the additive identity: $A + 0 = A$.

### Pattern in powers of A

```math
A^n =
\begin{pmatrix}
2^n & n \cdot 2^{n-1} \\
0 & 2^n
\end{pmatrix}
```

The diagonal entries double with each power, and the upper-right entry follows n · 2^(n-1), giving 1, 4, 12, ...
