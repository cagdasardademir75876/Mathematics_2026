
### Exercise 8. Determinant of a Product

**Problem**

Let $A,B$ be square matrices such that $\det A=3$ and $\det B=-5$. Compute $\det(AB)$, $\det(BA)$ and, if it exists, $\det(A^{-1}B)$. Explain why the first two results are equal even though usually $AB\neq BA$.

> **Why this exercise:** organizes how determinants behave with respect to products and inverses.

**Solution**

We are given two square matrices $A$ and $B$ such that

$$
\det(A)=3,\qquad \det(B)=-5.
$$

We will use the determinant properties for matrix products and inverses.

**1. Computing $\det(AB)$**

The determinant of a product of two square matrices is equal to the product of their determinants.

Therefore,

$$
\det(AB)=\det(A)\det(B).
$$

Substituting the given values,

$$
\det(AB)=3\cdot(-5)=-15.
$$

**2. Computing $\det(BA)$**

Using the same determinant property,

$$
\det(BA)=\det(B)\det(A).
$$

Substituting the given values,

$$
\det(BA)=(-5)\cdot3=-15.
$$

**3. Computing $\det(A^{-1}B)$**

First, we check whether the inverse of $A$ exists.

A square matrix is invertible if and only if its determinant is nonzero. Since

$$
\det(A)=3\neq0,
$$

the inverse matrix $A^{-1}$ exists.

The determinant of an inverse matrix is the reciprocal of the determinant of the original matrix:

$$
\det(A^{-1})=\frac{1}{\det(A)}.
$$

Therefore,

$$
\det(A^{-1})=\frac{1}{3}.
$$

Using the determinant property for products,

$$
\det(A^{-1}B)=\det(A^{-1})\det(B).
$$

Substituting the known values,

$$
\det(A^{-1}B)=\frac{1}{3}\cdot(-5).
$$

Thus,

$$
\det(A^{-1}B)=-\frac{5}{3}.
$$

**4. Why Are $\det(AB)$ and $\det(BA)$ Equal?**

Matrix multiplication is generally not commutative. This means that, in general,

$$
AB\neq BA.
$$

However, the determinant of a product satisfies

$$
\det(AB)=\det(A)\det(B).
$$

Similarly,

$$
\det(BA)=\det(B)\det(A).
$$

Since the determinants are real numbers and multiplication of real numbers is commutative,

$$
\det(A)\det(B)=\det(B)\det(A).
$$

Consequently,

$$
\det(AB)=\det(BA).
$$

This shows that two matrices can have different products while those products have the same determinant.

**Final Answers**

$$
\begin{aligned}
\det(AB)&=-15 \\
\det(BA)&=-15 \\
\det(A^{-1}B)&=-\frac{5}{3}
\end{aligned}
$$

The inverse $A^{-1}$ exists because $\det(A)=3\neq0$.

Therefore, all three requested determinants are defined and can be calculated using determinant properties.
