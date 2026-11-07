# Exercise 5. Matrix Times Vector

## Exercise Statement

Given:

\[
A=
\begin{pmatrix}
2&-1\\
1&3
\end{pmatrix},
\qquad
x=
\begin{pmatrix}
4\\
2
\end{pmatrix}
\]

Answer the following questions:

1. Compute \(Ax\).
2. Express \(Ax\) as a linear combination of the columns of \(A\), with coefficients coming from the vector \(x\).

## Solution

### Part 1. Calculate Ax

\[
Ax=
\begin{pmatrix}
2&-1\\
1&3
\end{pmatrix}
\begin{pmatrix}
4\\
2
\end{pmatrix}
\]

\[
=
\begin{pmatrix}
2(4)+(-1)(2)\\
1(4)+3(2)
\end{pmatrix}
\]

\[
=
\begin{pmatrix}
8-2\\
4+6
\end{pmatrix}
\]

\[
\boxed{
Ax=
\begin{pmatrix}
6\\
10
\end{pmatrix}
}
\]

### Part 2. Express Ax as a Column Combination

The columns of matrix \(A\) are:

\[
a_1=
\begin{pmatrix}
2\\
1
\end{pmatrix},
\qquad
a_2=
\begin{pmatrix}
-1\\
3
\end{pmatrix}
\]

The entries of vector \(x\) are 4 and 2. These entries become the coefficients of the corresponding columns.

Therefore:

\[
Ax=4a_1+2a_2
\]

\[
=
4\begin{pmatrix}
2\\
1
\end{pmatrix}
+
2\begin{pmatrix}
-1\\
3
\end{pmatrix}
\]

\[
=
\begin{pmatrix}
8\\
4
\end{pmatrix}
+
\begin{pmatrix}
-2\\
6
\end{pmatrix}
\]

\[
\boxed{
Ax=4(2,1)+2(-1,3)=(6,10)
}
\]

### Explanation

The entries of vector \(x\) determine the coefficients used to combine the columns of matrix \(A\). The first entry multiplies the first column, and the second entry multiplies the second column.
