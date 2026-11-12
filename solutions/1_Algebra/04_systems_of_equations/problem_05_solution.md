# Exercise 5. Row Echelon Form and Number of Solutions

## Solution

$$
\begin{pmatrix}
1 & 2 & -1 & \mid & 3 \\
0 & 1 & 2 & \mid & 1 \\
0 & 0 & 0 & \mid & 0 \\
\end{pmatrix}
$$

The last row is $0=0$, so the system is consistent. There are $3$ unknowns and $2$ pivots (in columns 1 and 2), so there are $3-2=1$ free variable, namely $z$. Hence there are infinitely many solutions.

Put $z=t$. Row 2 gives $y=1-2t$. Row 1 gives

$$
x=3-2y+z=3-2(1-2t)+t=1+5t
$$

$$
(x,y,z)=(1+5t,\;1-2t,\;t),\qquad t\in\mathbb{R}
$$

Check:

$$
(1+5t)+2(1-2t)-t=3,
$$

$$
(1-2t)+2t=1
$$
