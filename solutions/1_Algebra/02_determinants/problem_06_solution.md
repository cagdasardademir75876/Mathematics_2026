
### Exercise 6. Parameter and Invertibility

**Problem**

For

$$
A(t)=
\begin{pmatrix}
t & 1 \\
2 & t \\
\end{pmatrix}
$$

find all values of $t$ for which the matrix is not invertible. Explain how your answer is related to the determinant being zero.

> **Why this exercise:** shows how the determinant can be used to study a family of matrices depending on a parameter.

**Solution**

A square matrix is not invertible if and only if its determinant is equal to zero.

First, calculate the determinant of the given matrix:

$$
\det(A(t)) = t \cdot t - 1 \cdot 2
$$

Simplifying,

$$
\det(A(t)) = t^2 - 2
$$

To find the values of $t$ for which the matrix is not invertible, set the determinant equal to zero:

$$
t^2 - 2 = 0
$$

Move the constant term to the right side:

$$
t^2 = 2
$$

Taking the square root of both sides gives

$$
t = \sqrt{2}
\qquad \mathrm{or} \qquad
t = -\sqrt{2}
$$

**Final Answer**

The matrix is not invertible when

$$
t \in \{-\sqrt{2},\sqrt{2}\}
$$

For every other real value of $t$, the determinant is nonzero, so the matrix is invertible.

**Explanation**

The determinant determines whether a square matrix is invertible. A square matrix has an inverse if and only if its determinant is nonzero.

In this example, when $t = \sqrt{2}$ or $t = -\sqrt{2}$, the determinant becomes zero. Therefore, the matrix has no inverse for these two values.

This demonstrates how the determinant can be used to determine the invertibility of a matrix whose entries depend on a parameter.
