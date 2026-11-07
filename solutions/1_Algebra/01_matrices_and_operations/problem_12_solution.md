# Exercise 12. Formula for a Matrix Power

## Exercise Statement

Given:

\[
A=
\begin{pmatrix}
1&1\\
0&1
\end{pmatrix}
\]

Compute \(A^2,A^3,A^4\), and use them to formulate a conjecture for \(A^n\).

Then prove the formula using mathematical induction. Assume the formula is true for n, multiply by A, and explain why you obtain the formula for n + 1.

## Solution

### Part 1. Calculate A²

\[
A^2=
\begin{pmatrix}
1&1\\
0&1
\end{pmatrix}
\begin{pmatrix}
1&1\\
0&1
\end{pmatrix}
\]

\[
\boxed{
A^2=
\begin{pmatrix}
1&2\\
0&1
\end{pmatrix}
}
\]

### Part 2. Calculate A³

\[
A^3=A^2A
\]

\[
=
\begin{pmatrix}
1&2\\
0&1
\end{pmatrix}
\begin{pmatrix}
1&1\\
0&1
\end{pmatrix}
\]

\[
\boxed{
A^3=
\begin{pmatrix}
1&3\\
0&1
\end{pmatrix}
}
\]

### Part 3. Calculate A⁴

\[
A^4=A^3A
\]

\[
=
\begin{pmatrix}
1&3\\
0&1
\end{pmatrix}
\begin{pmatrix}
1&1\\
0&1
\end{pmatrix}
\]

\[
\boxed{
A^4=
\begin{pmatrix}
1&4\\
0&1
\end{pmatrix}
}
\]

### Part 4. Formulate the Conjecture

The upper-right entry increases by one with each multiplication.

The general formula is:

\[
\boxed{
A^n=
\begin{pmatrix}
1&n\\
0&1
\end{pmatrix}
}
\]

### Part 5. Proof by Mathematical Induction

**Base Case:**

For n = 1:

\[
A^1=
\begin{pmatrix}
1&1\\
0&1
\end{pmatrix}
\]

The formula is true.

**Inductive Hypothesis:**

Assume that the formula is true for n:

\[
A^n=
\begin{pmatrix}
1&n\\
0&1
\end{pmatrix}
\]

**Inductive Step:**

Multiply both sides by A:

\[
A^{n+1}=A^nA
\]

\[
=
\begin{pmatrix}
1&n\\
0&1
\end{pmatrix}
\begin{pmatrix}
1&1\\
0&1
\end{pmatrix}
\]

\[
=
\begin{pmatrix}
1&n+1\\
0&1
\end{pmatrix}
\]

This is exactly the proposed formula for n + 1.

Therefore, by mathematical induction:

\[
\boxed{
A^n=
\begin{pmatrix}
1&n\\
0&1
\end{pmatrix}
}
\]

for every positive integer n.
