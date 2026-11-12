# Exercise 10. A Polynomial Through Three Points

## Solution

Substituting the points into $p(x)=ax^2+bx+c$:

$$
\begin{cases}
a+b+c=3, \\
4a+2b+c=9, \\
c=1.
\end{cases}
$$

The first equation comes from $(1,3)$, the second from $(2,9)$, and the third from $(0,1)$. Augmented matrix in the unknowns $(a,b,c)$:

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 3 \\
4 & 2 & 1 & \mid & 9 \\
0 & 0 & 1 & \mid & 1 \\
\end{pmatrix}
$$

Apply $R_2\to R_2-4R_1$:

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 3 \\
0 & -2 & -3 & \mid & -3 \\
0 & 0 & 1 & \mid & 1 \\
\end{pmatrix}
$$

Back substitution: $c=1$, then $-2b-3=-3$ gives $b=0$, then $a=3-0-1=2$.

$$
p(x)=2x^2+1
$$

Check:

$$
p(0)=1,
$$

$$
p(1)=3,
$$

$$
p(2)=9
$$
