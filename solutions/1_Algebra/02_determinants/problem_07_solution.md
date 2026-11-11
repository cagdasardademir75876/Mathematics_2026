
### Exercise 7. Using Properties Instead of Recomputing

**Problem**

Suppose that for a $3\times3$ matrix, $\det A=-4$. Compute

$$
\det(2A),\qquad \det(A^T),\qquad \det(A^2),\qquad \det(-A).
$$

Justify each answer using the appropriate property.

> **Why this exercise:** teaches how to use determinant properties instead of repeating a full calculation.

**Solution**

We are given that $A$ is a $3\times3$ matrix and

$$
\det(A)=-4.
$$

We can use the properties of determinants to calculate each expression without expanding the determinants.

**1. Computing $\det(2A)$**

For an $n\times n$ matrix, multiplying the entire matrix by a scalar $k$ multiplies its determinant by $k^n$.

Since $A$ is a $3\times3$ matrix,

$$
\det(2A)=2^3\det(A).
$$

Substituting the given determinant,

$$
\det(2A)=8\cdot(-4)=-32.
$$

**2. Computing $\det(A^T)$**

The determinant of a matrix is equal to the determinant of its transpose.

Therefore,

$$
\det(A^T)=\det(A)=-4.
$$

**3. Computing $\det(A^2)$**

The determinant of a product of two square matrices is equal to the product of their determinants.

Since $A^2=AA$,

$$
\det(A^2)=\det(A)\det(A).
$$

Thus,

$$
\det(A^2)=(-4)^2=16.
$$

**4. Computing $\det(-A)$**

Multiplying a $3\times3$ matrix by $-1$ multiplies its determinant by $(-1)^3$.

Therefore,

$$
\det(-A)=(-1)^3\det(A).
$$

Substituting the given value,

$$
\det(-A)=-1\cdot(-4)=4.
$$

**Final Answers**

$$
\begin{aligned}
\det(2A)&=-32 \\
\det(A^T)&=-4 \\
\det(A^2)&=16 \\
\det(-A)&=4
\end{aligned}
$$

These results demonstrate that determinant properties allow us to calculate determinants of transformed matrices directly, without performing new determinant expansions.
