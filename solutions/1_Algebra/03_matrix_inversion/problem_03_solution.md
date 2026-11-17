### Exercise 3. When Does the Inverse Not Exist?

**Problem**

For

$$
A=
\begin{pmatrix}
2 & 4 \\
1 & 2
\end{pmatrix}
$$

explain in two ways why $A^{-1}$ does not exist: using the determinant and using dependence between the rows.

**Solution**

**Method 1: Using the Determinant**

A square matrix $A$ has an inverse $A^{-1}$ if and only if its determinant is non-zero ($\det(A) \neq 0$). 

For the given $2 \times 2$ matrix $A$, we compute the determinant as follows:

$$
\det(A) = (2)(2) - (4)(1)
$$

$$
\det(A) = 4 - 4 = 0
$$

Since $\det(A) = 0$, the matrix is singular and therefore **$A^{-1}$ does not exist**. (In the $2 \times 2$ inverse formula, this would require dividing by $\det(A) = 0$, which is undefined).

**Method 2: Using Linear Dependence Between the Rows**

An $n \times n$ matrix is invertible if and only if its rows (and columns) are linearly independent.

Let $R_1$ and $R_2$ denote the first and second rows of matrix $A$:

$$
R_1 = \begin{pmatrix} 2 & 4 \end{pmatrix}
$$

$$
R_2 = \begin{pmatrix} 1 & 2 \end{pmatrix}
$$

We can observe that the first row is an exact scalar multiple of the second row:

$$
R_1 = 2 R_2
$$

Equivalently, we can write a non-trivial linear combination of the rows that equals the zero vector:

$$
R_1 - 2 R_2 = \begin{pmatrix} 0 & 0 \end{pmatrix}
$$

Because the rows of $A$ are **linearly dependent**, performing row reduction (Gaussian elimination) will produce an entire row of zeros, meaning $A$ cannot be reduced to the $2 \times 2$ identity matrix $I_2$. Consequently, **$A^{-1}$ does not exist**.
