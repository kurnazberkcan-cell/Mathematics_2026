**Solution:** A square matrix is invertible if and only if its determinant is nonzero. So $A(t)$ is not invertible exactly when $\det A(t) = 0$.

Compute the determinant:

$$
\det A(t) = \det\begin{pmatrix} t & 1 \\ 2 & t \end{pmatrix} = t\cdot t - 1\cdot 2 = t^2 - 2
$$

Set it equal to zero:

$$
t^2 - 2 = 0 \quad\Longrightarrow\quad t^2 = 2 \quad\Longrightarrow\quad t = \sqrt{2} \ \text{ or } \ t = -\sqrt{2}
$$

Therefore $A(t)$ is not invertible exactly for

$$
\boxed{t = \pm\sqrt{2}}
$$

**Relation to the determinant being zero:**

For a $2\times 2$ matrix, the inverse is given by

$$
A^{-1} = \frac{1}{\det A}\begin{pmatrix} d & -b \\ -c & a \end{pmatrix}
$$

which exists only if $\det A \neq 0$. When $\det A(t) = t^2 - 2 = 0$, the formula would require division by zero, so no inverse exists.

**Check:** For $t = \sqrt{2}$,

$$
A(\sqrt{2}) = \begin{pmatrix} \sqrt{2} & 1 \\ 2 & \sqrt{2} \end{pmatrix}
$$

The second row equals $\sqrt{2}$ times the first row, since $\sqrt{2}\cdot\sqrt{2} = 2$ and $\sqrt{2}\cdot 1 = \sqrt{2}$. The rows are linearly dependent, so the determinant is $0$ and the matrix is not invertible. The case $t = -\sqrt{2}$ works the same way, with the second row equal to $-\sqrt{2}$ times the first row.
