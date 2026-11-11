
### Exercise 13. Determinant by Elimination

**Problem**

Compute the determinant

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 5 & 7 \\
1 & 0 & 2 \\
\end{pmatrix}
$$

using elimination. Record the effect of every row operation used on the value of the determinant.

> **Why this exercise:** reinforces organizing a determinant calculation through row operations without introducing an unnecessary second procedure.

**Solution**

**1. Writing the Original Matrix**

We are given

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 5 & 7 \\
1 & 0 & 2 \\
\end{pmatrix}
$$

Our goal is to transform this matrix into upper triangular form using row operations.

**2. First Row Operation**

Subtract twice the first row from the second row:

$$
R_2\leftarrow R_2-2R_1
$$

This gives

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
1 & 0 & 2 \\
\end{pmatrix}
$$

Adding a multiple of one row to another does not change the determinant.

**3. Second Row Operation**

Subtract the first row from the third row:

$$
R_3\leftarrow R_3-R_1
$$

The matrix becomes

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & -2 & -1 \\
\end{pmatrix}
$$

This operation also does not change the determinant.

**4. Third Row Operation**

Add twice the second row to the third row:

$$
R_3\leftarrow R_3+2R_2
$$

We obtain

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 0 & 1 \\
\end{pmatrix}
$$

This operation also preserves the determinant.

**5. Computing the Determinant**

The resulting matrix is upper triangular.

The determinant of an upper triangular matrix is the product of its diagonal entries.

Therefore,

$$
\det(A)=1\cdot1\cdot1
$$

$$
\det(A)=1
$$

**6. Effect of the Row Operations**

All three operations have the form

$$
R_i\leftarrow R_i+cR_j
$$

These operations do not change the determinant.

No row swaps or row multiplications by non-unit scalars were performed. Therefore, the determinant remains unchanged throughout the elimination process.

**Final Answer**

$$
\det(A)=1
$$

The determinant is equal to $1$, and all row operations used preserve its value.
