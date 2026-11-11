### Exercise 5. Row Operations

**Problem**

For

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 1 & 0 \\
-1 & 4 & 2
\end{pmatrix}
$$

find $\det A$ by simplifying the matrix with row operations. At each step, indicate whether and how the determinant changes.

**Solution**

**Part 1: Applying Row Operations to Transform into Upper Triangular Form**

We will use elementary row operations to reduce matrix $A$ to an upper triangular matrix, tracking how each operation affects the determinant.

- **Step 1:** Eliminate the entries below the first element in the first column.

  Perform the row operation $R_2 \leftarrow R_2 - 2R_1$:

  $$
  R_2 - 2R_1 = (2 - 2(1), \; 1 - 2(2), \; 0 - 2(3)) = (0, -3, -6)
  $$

  Perform the row operation $R_3 \leftarrow R_3 + R_1$:

  $$
  R_3 + R_1 = (-1 + 1, \; 4 + 2, \; 2 + 3) = (0, 6, 5)
  $$

  *Effect on Determinant:* Adding a multiple of one row to another **does not change** the value of the determinant. Thus, the determinant remains equal to $\det(A)$.

  The matrix becomes $A_1$:

  $$
  \begin{aligned}
  A_1 &=
  \begin{pmatrix}
  1 & 2 & 3 \\
  0 & -3 & -6 \\
  0 & 6 & 5
  \end{pmatrix}
  \end{aligned}
  $$

- **Step 2:** Eliminate the entry below the leading entry in the second column.

  Perform the row operation $R_3 \leftarrow R_3 + 2R_2$:

  $$
  R_3 + 2R_2 = (0 + 2(0), \; 6 + 2(-3), \; 5 + 2(-6)) = (0, 0, -7)
  $$

  *Effect on Determinant:* Again, adding a multiple of one row to another **does not change** the determinant.

  The matrix is now in upper triangular form ($A_2$):

  $$
  \begin{aligned}
  A_2 &=
  \begin{pmatrix}
  1 & 2 & 3 \\
  0 & -3 & -6 \\
  0 & 0 & -7
  \end{pmatrix}
  \end{aligned}
  $$

**Part 2: Computing the Final Determinant**

Since row operations that add a multiple of one row to another preserve the determinant, we have:

$$
\det(A) = \det(A_2)
$$

For an upper triangular matrix, the determinant is simply the **product of its main diagonal entries**:

$$
\det(A) = (1) \cdot (-3) \cdot (-7)
$$

$$
\det(A) = 21
$$

Thus, $\det(A) = 21$.
