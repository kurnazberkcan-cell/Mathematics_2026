## Results

```math
AB =
\begin{pmatrix}
a + c & b + d \\
c & d
\end{pmatrix}
```

```math
BA =
\begin{pmatrix}
a & a + b \\
c & c + d
\end{pmatrix}
```

### Conditions for AB = BA

Comparing entries:

```math
a + c = a \;\Rightarrow\; c = 0
```

```math
b + d = a + b \;\Rightarrow\; d = a
```

```math
c = c, \qquad d = c + d \;\Rightarrow\; c = 0
```

So the conditions are $c = 0$ and $d = a$, with $a$ and $b$ free.

### General form of B

```math
B =
\begin{pmatrix}
a & b \\
0 & a
\end{pmatrix}
= aI + bN,
\qquad
N =
\begin{pmatrix}
0 & 1 \\
0 & 0
\end{pmatrix}
```

Every matrix commuting with $A$ is upper triangular with equal diagonal entries.
