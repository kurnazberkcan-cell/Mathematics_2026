# Problem 13. A Recurrence Written in Matrix Form

## Question

Let

$$
F=
\begin{pmatrix}
1 & 1 \\
1 & 0 \\
\end{pmatrix}.
$$

Compute $F^2$, $F^3$, $F^4$, and $F^5$. Compare the numbers obtained with the sequence $0,1,1,2,3,5,8,\ldots$ and describe the relationship you observe. Then compute

$$
F
\begin{pmatrix}
a \\
b \\
\end{pmatrix}
$$

and explain how this multiplication performs one recurrence step: it creates the sum of two consecutive terms and keeps one of them for the next step.

## Solution

$$
F^2=
\begin{pmatrix}
2 & 1 \\
1 & 1 \\
\end{pmatrix},
$$

$$
F^3=F^2F=
\begin{pmatrix}
3 & 2 \\
2 & 1 \\
\end{pmatrix},
$$

$$
F^4=F^3F=
\begin{pmatrix}
5 & 3 \\
3 & 2 \\
\end{pmatrix},
$$

$$
F^5=F^4F=
\begin{pmatrix}
8 & 5 \\
5 & 3 \\
\end{pmatrix}.
$$

Let $F_0=0$, $F_1=1$, $F_2=1$, $F_3=2,\ldots$ be the Fibonacci numbers. The entries are exactly these numbers:

$$
F^n=
\begin{pmatrix}
F_{n+1} & F_n \\
F_n & F_{n-1} \\
\end{pmatrix}.
$$

For example, $F^5$ contains $F_6=8$, $F_5=5$, $F_4=3$.

Now the product with a vector:

$$
F
\begin{pmatrix}
a \\
b \\
\end{pmatrix}
=
\begin{pmatrix}
a+b \\
a \\
\end{pmatrix}.
$$

If $a$ and $b$ are two consecutive terms of the sequence, the first coordinate of the result is their sum, which is the next term. The second coordinate is $a$, the larger of the two old terms, which is kept for the next step. So the pair $(F_{k+1},F_k)^T$ is sent to $(F_{k+2},F_{k+1})^T$, and applying $F$ repeatedly generates the sequence. This is why the powers $F^n$ contain the Fibonacci numbers.
