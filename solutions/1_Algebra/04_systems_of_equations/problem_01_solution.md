### Exercise 1. From a System to a Matrix
Write the system

$$
\begin{cases}
2x-y+z=4, \\
x+3y-2z=1, \\
3x+y+z=7.
\end{cases}
$$

in the form $Ax=b$.
Identify the coefficient matrix, the vector of unknowns, and the right-hand side vector. Explain how each row of the matrix corresponds to one equation.

## Solution

$$
A=
\begin{pmatrix}
2 & -1 & 1 \\
1 & 3 & -2 \\
3 & 1 & 1 \\
\end{pmatrix},
$$

$$
x=
\begin{pmatrix}
x \\
y \\
z \\
\end{pmatrix},
$$

$$
b=
\begin{pmatrix}
4 \\
1 \\
7 \\
\end{pmatrix}
$$

The system is

$$
\begin{pmatrix}
2 & -1 & 1 \\
1 & 3 & -2 \\
3 & 1 & 1 \\
\end{pmatrix}
\begin{pmatrix}
x \\
y \\
z \\
\end{pmatrix}=
\begin{pmatrix}
4 \\
1 \\
7 \\
\end{pmatrix}
$$

Row $i$ of $A$ holds the coefficients of $x,y,z$ in equation $i$, and the $i$-th entry of $b$ is the right-hand side of equation $i$. For example, row 1 gives $2\cdot x+(-1)\cdot y+1\cdot z=4$, which is the first equation.
