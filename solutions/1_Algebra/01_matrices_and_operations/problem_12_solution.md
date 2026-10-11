## Results

```math
A^2 =
\begin{pmatrix}
1 & 2 \\
0 & 1
\end{pmatrix}
```

```math
A^3 =
\begin{pmatrix}
1 & 3 \\
0 & 1
\end{pmatrix}
```

```math
A^4 =
\begin{pmatrix}
1 & 4 \\
0 & 1
\end{pmatrix}
```

### Conjecture

```math
A^n =
\begin{pmatrix}
1 & n \\
0 & 1
\end{pmatrix},
\qquad n \ge 1
```

### Inductive step

Assume the formula holds for n. Then:

```math
A^{n+1} = A^n A =
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
1 & 1 + n \\
0 & 1
\end{pmatrix}
=
\begin{pmatrix}
1 & n + 1 \\
0 & 1
\end{pmatrix}
```

This is exactly the formula for n + 1. Since $A^1 = A$ matches the formula for n = 1, the formula holds for all $n \ge 1$ by induction.

### Why it works

Multiplying by $A$ keeps the diagonal entries equal to 1 and the lower-left entry equal to 0. In the upper-right entry, the existing value n is kept and a new 1 is added, so it becomes n + 1.
