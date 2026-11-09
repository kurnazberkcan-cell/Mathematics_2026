# Problem 13. Undoing a Composite Transformation

## Question

The matrices

$$
S=
\begin{pmatrix}
2 & 0 \\
0 & 1 \\
\end{pmatrix},
$$

$$
H=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}
$$

describe nonuniform scaling and shear. For $T=HS$, find $T^{-1}$ in two ways:

1. first compute $T$, then its inverse,
2. use $(HS)^{-1}=S^{-1}H^{-1}$.

Compare the results. Additionally compute $H^{-1}S^{-1}$ and verify that the incorrect order gives a different matrix. Explain the rule: when undoing a composition of operations, we undo them from the end.

## Solution

Method 1. The product is

$$
T=HS=
\begin{pmatrix}
2 & 1 \\
0 & 1 \\
\end{pmatrix}.
$$

Since $\det T=2$,

$$
T^{-1}=\frac{1}{2}
\begin{pmatrix}
1 & -1 \\
0 & 2 \\
\end{pmatrix}
$$

$$
T^{-1}=
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & 1 \\
\end{pmatrix}.
$$

Method 2. The individual inverses are

$$
S^{-1}=
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & 1 \\
\end{pmatrix},
$$

$$
H^{-1}=
\begin{pmatrix}
1 & -1 \\
0 & 1 \\
\end{pmatrix}.
$$

Then

$$
S^{-1}H^{-1}=
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & 1 \\
\end{pmatrix}.
$$

Both methods give the same matrix.

The incorrect order gives

$$
H^{-1}S^{-1}=
\begin{pmatrix}
\frac{1}{2} & -1 \\
0 & 1 \\
\end{pmatrix}.
$$

This differs from $T^{-1}$ in the entry in position $(1,2)$, where $-1\neq-\frac{1}{2}$.

Rule: $T=HS$ first scales and then shears. To return to the starting point, the shear, which was applied last, must be undone first, and the scaling afterwards. This is the product $S^{-1}H^{-1}$, in which $H^{-1}$ acts first on a vector.
