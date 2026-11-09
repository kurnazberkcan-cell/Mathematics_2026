# Problem 12. Formula for a Matrix Power

## Question

Let

$$
A=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}.
$$

Compute $A^2$, $A^3$, and $A^4$, and use them to formulate a conjecture for $A^n$. Then do not stop after checking one more case: assume the formula is true for $n$, multiply by $A$, and explain why you obtain exactly the formula for $n+1$.

## Solution

$$
A^2=
\begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix},
$$

$$
A^3=A^2A=
\begin{pmatrix}
1 & 3 \\
0 & 1 \\
\end{pmatrix},
$$

$$
A^4=A^3A=
\begin{pmatrix}
1 & 4 \\
0 & 1 \\
\end{pmatrix}.
$$

Conjecture: for every positive integer $n$,

$$
A^n=
\begin{pmatrix}
1 & n \\
0 & 1 \\
\end{pmatrix}.
$$

Inductive step: assume the formula holds for some $n$. Then

$$
A^{n+1}=A^nA=
\begin{pmatrix}
1 & n \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}
$$

$$
A^{n+1}=
\begin{pmatrix}
1 & 1+n \\
0 & 1 \\
\end{pmatrix}.
$$

This is exactly the formula with $n$ replaced by $n+1$. The formula holds for $n=1$, since $A^1=A$, so by induction it holds for all $n\geq1$.
