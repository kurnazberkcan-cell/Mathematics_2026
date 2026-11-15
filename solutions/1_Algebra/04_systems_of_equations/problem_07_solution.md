# Exercise 7. Choosing a Method Deliberately
Do not solve all of the following systems completely. For each situation, choose the method that best uses its structure and justify your choice:

1. one system with a triangular coefficient matrix

$$
\begin{cases}
2x-y=3, \\
4y=8;
\end{cases}
$$

2. three systems $Ax=b_i$ with the same invertible matrix $A$, when $A^{-1}$ is already known;
3. one $3\times3$ system for which the inverse matrix is not given and the goal is only to find one solution vector.

For case 1, carry out the chosen method completely. For cases 2 and 3, describe the plan and indicate which part of the computation would be reusable or unnecessary. Do not judge a method by its name alone — refer to the number of right-hand sides and the structure of the matrix.
## Solution

**Case 1.** The matrix is already triangular, so the best choice is back substitution. No elimination is needed.

$$
4y=8\quad\Rightarrow\quad y=2
$$

$$
2x-2=3\quad\Rightarrow\quad x=\tfrac52
$$

$$
(x,y)=\left(\tfrac52,\;2\right)
$$

Check:

$$
2\cdot\tfrac52-2=3,
$$

$$
4\cdot2=8
$$

**Case 2.** There are three right-hand sides and one matrix $A$ with $A^{-1}$ already known. The best choice is to compute

$$
x_i=A^{-1}b_i,\qquad i=1,2,3
$$

Only three matrix-vector products are needed. The reusable part is $A^{-1}$ itself, which is computed once and serves all three systems. No elimination has to be repeated.

**Case 3.** There is one right-hand side and no inverse is given. The best choice is Gaussian elimination on the augmented matrix, followed by back substitution. Computing $A^{-1}$ would be unnecessary: it amounts to solving three extra systems (one per column of the identity matrix) whose answers are not needed for a single solution vector.
