# Problem 14. Rotation Matrices

## Question

The matrix for a rotation through an angle $\theta$ is

$$
R(\theta)=
\begin{pmatrix}
\cos\theta & -\sin\theta \\
\sin\theta & \cos\theta \\
\end{pmatrix}.
$$

Compute $R(\alpha)R(\beta)$ and, using the angle-sum formulas for sine and cosine, show that $R(\alpha)R(\beta)=R(\alpha+\beta)$. Explain the result geometrically.

## Solution

$$
R(\alpha)R(\beta)=
\begin{pmatrix}
\cos\alpha\cos\beta-\sin\alpha\sin\beta & -\cos\alpha\sin\beta-\sin\alpha\cos\beta \\
\sin\alpha\cos\beta+\cos\alpha\sin\beta & -\sin\alpha\sin\beta+\cos\alpha\cos\beta \\
\end{pmatrix}.
$$

The angle-sum formulas are

$$
\cos(\alpha+\beta)=\cos\alpha\cos\beta-\sin\alpha\sin\beta,
$$

$$
\sin(\alpha+\beta)=\sin\alpha\cos\beta+\cos\alpha\sin\beta.
$$

The upper-left and lower-right entries equal $\cos(\alpha+\beta)$. The lower-left entry equals $\sin(\alpha+\beta)$. The upper-right entry is $-(\cos\alpha\sin\beta+\sin\alpha\cos\beta)=-\sin(\alpha+\beta)$. Therefore

$$
R(\alpha)R(\beta)=
\begin{pmatrix}
\cos(\alpha+\beta) & -\sin(\alpha+\beta) \\
\sin(\alpha+\beta) & \cos(\alpha+\beta) \\
\end{pmatrix}
=R(\alpha+\beta).
$$

Geometric explanation: $R(\alpha)R(\beta)$ means first rotating by $\beta$ and then by $\alpha$. Two rotations about the origin in succession give a single rotation by the sum of the angles, so the matrix of the composition is $R(\alpha+\beta)$. Since $\alpha+\beta=\beta+\alpha$, it also follows that $R(\alpha)R(\beta)=R(\beta)R(\alpha)$: rotations in the plane commute.
