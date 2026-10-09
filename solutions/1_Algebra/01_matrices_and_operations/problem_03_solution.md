## Exercise 3. When Can Matrices Be Multiplied?

The matrix sizes are

$$
A_{2\times3},\qquad B_{3\times4},\qquad C_{4\times2},\qquad D_{2\times2}.
$$

For the products

$$
AB,\ BA,\ BC,\ CB,\ AC,\ CA,\ AD,\ DA
$$

determine whether they are defined. If so, state the size of the result. Justify each decision using the dimension compatibility condition.

> **Why this exercise:** forces an understanding of dimension compatibility before carrying out any calculation.

---

### Solution

The product $XY$ is defined if and only if the number of columns of $X$ equals the number of rows of $Y$. If $X$ is $m\times n$ and $Y$ is $n\times p$, then $XY$ is $m\times p$.

| Product | Sizes | Inner dimensions | Defined? | Result size |
|---------|-------|------------------|----------|-------------|
| $AB$ | $2\times3$ and $3\times4$ | $3=3$ | Yes | $2\times4$ |
| $BA$ | $3\times4$ and $2\times3$ | $4\neq2$ | No | — |
| $BC$ | $3\times4$ and $4\times2$ | $4=4$ | Yes | $3\times2$ |
| $CB$ | $4\times2$ and $3\times4$ | $2\neq3$ | No | — |
| $AC$ | $2\times3$ and $4\times2$ | $3\neq4$ | No | — |
| $CA$ | $4\times2$ and $2\times3$ | $2=2$ | Yes | $4\times3$ |
| $AD$ | $2\times3$ and $2\times2$ | $3\neq2$ | No | — |
| $DA$ | $2\times2$ and $2\times3$ | $2=2$ | Yes | $2\times3$ |

Defined products: $AB$, $BC$, $CA$, $DA$.

---
