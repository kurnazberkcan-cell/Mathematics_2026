# Exercise 10. Columns of a Matrix Product

## Exercise Statement

Given:

\[
A=
\begin{pmatrix}
1&2&0\\
0&1&1
\end{pmatrix},
\qquad
B=
\begin{pmatrix}
1&2\\
-1&0\\
3&1
\end{pmatrix}
\]

Denote the columns of B by \(b_1\) and \(b_2\).

Answer the following questions:

1. Compute \(Ab_1\) and \(Ab_2\).
2. Compute the matrix \(AB\).
3. Compare the results and explain why the columns of \(AB\) are exactly the vectors \(Ab_1\) and \(Ab_2\).

## Solution

### Part 1. Calculate Ab₁ and Ab₂

The columns of B are:

\[
b_1=
\begin{pmatrix}
1\\
-1\\
3
\end{pmatrix},
\qquad
b_2=
\begin{pmatrix}
2\\
0\\
1
\end{pmatrix}
\]

First:

\[
Ab_1=
\begin{pmatrix}
1&2&0\\
0&1&1
\end{pmatrix}
\begin{pmatrix}
1\\
-1\\
3
\end{pmatrix}
\]

\[
=
\begin{pmatrix}
1-2+0\\
0-1+3
\end{pmatrix}
\]

\[
\boxed{
Ab_1=
\begin{pmatrix}
-1\\
2
\end{pmatrix}
}
\]

Next:

\[
Ab_2=
\begin{pmatrix}
1&2&0\\
0&1&1
\end{pmatrix}
\begin{pmatrix}
2\\
0\\
1
\end{pmatrix}
\]

\[
=
\begin{pmatrix}
2+0+0\\
0+0+1
\end{pmatrix}
\]

\[
\boxed{
Ab_2=
\begin{pmatrix}
2\\
1
\end{pmatrix}
}
\]

### Part 2. Calculate AB

\[
AB=
\begin{pmatrix}
1&2&0\\
0&1&1
\end{pmatrix}
\begin{pmatrix}
1&2\\
-1&0\\
3&1
\end{pmatrix}
\]

\[
\boxed{
AB=
\begin{pmatrix}
-1&2\\
2&1
\end{pmatrix}
}
\]

### Part 3. Compare the Results

The first column of AB is:

\[
\begin{pmatrix}
-1\\
2
\end{pmatrix}
=Ab_1
\]

The second column of AB is:

\[
\begin{pmatrix}
2\\
1
\end{pmatrix}
=Ab_2
\]

Therefore:

\[
\boxed{
AB=[Ab_1\quad Ab_2]
}
\]

### Explanation

Matrix multiplication applies A separately to every column of B.

Therefore, the columns of the resulting matrix AB are exactly the products of A with the individual columns of B.
