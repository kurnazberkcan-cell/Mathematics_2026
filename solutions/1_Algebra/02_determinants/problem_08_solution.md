## Problem 8

**Question:** Let $A$ and $B$ be $n\times n$ matrices with $\det A = 3$ and $\det B = -5$. Compute $\det(AB)$ and $\det(BA)$, and explain why they are equal even though $AB$ and $BA$ are generally different matrices. Then compute $\det(A^{-1}B)$.

### Solution

**Computing $\det(AB)$ and $\det(BA)$.**

$$
\det(AB) = \det A\cdot\det B = 3\cdot(-5) = -15
$$

$$
\det(BA) = \det B\cdot\det A = (-5)\cdot 3 = -15
$$

**Why they are equal.** In general $AB \neq BA$, but the determinant is multiplicative, $\det(AB) = \det A\cdot\det B$, and the determinants are just real numbers, so their product does not depend on the order:

$$
\det A\cdot\det B = \det B\cdot\det A
$$

Hence $\det(AB) = \det(BA)$ even when the matrices $AB$ and $BA$ are different.

**Computing $\det(A^{-1}B)$.** Since $\det A = 3 \neq 0$, the matrix $A$ is invertible, so $A^{-1}$ exists and

$$
\det(A^{-1}) = \frac{1}{\det A} = \frac{1}{3}
$$

Therefore

$$
\det(A^{-1}B) = \det(A^{-1})\cdot\det B = \frac{1}{3}\cdot(-5) = -\frac{5}{3}
$$

### Conclusion

$$
\det(AB) = -15, \qquad \det(BA) = -15, \qquad \det(A^{-1}B) = -\frac{5}{3}
$$
