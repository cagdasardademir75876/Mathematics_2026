
### Exercise 10. Detecting Dependence

**Problem**

Without carrying out a full determinant calculation, explain why

$$
\det
\begin{pmatrix}
1 & 2 & 3 \\
2 & 4 & 6 \\
0 & 1 & 5 \\
\end{pmatrix}=0.
$$

Identify a specific dependence between the rows and connect it with noninvertibility of the matrix.

> **Why this exercise:** teaches how to recognize a zero determinant from the structure of a matrix.

**Solution**

**1. Identifying the Dependence Between the Rows**

Let the rows of the given matrix be denoted by $R_1$, $R_2$, and $R_3$.

The first two rows are

$$
R_1=(1,2,3)
$$

$$
R_2=(2,4,6)
$$

We can see that the second row is exactly twice the first row:

$$
R_2=2R_1
$$

Therefore, the rows are linearly dependent.

**2. Why the Determinant Is Zero**

A fundamental property of determinants states that if two rows of a matrix are proportional, or if the rows are otherwise linearly dependent, the determinant is zero.

Since $R_2=2R_1$, the determinant must satisfy

$$
\det(A)=0
$$

This conclusion is obtained directly from the structure of the matrix, without calculating the determinant.

**3. Connection with Noninvertibility**

A square matrix is invertible if and only if its determinant is nonzero.

Since the determinant is zero,

$$
\det(A)=0
$$

the matrix is not invertible.

The linear dependence between its rows means that the rows cannot form a basis of $\mathbb{R}^3$.

**Final Answer**

The second row is twice the first row:

$$
R_2=2R_1
$$

Therefore, the rows are linearly dependent, the determinant is zero, and the matrix is not invertible.
