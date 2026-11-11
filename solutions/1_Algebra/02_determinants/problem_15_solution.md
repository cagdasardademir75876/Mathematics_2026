
### Exercise 15. Combining Determinant Properties

**Problem**

Let $A$ and $B$ be invertible $2\times2$ matrices with

$$
\det(A)=-2,\qquad \det(B)=3.
$$

Without finding the entries of the matrices, compute

$$
\det\left(B^{-1}A^TB\right).
$$

State the determinant properties you use in order and explain why the factors involving $B$ eventually cancel.

> **Why this exercise:** tests the transfer of several known properties into one short problem instead of checking a single property again with numbers.

**Solution**

**1. Given Information**

We are given that $A$ and $B$ are invertible $2\times2$ matrices and

$$
\det(A)=-2,\qquad \det(B)=3.
$$

We need to calculate

$$
\det\left(B^{-1}A^TB\right).
$$

We can solve this problem using determinant properties without finding the individual matrix entries.

**2. Applying the Product Property**

The determinant of a product of square matrices is equal to the product of their determinants.

Therefore,

$$
\det(B^{-1}A^TB)
=
\det(B^{-1})\det(A^T)\det(B)
$$

**3. Applying the Inverse and Transpose Properties**

The determinant of an inverse matrix is the reciprocal of the original determinant:

$$
\det(B^{-1})=\frac{1}{\det(B)}
$$

The determinant of a transpose is equal to the determinant of the original matrix:

$$
\det(A^T)=\det(A)
$$

Substituting these properties gives

$$
\det(B^{-1}A^TB)
=
\frac{1}{\det(B)}\det(A)\det(B)
$$

**4. Simplifying the Expression**

Since $\det(B)=3$ and $\det(A)=-2$, we obtain

$$
\det(B^{-1}A^TB)
=
\frac{1}{3}\cdot(-2)\cdot3
$$

The factors involving $B$ cancel because

$$
\frac{1}{\det(B)}\cdot\det(B)=1
$$

Therefore,

$$
\det(B^{-1}A^TB)=-2
$$

**5. Explanation of the Cancellation**

The matrix $B$ is invertible, so its determinant is nonzero.

The inverse matrix $B^{-1}$ has a determinant equal to the reciprocal of $\det(B)$.

When we calculate the determinant of $B^{-1}A^TB$, the determinant of $B^{-1}$ multiplies the determinant of $B$.

These two factors cancel each other:

$$
\det(B^{-1})\det(B)=1
$$

The transpose does not change the determinant of $A$.

As a result, the final determinant depends only on $\det(A)$.

**Final Answer**

$$
\det(B^{-1}A^TB)=-2
$$

The factors involving $B$ cancel because the determinant of an inverse is the reciprocal of the determinant of the original matrix. The transpose preserves the determinant, so the final result is equal to $\det(A)$.
