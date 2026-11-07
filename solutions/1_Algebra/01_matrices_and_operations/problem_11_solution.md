# Exercise 11. When Do Matrices Commute?

## Exercise Statement

Given:

\[
A=
\begin{pmatrix}
1&1\\
0&1
\end{pmatrix},
\qquad
B=
\begin{pmatrix}
a&b\\
c&d
\end{pmatrix}
\]

Find the conditions on \(a,b,c,d\) under which:

\[
AB=BA
\]

Describe the general form of all such matrices B.

## Solution

### Part 1. Calculate AB

\[
AB=
\begin{pmatrix}
1&1\\
0&1
\end{pmatrix}
\begin{pmatrix}
a&b\\
c&d
\end{pmatrix}
\]

\[
AB=
\begin{pmatrix}
a+c&b+d\\
c&d
\end{pmatrix}
\]

### Part 2. Calculate BA

\[
BA=
\begin{pmatrix}
a&b\\
c&d
\end{pmatrix}
\begin{pmatrix}
1&1\\
0&1
\end{pmatrix}
\]

\[
BA=
\begin{pmatrix}
a&a+b\\
c&c+d
\end{pmatrix}
\]

### Part 3. Find the Conditions

For AB = BA, corresponding entries must be equal.

\[
a+c=a
\]

\[
b+d=a+b
\]

\[
c=c
\]

\[
d=c+d
\]

Simplifying:

\[
c=0
\]

\[
d=a
\]

The upper-right entry b is unrestricted.

### Final Answer

The general form of B is:

\[
\boxed{
B=
\begin{pmatrix}
a&b\\
0&a
\end{pmatrix}
}
\]

where a and b can be any real numbers.

### Explanation

Matrices A and B commute only when B has equal diagonal entries and a zero in its lower-left position. The upper-right entry can be any real number.
