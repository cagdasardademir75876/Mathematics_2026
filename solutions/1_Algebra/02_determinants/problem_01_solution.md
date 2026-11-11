### Exercise 1. Determinant of a 2×2 Matrix

**Problem**

Compute

$$
\det
\begin{pmatrix}
3 & -2 \\
5 & 4
\end{pmatrix}
$$

and

$$
\det
\begin{pmatrix}
1 & 7 \\
2 & 14
\end{pmatrix}
$$

Which matrix is invertible? Justify your answer.

**Solution**

**Part 1: Computing the Determinants**

For a general $2 \times 2$ matrix

$$
M =
\begin{pmatrix}
a & b \\
c & d
\end{pmatrix}
$$

the determinant is computed using the formula:

$$
\det(M) = ad - bc
$$

- **First Matrix:**

Let $A = \begin{pmatrix} 3 & -2 \\ 5 & 4 \end{pmatrix}$.

$$
\det(A) = (3)(4) - (-2)(5)
$$

$$
\det(A) = 12 - (-10)
$$

$$
\det(A) = 12 + 10 = 22
$$

- **Second Matrix:**

Let $B = \begin{pmatrix} 1 & 7 \\ 2 & 14 \end{pmatrix}$.

$$
\det(B) = (1)(14) - (7)(2)
$$

$$
\det(B) = 14 - 14 = 0
$$

**Part 2: Invertibility and Justification**

A square matrix is invertible if and only if its determinant is non-zero ($\det(M) \neq 0$).

- For matrix $A$, $\det(A) = 22 \neq 0$. Therefore, **matrix $A$ is invertible**.
- For matrix $B$, $\det(B) = 0$. Therefore, **matrix $B$ is not invertible** (it is singular).

**Geometric/Algebraic Justification:** 
Matrix $A$ has linearly independent rows and columns (its columns do not lie on the same line), meaning it spans the full 2D space. In contrast, matrix $B$ has linearly dependent columns (the second column is exactly 7 times the first column: $b_2 = 7b_1$), meaning the transformation collapses 2D space onto a line, yielding a determinant of zero and no inverse.
