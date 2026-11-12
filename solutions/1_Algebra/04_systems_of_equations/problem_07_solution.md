# Exercise 7. Choosing a Method Deliberately

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
