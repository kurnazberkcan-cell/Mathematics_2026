# Problem 15. Associativity of Multiplication and Different Calculation Paths

## Question

Given

$$
A=
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1 \\
\end{pmatrix},
$$

$$
B=
\begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3 \\
\end{pmatrix},
$$

$$
C=
\begin{pmatrix}
2 & 1 \\
0 & -1 \\
\end{pmatrix}.
$$

Compute $(AB)C$ and $A(BC)$. Compare the results and the number of intermediate operations. Explain what associativity of matrix multiplication means in this example.

## Solution

Path 1: $(AB)C$. First,

$$
AB=
\begin{pmatrix}
1+4+0 & 0+2+0 \\
0+2-1 & 0+1+3 \\
\end{pmatrix}
$$

$$
AB=
\begin{pmatrix}
5 & 2 \\
1 & 4 \\
\end{pmatrix}.
$$

Then

$$
(AB)C=
\begin{pmatrix}
10+0 & 5-2 \\
2+0 & 1-4 \\
\end{pmatrix}
$$

$$
(AB)C=
\begin{pmatrix}
10 & 3 \\
2 & -3 \\
\end{pmatrix}.
$$

Path 2: $A(BC)$. First,

$$
BC=
\begin{pmatrix}
2 & 1 \\
4 & 1 \\
-2 & -4 \\
\end{pmatrix}.
$$

Then

$$
A(BC)=
\begin{pmatrix}
2+8+0 & 1+2+0 \\
4-2 & 1-4 \\
\end{pmatrix}
$$

$$
A(BC)=
\begin{pmatrix}
10 & 3 \\
2 & -3 \\
\end{pmatrix}.
$$

Both paths give the same matrix.

Counting multiplications of numbers: for $(AB)C$, the product $AB$ has $4$ entries with $3$ multiplications each, which is $12$, and $(AB)C$ has $4$ entries with $2$ multiplications each, which is $8$. In total this is $20$. For $A(BC)$, the product $BC$ has $6$ entries with $2$ multiplications each, which is $12$, and $A(BC)$ has $4$ entries with $3$ multiplications each, which is $12$. In total this is $24$.

Associativity means that $(AB)C=A(BC)$ whenever the products are defined, so the grouping of the factors does not change the result. The final matrix is the same, but the amount of computation can differ, as seen here ($20$ versus $24$ multiplications).
