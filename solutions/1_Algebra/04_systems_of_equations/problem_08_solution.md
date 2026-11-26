# Exercise 8. Two Systems with the Same Coefficient Matrix

## Question

Solve by elimination the following two systems:

**First system:**

$$
\begin{cases}
2x+y=5, \\
x-y=1.
\end{cases}
$$

**Second system:**

$$
\begin{cases}
2x+y=1, \\
x-y=4.
\end{cases}
$$

Compare the successive elimination steps. Which part of the calculation is the same in both cases, and why?

## Solution

### First system

Write the augmented matrix:

$$
\begin{pmatrix}
2 & 1 & \mid & 5 \\
1 & -1 & \mid & 1
\end{pmatrix}
$$

Swap $R_1$ and $R_2$:

$$
\begin{pmatrix}
1 & -1 & \mid & 1 \\
2 & 1 & \mid & 5
\end{pmatrix}
$$

Apply the row operation:

$$
R_2 \leftarrow R_2-2R_1
$$

$$
\begin{pmatrix}
1 & -1 & \mid & 1 \\
0 & 3 & \mid & 3
\end{pmatrix}
$$

From the second row:

$$
3y=3
$$

$$
y=1
$$

Substitute into the first equation:

$$
x-1=1
$$

$$
x=2
$$

The solution is

$$
(x,y)=(2,1).
$$

### Second system

Write the augmented matrix:

$$
\begin{pmatrix}
2 & 1 & \mid & 1 \\
1 & -1 & \mid & 4
\end{pmatrix}
$$

Swap $R_1$ and $R_2$:

$$
\begin{pmatrix}
1 & -1 & \mid & 4 \\
2 & 1 & \mid & 1
\end{pmatrix}
$$

Apply the same row operation:

$$
R_2 \leftarrow R_2-2R_1
$$

$$
\begin{pmatrix}
1 & -1 & \mid & 4 \\
0 & 3 & \mid & -7
\end{pmatrix}
$$

From the second row:

$$
3y=-7
$$

$$
y=-\frac{7}{3}
$$

Substitute into the first equation:

$$
x+\frac{7}{3}=4
$$

$$
x=\frac{5}{3}
$$

The solution is

$$
(x,y)=\left(\frac{5}{3},-\frac{7}{3}\right).
$$

### Verification

For the first system:

$$
2(2)+1=5
$$

$$
2-1=1
$$

For the second system:

$$
2\cdot\frac{5}{3}-\frac{7}{3}=1
$$

$$
\frac{5}{3}+\frac{7}{3}=4
$$

Both solutions satisfy their respective systems.

### Comparison

The row operations are the same in both systems:

1. Swap $R_1$ and $R_2$.
2. Apply $R_2 \leftarrow R_2-2R_1$.

The resulting coefficient matrix is also identical:

$$
\begin{pmatrix}
1 & -1 \\
0 & 3
\end{pmatrix}
$$

The row operations depend only on the coefficients of the variables, not on the right-hand side.

Therefore, the elimination steps for the coefficient part are identical, while the last column changes because the right-hand sides are different.
