# Exercise 4. Matrix Multiplication and Noncommutativity

## Exercise Statement

Given:

\[
A=
\begin{pmatrix}
1&2\\
0&1
\end{pmatrix},
\qquad
B=
\begin{pmatrix}
2&0\\
3&1
\end{pmatrix}
\]

Compute \(AB\) and \(BA\). Determine whether \(AB=BA\). Use this example to explain what noncommutativity of matrix multiplication means.

## Solution

### 1. Calculate AB

\[
AB=
\begin{pmatrix}
1&2\\
0&1
\end{pmatrix}
\begin{pmatrix}
2&0\\
3&1
\end{pmatrix}
\]

\[
=
\begin{pmatrix}
1(2)+2(3)&1(0)+2(1)\\
0(2)+1(3)&0(0)+1(1)
\end{pmatrix}
\]

\[
\boxed{
AB=
\begin{pmatrix}
8&2\\
3&1
\end{pmatrix}
}
\]

### 2. Calculate BA

\[
BA=
\begin{pmatrix}
2&0\\
3&1
\end{pmatrix}
\begin{pmatrix}
1&2\\
0&1
\end{pmatrix}
\]

\[
=
\begin{pmatrix}
2(1)+0(0)&2(2)+0(1)\\
3(1)+1(0)&3(2)+1(1)
\end{pmatrix}
\]

\[
\boxed{
BA=
\begin{pmatrix}
2&4\\
3&7
\end{pmatrix}
}
\]

### 3. Compare the Results

\[
AB=
\begin{pmatrix}
8&2\\
3&1
\end{pmatrix}
\]

\[
BA=
\begin{pmatrix}
2&4\\
3&7
\end{pmatrix}
\]

Therefore:

\[
\boxed{AB\neq BA}
\]

### Explanation

Matrix multiplication is generally not commutative. This means that changing the order of multiplication can produce a different result.

Unlike ordinary multiplication of numbers, the order of matrices matters.
