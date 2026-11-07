# Exercise 14. Rotation Matrices

## Exercise Statement

The matrix for a rotation through an angle \(\theta\) is:

\[
R(\theta)=
\begin{pmatrix}
\cos\theta&-\sin\theta\\
\sin\theta&\cos\theta
\end{pmatrix}
\]

Compute \(R(\alpha)R(\beta)\) and, using the angle-sum formulas for sine and cosine, show that:

\[
R(\alpha)R(\beta)=R(\alpha+\beta)
\]

Explain the result geometrically.

## Solution

### Part 1. Write the Rotation Matrices

\[
R(\alpha)=
\begin{pmatrix}
\cos\alpha&-\sin\alpha\\
\sin\alpha&\cos\alpha
\end{pmatrix}
\]

\[
R(\beta)=
\begin{pmatrix}
\cos\beta&-\sin\beta\\
\sin\beta&\cos\beta
\end{pmatrix}
\]

### Part 2. Multiply the Matrices

\[
R(\alpha)R(\beta)=
\begin{pmatrix}
\cos\alpha&-\sin\alpha\\
\sin\alpha&\cos\alpha
\end{pmatrix}
\begin{pmatrix}
\cos\beta&-\sin\beta\\
\sin\beta&\cos\beta
\end{pmatrix}
\]

Multiplying the entries:

\[
=
\begin{pmatrix}
\cos\alpha\cos\beta-\sin\alpha\sin\beta&
-\cos\alpha\sin\beta-\sin\alpha\cos\beta\\
\sin\alpha\cos\beta+\cos\alpha\sin\beta&
-\sin\alpha\sin\beta+\cos\alpha\cos\beta
\end{pmatrix}
\]

### Part 3. Apply the Angle-Sum Formulas

Recall:

\[
\cos(\alpha+\beta)
=
\cos\alpha\cos\beta-\sin\alpha\sin\beta
\]

\[
\sin(\alpha+\beta)
=
\sin\alpha\cos\beta+\cos\alpha\sin\beta
\]

Substituting these identities:

\[
R(\alpha)R(\beta)=
\begin{pmatrix}
\cos(\alpha+\beta)&-\sin(\alpha+\beta)\\
\sin(\alpha+\beta)&\cos(\alpha+\beta)
\end{pmatrix}
\]

Therefore:

\[
\boxed{
R(\alpha)R(\beta)=R(\alpha+\beta)
}
\]

### Geometric Explanation

Applying two rotations consecutively is equivalent to performing one rotation through the sum of the two angles.

For example, rotating a vector by 30 degrees and then by 60 degrees is equivalent to rotating it by 90 degrees.
