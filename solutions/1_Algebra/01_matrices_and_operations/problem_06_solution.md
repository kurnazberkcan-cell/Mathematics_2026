# Exercise 6. Transpose

## Exercise Statement

Given:

\[
A=
\begin{pmatrix}
1&2&3\\
4&5&6
\end{pmatrix},
\qquad
B=
\begin{pmatrix}
1&0\\
2&1\\
-1&3
\end{pmatrix}
\]

Answer the following questions:

1. Compute \(A^T\) and \(B^T\).
2. Compute \(AB\).
3. Verify that:

\[
(AB)^T=B^TA^T
\]

## Solution

### Part 1. Calculate the Transposes

A transpose is obtained by changing the rows into columns.

\[
\boxed{
A^T=
\begin{pmatrix}
1&4\\
2&5\\
3&6
\end{pmatrix}
}
\]

\[
\boxed{
B^T=
\begin{pmatrix}
1&2&-1\\
0&1&3
\end{pmatrix}
}
\]

### Part 2. Calculate AB

\[
AB=
\begin{pmatrix}
1&2&3\\
4&5&6
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
1+4-3&0+2+9\\
4+10-6&0+5+18
\end{pmatrix}
\]

\[
\boxed{
AB=
\begin{pmatrix}
2&11\\
8&23
\end{pmatrix}
}
\]

### Part 3. Verify the Transpose Identity

First, transpose the result of AB:

\[
(AB)^T=
\begin{pmatrix}
2&8\\
11&23
\end{pmatrix}
\]

Now calculate \(B^TA^T\):

\[
B^TA^T=
\begin{pmatrix}
1&2&-1\\
0&1&3
\end{pmatrix}
\begin{pmatrix}
1&4\\
2&5\\
3&6
\end{pmatrix}
\]

\[
=
\begin{pmatrix}
1(1)+2(2)-1(3)&1(4)+2(5)-1(6)\\
0(1)+1(2)+3(3)&0(4)+1(5)+3(6)
\end{pmatrix}
\]

\[
=
\begin{pmatrix}
2&8\\
11&23
\end{pmatrix}
\]

Therefore:

\[
\boxed{(AB)^T=B^TA^T}
\]

### Explanation

The transpose of a matrix product reverses the order of the factors. The calculations confirm this identity.
