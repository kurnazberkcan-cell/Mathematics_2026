
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
