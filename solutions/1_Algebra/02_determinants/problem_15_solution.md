# Exercise 15. Combining Determinant Properties

## Question

Let $A$ and $B$ be invertible $2 \times 2$ matrices with

$$
\det A=-2,\qquad \det B=3.
$$

Without finding the entries of the matrices, compute

$$
\det\left(B^{-1}A^TB\right).
$$

State the determinant properties used in order and explain why the factors involving $B$ eventually cancel.

## Solution

We use the following determinant properties:

1. The determinant of a product is the product of the determinants.
2. The determinant of an inverse is the reciprocal of the determinant.
3. The determinant of a transpose equals the determinant of the original matrix.

Start by applying the product property:

$$
\det(B^{-1}A^TB)
=
\det(B^{-1})\det(A^T)\det(B)
$$

Using the inverse property:

$$
\det(B^{-1})=\frac{1}{\det B}
$$

Using the transpose property:

$$
\det(A^T)=\det A
$$

Substitute the given values:

$$
\det(B^{-1}A^TB)
=
\frac{1}{3}\cdot(-2)\cdot3
$$

The factors involving $B$ cancel because

$$
\frac{1}{\det B}\cdot\det B=1.
$$

Therefore,

$$
\det(B^{-1}A^TB)=-2.
$$

The final result is

$$
\boxed{\det(B^{-1}A^TB)=-2}
$$
