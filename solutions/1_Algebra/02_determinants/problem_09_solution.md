# Exercise 9. Area and the Determinant

## Question

Consider the vectors:

\[
u=
\begin{pmatrix}
3\\
1
\end{pmatrix},
\qquad
v=
\begin{pmatrix}
1\\
4
\end{pmatrix}
\]

These vectors span a parallelogram.

1. Compute the area of the parallelogram using a determinant.
2. Reverse the order of the vectors.
3. Explain what changes in the determinant and what remains unchanged in the area.

## Solution

The area of a parallelogram formed by two vectors in \(\mathbb{R}^2\) is the absolute value of the determinant of the matrix formed by placing the vectors as columns.

First, calculate the determinant:

\[
\det
\begin{pmatrix}
3 & 1\\
1 & 4
\end{pmatrix}
=3\cdot4-1\cdot1
\]

\[
=12-1=11
\]

Therefore, the area is:

\[
\boxed{A=|\det(u,v)|=11}
\]

**Reversing the order of the vectors:**

Now place \(v\) before \(u\):

\[
\det
\begin{pmatrix}
1 & 3\\
4 & 1
\end{pmatrix}
=1\cdot1-3\cdot4
\]

\[
=1-12=-11
\]

Therefore:

\[
\boxed{\det(v,u)=-11}
\]

The area is still:

\[
A=|-11|=11
\]

**Conclusion:**

Reversing the order of the vectors changes the sign of the determinant from \(11\) to \(-11\). However, the area remains unchanged because area is calculated using the absolute value of the determinant.

Thus, the parallelogram has the same area, \(11\), regardless of the order of the vectors, while the signed determinant changes sign.
