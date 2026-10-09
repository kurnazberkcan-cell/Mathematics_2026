## Exercise 2. Addition and Scalar Multiplication

For

$$
A=
\begin{pmatrix}
1 & 2 \\
-1 & 3
\end{pmatrix},
\qquad
B=
\begin{pmatrix}
4 & -2 \\
0 & 5
\end{pmatrix}
$$

compute

$$
A+B,\qquad A-B,\qquad 3A-2B.
$$

Explain why matrix addition is possible only for matrices of the same size.

> **Why this exercise:** reinforces entry-by-entry operations and the importance of compatible dimensions.

---

### Solution

Addition, subtraction, and scalar multiplication are performed entry by entry.

**1. Sum**

$$
A+B=
\begin{pmatrix}
1+4 & 2+(-2) \\
-1+0 & 3+5
\end{pmatrix}
=
\begin{pmatrix}
5 & 0 \\
-1 & 8
\end{pmatrix}
$$

**2. Difference**

$$
A-B=
\begin{pmatrix}
1-4 & 2-(-2) \\
-1-0 & 3-5
\end{pmatrix}
=
\begin{pmatrix}
-3 & 4 \\
-1 & -2
\end{pmatrix}
$$

**3. Linear combination**

$$
3A=
\begin{pmatrix}
3 & 6 \\
-3 & 9
\end{pmatrix},
\qquad
2B=
\begin{pmatrix}
8 & -4 \\
0 & 10
\end{pmatrix}
$$

$$
3A-2B=
\begin{pmatrix}
3-8 & 6-(-4) \\
-3-0 & 9-10
\end{pmatrix}
=
\begin{pmatrix}
-5 & 10 \\
-3 & -1
\end{pmatrix}
$$

**4. Why the sizes must match**

Matrix addition is defined by

$$
(A+B)_{ij} = a_{ij} + b_{ij}.
$$

This formula needs every position $(i,j)$ of $A$ to have a matching entry at the same position in $B$. If $A$ and $B$ have different sizes, some entries of one matrix have no partner in the other, so the sum is not defined. For example, a $2\times 3$ matrix cannot be added to a $3\times 2$ matrix.
