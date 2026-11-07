# Exercise 13. A Recurrence Written in Matrix Form

## Exercise Statement

Given:

\[
F=
\begin{pmatrix}
1&1\\
1&0
\end{pmatrix}
\]

Answer the following questions:

1. Compute \(F^2,F^3,F^4,F^5\).
2. Compare the numbers obtained with the Fibonacci sequence:

\[
0,1,1,2,3,5,8,\ldots
\]

Describe the relationship you observe.
3. Compute:

\[
F
\begin{pmatrix}
a\\
b
\end{pmatrix}
\]

Explain how this multiplication performs one recurrence step: it creates the sum of two consecutive terms and keeps one of them for the next step.

## Solution

### Part 1. Calculate the Matrix Powers

First:

\[
F^2=
\begin{pmatrix}
1&1\\
1&0
\end{pmatrix}
\begin{pmatrix}
1&1\\
1&0
\end{pmatrix}
\]

\[
\boxed{
F^2=
\begin{pmatrix}
2&1\\
1&1
\end{pmatrix}
}
\]

Next:

\[
F^3=F^2F
\]

\[
\boxed{
F^3=
\begin{pmatrix}
3&2\\
2&1
\end{pmatrix}
}
\]

Next:

\[
F^4=F^3F
\]

\[
\boxed{
F^4=
\begin{pmatrix}
5&3\\
3&2
\end{pmatrix}
}
\]

Finally:

\[
F^5=F^4F
\]

\[
\boxed{
F^5=
\begin{pmatrix}
8&5\\
5&3
\end{pmatrix}
}
\]

### Part 2. Compare with the Fibonacci Sequence

The Fibonacci sequence is:

\[
0,1,1,2,3,5,8,\ldots
\]

The matrix powers contain consecutive Fibonacci numbers:

\[
F^2=
\begin{pmatrix}
2&1\\
1&1
\end{pmatrix}
\]

\[
F^3=
\begin{pmatrix}
3&2\\
2&1
\end{pmatrix}
\]

\[
F^4=
\begin{pmatrix}
5&3\\
3&2
\end{pmatrix}
\]

\[
F^5=
\begin{pmatrix}
8&5\\
5&3
\end{pmatrix}
\]

The general relationship is:

\[
\boxed{
F^n=
\begin{pmatrix}
F_{n+1}&F_n\\
F_n&F_{n-1}
\end{pmatrix}
}
\]

where \(F_0=0\) and \(F_1=1\).

### Part 3. Matrix Multiplication as a Recurrence Step

\[
F
\begin{pmatrix}
a\\
b
\end{pmatrix}
=
\begin{pmatrix}
1&1\\
1&0
\end{pmatrix}
\begin{pmatrix}
a\\
b
\end{pmatrix}
\]

\[
=
\begin{pmatrix}
a+b\\
a
\end{pmatrix}
\]

Therefore:

\[
\boxed{
F
\begin{pmatrix}
a\\
b
\end{pmatrix}
=
\begin{pmatrix}
a+b\\
a
\end{pmatrix}
}
\]

### Explanation

The multiplication creates a new term by adding the two previous consecutive terms. It also keeps the previous first term as the second entry.

This is exactly the Fibonacci recurrence rule.
