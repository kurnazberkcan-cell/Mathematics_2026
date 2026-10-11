## Results

```math
AB =
\begin{pmatrix}
5 & 2 \\
1 & 4
\end{pmatrix}
```

```math
(AB)C =
\begin{pmatrix}
5 & 2 \\
1 & 4
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
0 & -1
\end{pmatrix}
=
\begin{pmatrix}
10 & 3 \\
2 & -3
\end{pmatrix}
```

```math
BC =
\begin{pmatrix}
2 & 1 \\
4 & 1 \\
-2 & -4
\end{pmatrix}
```

```math
A(BC) =
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
4 & 1 \\
-2 & -4
\end{pmatrix}
=
\begin{pmatrix}
10 & 3 \\
2 & -3
\end{pmatrix}
```

### Comparison

```math
(AB)C = A(BC) =
\begin{pmatrix}
10 & 3 \\
2 & -3
\end{pmatrix}
```

### Number of operations

| Order | Intermediate product | Multiplications | Additions |
|---|---|---|---|
| $(AB)C$ | $AB$ is $2\times 2$ | $12 + 8 = 20$ | $8 + 4 = 12$ |
| $A(BC)$ | $BC$ is $3\times 2$ | $12 + 12 = 24$ | $6 + 8 = 14$ |

Both groupings give the same matrix, but $(AB)C$ needs fewer operations here because its intermediate matrix is smaller.

### Meaning of associativity

Associativity means the grouping of the factors does not change the result:

```math
(AB)C = A(BC)
```

In this example, applying $B$ and then $A$ first (as $AB$) and then $C$ gives the same final matrix as first combining $B$ and $C$ and then applying $A$. The order of the matrices stays the same; only the placement of parentheses changes, and this affects the cost of computing the product, not its value.
