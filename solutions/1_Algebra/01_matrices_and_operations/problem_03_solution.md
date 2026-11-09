# Problem 3. When Can Matrices Be Multiplied?

## Question

The matrix sizes are $A_{2\times3}$, $B_{3\times4}$, $C_{4\times2}$, $D_{2\times2}$.

For each of the products $AB$, $BA$, $BC$, $CB$, $AC$, $CA$, $AD$, $DA$, determine whether it is defined. If it is, state the size of the result. Justify each decision using the dimension compatibility condition.

## Solution

The product $XY$ of an $m\times n$ matrix $X$ and a $p\times q$ matrix $Y$ is defined exactly when $n=p$, that is, when the number of columns of $X$ equals the number of rows of $Y$. The result then has size $m\times q$.

- $AB$: $A_{2\times3}$, $B_{3\times4}$. Here $3=3$, so the product is defined and has size $2\times4$.
- $BA$: $B_{3\times4}$, $A_{2\times3}$. Here $4\neq2$, so the product is not defined.
- $BC$: $B_{3\times4}$, $C_{4\times2}$. Here $4=4$, so the product is defined and has size $3\times2$.
- $CB$: $C_{4\times2}$, $B_{3\times4}$. Here $2\neq3$, so the product is not defined.
- $AC$: $A_{2\times3}$, $C_{4\times2}$. Here $3\neq4$, so the product is not defined.
- $CA$: $C_{4\times2}$, $A_{2\times3}$. Here $2=2$, so the product is defined and has size $4\times3$.
- $AD$: $A_{2\times3}$, $D_{2\times2}$. Here $3\neq2$, so the product is not defined.
- $DA$: $D_{2\times2}$, $A_{2\times3}$. Here $2=2$, so the product is defined and has size $2\times3$.

Conclusion: the defined products are $AB$, $BC$, $CA$, $DA$.
