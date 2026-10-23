## Problem 9

**Question:** Let $u = \begin{pmatrix} 3 \\ 1 \end{pmatrix}$ and $v = \begin{pmatrix} 1 \\ 4 \end{pmatrix}$. Compute the signed determinant of the matrix whose columns are $(u, v)$ and the area of the parallelogram spanned by $u$ and $v$. Then reverse the order of the vectors to $(v, u)$ and repeat. Explain what changes and what does not.

### Solution

**Original order $(u, v)$:**

$$
M = \begin{pmatrix} 3 & 1 \\ 1 & 4 \end{pmatrix}, \qquad
\det M = 3\cdot 4 - 1\cdot 1 = 11
$$

$$
\text{Area} = |\det M| = 11
$$

**Reversed order $(v, u)$:**

$$
M' = \begin{pmatrix} 1 & 3 \\ 4 & 1 \end{pmatrix}, \qquad
\det M' = 1\cdot 1 - 3\cdot 4 = 1 - 12 = -11
$$

$$
\text{Area} = |\det M'| = |-11| = 11
$$

**What changes and what does not.** Reversing the order of the vectors swaps the two columns of the matrix. Swapping two columns multiplies the determinant by $-1$, so $\det M' = -\det M$: the determinant changes sign from $+11$ to $-11$. The sign records the orientation of the ordered pair: $(u, v)$ is positively oriented (counterclockwise), while $(v, u)$ is negatively oriented (clockwise).

The area does not change, because the parallelogram spanned by $u$ and $v$ is the same set of points regardless of the order in which the vectors are listed. The area is the
