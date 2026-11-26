# Exercise 14. A System of Equations and the Determinant

## Question

Consider the system $Ax=b$, where

$$
A=
\begin{pmatrix}
1 & 2 \\
k & 4
\end{pmatrix}.
$$

Determine the values of $k$ for which the system has exactly one solution for every right-hand side $b$.

For the remaining value of $k$, give:
- An example of a right-hand side $b$ for which the system has infinitely many solutions.
- An example of a right-hand side $b$ for which the system has no solution.

## Solution

A system $Ax=b$ has exactly one solution for every $b$ if and only if the matrix $A$ is invertible.

Calculate the determinant:

$$
\det A =
\begin{vmatrix}
1 & 2 \\
k & 4
\end{vmatrix}
$$

$$
\det A = 4-2k
$$

The matrix is invertible when

$$
4-2k \neq 0
$$

$$
k \neq 2
$$

Therefore, the system has exactly one solution for every $b$ when $k \neq 2$.

For the exceptional value $k=2$, the matrix becomes

$$
A=
\begin{pmatrix}
1 & 2 \\
2 & 4
\end{pmatrix}.
$$

The corresponding system is

$$
\begin{cases}
x_1+2x_2=b_1 \\
2x_1+4x_2=b_2
\end{cases}
$$

The second equation has a left-hand side that is twice the first equation.

**Example 1: Infinitely many solutions**

Choose

$$
b=
\begin{pmatrix}
1 \\
2
\end{pmatrix}.
$$

The system becomes

$$
\begin{cases}
x_1+2x_2=1 \\
2x_1+4x_2=2
\end{cases}
$$

The second equation is twice the first equation. Therefore, there is only one independent equation with two unknowns, giving infinitely many solutions.

**Example 2: No solution**

Choose

$$
b=
\begin{pmatrix}
1 \\
3
\end{pmatrix}.
$$

The system becomes

$$
\begin{cases}
x_1+2x_2=1 \\
2x_1+4x_2=3
\end{cases}
$$

The second equation would require the left-hand side to equal $2$, while its right-hand side is $3$. This is a contradiction.

Therefore, the system has no solution.

In conclusion:
- For $k \neq 2$, the system has exactly one solution for every $b$.
- For $k=2$, the system may have infinitely many solutions or no solution, depending on $b$.
