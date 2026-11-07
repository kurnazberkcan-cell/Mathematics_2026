# Exercise 15. Associativity of Multiplication and Different Calculation Paths

## Exercise Statement

Given:

\[
A=
\begin{pmatrix}
1&2&0\\
0&1&1
\end{pmatrix}
\]

\[
B=
\begin{pmatrix}
1&0\\
2&1\\
-1&3
\end{pmatrix}
\]

\[
C=
\begin{pmatrix}
2&1\\
0&-1
\end{pmatrix}
\]

Answer the following questions:

1. Compute \((AB)C\).
2. Compute \(A(BC)\).
3. Compare the results and the number of intermediate operations.
4. Explain what associativity of matrix multiplication means in this example.

## Solution

### Part 1. Calculate (AB)C

First calculate AB:

\[
AB=
\begin{pmatrix}
1&2&0\\
0&1&1
\end{pmatrix}
\begin{pmatrix}
1&0\\
2&1\\
-1&3
\end{pmatrix}
\]

\[
=
\begin{pmatrix}
1+4+0&0+2+0\\
0+2-1&0+1+3
\end{pmatrix}
\]

\[
AB=
\begin{pmatrix}
5&2\\
1&4
\end{pmatrix}
\]

Now multiply by C:

\[
(AB)C=
\begin{pmatrix}
5&2\\
1&4
\end{pmatrix}
\begin{pmatrix}
2&1\\
0&-1
\end{pmatrix}
\]

\[
=
\begin{pmatrix}
10&5-2\\
2&1-4
\end{pmatrix}
\]

\[
\boxed{
(AB)C=
\begin{pmatrix}
10&3\\
2&-3
\end{pmatrix}
}
\]

### Part 2. Calculate A(BC)

First calculate BC:

\[
BC=
\begin{pmatrix}
1&0\\
2&1\\
-1&3
\end{pmatrix}
\begin{pmatrix}
2&1\\
0&-1
\end{pmatrix}
\]

\[
BC=
\begin{pmatrix}
2&1\\
4&1\\
-2&-4
\end{pmatrix}
\]

Now multiply by A:

\[
A(BC)=
\begin{pmatrix}
1&2&0\\
0&1&1
\end{pmatrix}
\begin{pmatrix}
2&1\\
4&1\\
-2&-4
\end{pmatrix}
\]

\[
=
\begin{pmatrix}
2+8+0&1+2+0\\
0+4-2&0+1-4
\end{pmatrix}
\]

\[
\boxed{
A(BC)=
\begin{pmatrix}
10&3\\
2&-3
\end{pmatrix}
}
\]

### Part 3. Compare the Results

\[
(AB)C=
\begin{pmatrix}
10&3\\
2&-3
\end{pmatrix}
\]

\[
A(BC)=
\begin{pmatrix}
10&3\\
2&-3
\end{pmatrix}
\]

Therefore:

\[
\boxed{(AB)C=A(BC)}
\]

Both calculation paths produce exactly the same matrix.

### Part 4. Compare the Number of Scalar Operations

For a standard \(m\times n\) multiplied by \(n\times p\) matrix product, the number of scalar multiplications is \(mnp\).

**Path 1: Calculate (AB)C**

- AB: \(2\times3\times2=12\) scalar multiplications.
- (AB)C: \(2\times2\times2=8\) scalar multiplications.
- Total: 20 scalar multiplications.

**Path 2: Calculate A(BC)**

- BC: \(3\times2\times2=12\) scalar multiplications.
- A(BC): \(2\times3\times2=12\) scalar multiplications.
- Total: 24 scalar multiplications.

Path 1 requires 20 scalar multiplications, while Path 2 requires 24.

Therefore, calculating AB first is more efficient for these particular matrix dimensions.

### Explanation

Associativity means that changing the grouping of matrix multiplication does not change the final result:

\[
\boxed{(AB)C=A(BC)}
\]

However, associativity changes grouping, not the order of the actions on a vector.

Acting on a vector, \((AB)C\) applies C first, then B, then A.

The same order applies to \(A(BC)\). Both expressions represent the same composition of transformations.

Associativity can change the number of calculations required, but it does not change the final matrix.
