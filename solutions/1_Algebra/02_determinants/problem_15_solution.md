
### Exercise 15. Combining Determinant Properties

**Problem**

Let $A$ and $B$ be invertible $2\times2$ matrices with

$$
\det A=-2,\qquad \det B=3.
$$

Without finding the entries of the matrices, compute

$$
\det(B^{-1}A^TB).
$$

State the determinant properties you use in order and explain why the factors involving $B$ eventually cancel.

> **Why this exercise:** tests the transfer of several known properties into one short problem instead of checking a single property again with numbers.

**Solution**

**1. Given Information**

We are given that $A$ and $B$ are invertible $2\times2$ matrices.

Their determinants are

$$
\det A=-2,\qquad \det B=3.
$$

We need to calculate

$$
\det(B^{-1}A^TB).
$$

**2. Applying the Product Property**

The determinant of a product of square matrices is equal to the product of their determinants.

Therefore,

$$
\det(B^{-1}A^TB)
=
\det(B^{-1})\det(A^T)\det(B)
$$

**3. Applying the Inverse and Transpose Properties**

The determinant of an inverse matrix is the reciprocal of the determinant of the original matrix:

$$
\det(B^{-1})=\frac{1}{\det B}
$$

The determinant of a transpose is equal to the determinant of the original matrix:

$$
\det(A^T)=\det A
$$

Substituting these properties gives

$$
\det(B^{-1}A^TB)
=
\frac{1}{\det B}\det A\det B
$$

**4. Simplifying the Expression**

Since $\det A=-2$ and $\det B=3$, we obtain

$$
\det(B^{-1}A^TB)
=
\frac{1}{3}\cdot(-2)\cdot3
$$

The factors involving $B$ cancel because

$$
\frac{1}{3}\cdot3=1
$$

Therefore,

$$
\det(B^{-1}A^TB)=-2
$$

**5. Explanation of the Cancellation**

The matrix $B$ is invertible, so its determinant is nonzero.

The determinant of $B^{-1}$ is the reciprocal of the determinant of $B$. When these two determinants are multiplied, their product is equal to $1$.

Also, taking the transpose of a matrix does not change its determinant.

Consequently, the factors involving $B$ cancel, and the final result depends only on the determinant of $A$.

**Final Answer**

$$
\det(B^{-1}A^TB)=-2
$$
