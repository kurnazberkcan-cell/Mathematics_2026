# Exercise 3. When Can Matrices Be Multiplied?

## Exercise Statement

The matrix dimensions are:

- \(A_{2\times3}\)
- \(B_{3\times4}\)
- \(C_{4\times2}\)
- \(D_{2\times2}\)

For the following products:

\[
AB,\ BA,\ BC,\ CB,\ AC,\ CA,\ AD,\ DA
\]

Determine whether each product is defined. If it is, state the dimensions of the resulting matrix. Justify each decision using the dimension compatibility condition.

## Solution

Two matrices can be multiplied if the number of columns of the first matrix equals the number of rows of the second matrix.

The resulting matrix has the number of rows of the first matrix and the number of columns of the second matrix.

### Calculations

1. **AB**

   \[
   (2\times3)(3\times4)=2\times4
   \]

   Defined.

2. **BA**

   \[
   (3\times4)(2\times3)
   \]

   Not defined because \(4\neq2\).

3. **BC**

   \[
   (3\times4)(4\times2)=3\times2
   \]

   Defined.

4. **CB**

   \[
   (4\times2)(3\times4)
   \]

   Not defined because \(2\neq3\).

5. **AC**

   \[
   (2\times3)(4\times2)
   \]

   Not defined because \(3\neq4\).

6. **CA**

   \[
   (4\times2)(2\times3)=4\times3
   \]

   Defined.

7. **AD**

   \[
   (2\times3)(2\times2)
   \]

   Not defined because \(3\neq2\).

8. **DA**

   \[
   (2\times2)(2\times3)=2\times3
   \]

   Defined.

### Final Results

| Product | Defined? | Result Size |
|---|---|---|
| AB | Yes | \(2\times4\) |
| BA | No | — |
| BC | Yes | \(3\times2\) |
| CB | No | — |
| AC | No | — |
| CA | Yes | \(4\times3\) |
| AD | No | — |
| DA | Yes | \(2\times3\) |

### Explanation

Matrix multiplication depends on the compatibility of the inner dimensions. The outer dimensions determine the size of the resulting matrix.
