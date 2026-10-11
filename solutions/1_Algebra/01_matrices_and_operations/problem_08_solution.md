## Results

After step 1, $R_2 \leftarrow R_2 - 2R_1$:

```math
\begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 3 \\
-1 & 1 & 3
\end{pmatrix}
```

After step 2, $R_3 \leftarrow R_3 + R_1$:

```math
\begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 3 \\
0 & 3 & 2
\end{pmatrix}
```

After step 3, interchange $R_2$ and $R_3$:

```math
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 2 \\
0 & 0 & 3
\end{pmatrix}
```

### Reverse operations

1. $R_2 \leftarrow R_2 - 2R_1$ is reversed by $R_2 \leftarrow R_2 + 2R_1$.
2. $R_3 \leftarrow R_3 + R_1$ is reversed by $R_3 \leftarrow R_3 - R_1$.
3. Interchanging $R_2$ and $R_3$ is reversed by interchanging $R_2$ and $R_3$ again.
