# Exercise 7. Identity Matrix, Zero Matrix, and Powers

## Exercise Statement

Given:

\[
A=
\begin{pmatrix}
2&1\\
0&2
\end{pmatrix}
\]

Compute:

\[
AI,\qquad IA,\qquad A+0,\qquad A^2,\qquad A^3
\]

Explain the roles of the identity matrix \(I\) and the zero matrix \(0\), and describe the pattern observed in successive powers of \(A\).

## Solution

### Part 1. Identity Matrix

The identity matrix is:

\[
I=
\begin{pmatrix}
1&0\\
0&1
\end{pmatrix}
\]

Multiplying A by I:

\[
AI=
\begin{pmatrix}
2&1\\
0&2
\end{pmatrix}
\begin{pmatrix}
1&0\\
0&1
\end{pmatrix}
\]

\[
\boxed{
AI=
\begin{pmatrix}
2&1\\
0&2
\end{pmatrix}
}
\]

Similarly:

\[
\boxed{
IA=
\begin{pmatrix}
2&1\\
0&2
\end{pmatrix}
}
\]

### Part 2. Zero Matrix

\[
0=
\begin{pmatrix}
0&0\\
0&0
\end{pmatrix}
\]

\[
A+0=
\begin{pmatrix}
2&1\\
0&2
\end{pmatrix}
+
\begin{pmatrix}
0&0\\
0&0
\end{pmatrix}
\]

\[
\boxed{
A+0=
\begin{pmatrix}
2&1\\
0&2
\end{pmatrix}
}
\]

### Part 3. Calculate A²

\[
A^2=A\cdot A
\]

\[
=
\begin{pmatrix}
2&1\\
0&2
\end{pmatrix}
\begin{pmatrix}
2&1\\
0&2
\end{pmatrix}
\]

\[
\boxed{
A^2=
\begin{pmatrix}
4&4\\
0&4
\end{pmatrix}
}
\]

### Part 4. Calculate A³

\[
A^3=A^2A
\]

\[
=
\begin{pmatrix}
4&4\\
0&4
\end{pmatrix}
\begin{pmatrix}
2&1\\
0&2
\end{pmatrix}
\]

\[
\boxed{
A^3=
\begin{pmatrix}
8&12\\
0&8
\end{pmatrix}
}
\]

### Part 5. Observe the Pattern

\[
A=
\begin{pmatrix}
2&1\\
0&2
\end{pmatrix}
\]

\[
A^2=
\begin{pmatrix}
4&4\\
0&4
\end{pmatrix}
\]

\[
A^3=
\begin{pmatrix}
8&12\\
0&8
\end{pmatrix}
\]

The general pattern is:

\[
\boxed{
A^n=
\begin{pmatrix}
2^n&n2^{n-1}\\
0&2^n
\end{pmatrix}
}
\]

### Explanation

The identity matrix does not change a matrix when multiplied by it. The zero matrix does not change a matrix when added to it.

The diagonal entries follow powers of 2, while the upper-right entry follows the pattern \(1,4,12,\ldots\).
