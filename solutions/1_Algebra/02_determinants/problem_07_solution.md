## Problem 7

**Question:** Let $A$ be a $3\times 3$ matrix with $\det A = -4$. Compute each of the following determinants and state the property you use:

$$
\det(2A), \qquad \det(A^{T}), \qquad \det(A^{2}), \qquad \det(-A)
$$

### Solution

**1. $\det(2A)$.** Multiplying an $n\times n$ matrix by a scalar $c$ gives $\det(cA) = c^{n}\det A$. Here $n = 3$:

$$
\det(2A) = 2^{3}\det A = 8\cdot(-4) = -32
$$

**2. $\det(A^{T})$.** A matrix and its transpose have the same determinant:

$$
\det(A^{T}) = \det A = -4
$$

**3. $\det(A^{2})$.** The determinant is multiplicative: $\det(AB) = \det A\cdot\det B$. With $B = A$:

$$
\det(A^{2}) = (\det A)^{2} = (-4)^{2} = 16
$$

**4. $\det(-A)$.** This is the scalar rule with $c = -1$ and $n = 3$:

$$
\det(-A) = (-1)^{3}\det A = -1\cdot(-4) = 4
$$

### Conclusion

$$
\det(2A) = -32, \qquad \det(A^{T}) = -4, \qquad \det(A^{2}) = 16, \qquad \det(-A) = 4
$$
