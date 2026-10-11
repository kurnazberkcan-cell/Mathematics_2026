## Results

```math
R(\alpha)R(\beta) =
\begin{pmatrix}
\cos\alpha\cos\beta - \sin\alpha\sin\beta & -\cos\alpha\sin\beta - \sin\alpha\cos\beta \\
\sin\alpha\cos\beta + \cos\alpha\sin\beta & -\sin\alpha\sin\beta + \cos\alpha\cos\beta
\end{pmatrix}
```

### Using the angle-sum formulas

```math
\cos(\alpha+\beta) = \cos\alpha\cos\beta - \sin\alpha\sin\beta
```

```math
\sin(\alpha+\beta) = \sin\alpha\cos\beta + \cos\alpha\sin\beta
```

Substituting these into the product:

```math
R(\alpha)R(\beta) =
\begin{pmatrix}
\cos(\alpha+\beta) & -\sin(\alpha+\beta) \\
\sin(\alpha+\beta) & \cos(\alpha+\beta)
\end{pmatrix}
= R(\alpha+\beta)
```

### Geometric explanation

$R(\beta)$ rotates a vector counterclockwise by $\beta$, and then $R(\alpha)$ rotates the result counterclockwise by a further $\alpha$. The total effect is a single counterclockwise rotation by $\alpha + \beta$, which is exactly $R(\alpha+\beta)$. Since the order of two rotations about the origin does not change the total angle, we also get $R(\alpha)R(\beta) = R(\beta)R(\alpha)$.
