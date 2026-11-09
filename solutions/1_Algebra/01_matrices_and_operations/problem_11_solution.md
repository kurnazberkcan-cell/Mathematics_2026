# Problem 11. When Do Matrices Commute?

## Question

Given

$$
A=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix},
$$

$$
B=
\begin{pmatrix}
a & b \\
c & d \\
\end{pmatrix}.
$$

Find the conditions on $a,b,c,d$ under which $AB=BA$. Describe the general form of all such matrices $B$.

## Solution

Both products are computed:

$$
AB=
\begin{pmatrix}
a+c & b+d \\
c & d \\
\end{pmatrix},
$$

$$
BA=
\begin{pmatrix}
a & a+b \\
c & c+d \\
\end{pmatrix}.
$$

Two matrices are equal exactly when all four entries are equal:

$$
\begin{aligned}
a+c&=a, \\
b+d&=a+b, \\
c&=c, \\
d&=c+d. \\
\end{aligned}
$$

The first equation gives $c=0$. The second gives $d=a$. The third is always true. The fourth gives $c=0$ again, so it adds no new condition.

Hence $AB=BA$ if and only if $c=0$ and $d=a$, while $a$ and $b$ are arbitrary. The general form is

$$
B=
\begin{pmatrix}
a & b \\
0 & a \\
\end{pmatrix}.
$$

Equivalently, $B=aI+bN$, where $N$ has a single entry $1$ in the upper-right corner.

Verification for this form:

$$
AB=
\begin{pmatrix}
a & a+b \\
0 & a \\
\end{pmatrix}
$$

$$
BA=
\begin{pmatrix}
a & a+b \\
0 & a \\
\end{pmatrix}
$$

Both products are equal, as required.
