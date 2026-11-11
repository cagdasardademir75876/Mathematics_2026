
### Exercise 11. Shortening the Calculation with Row Operations

**Problem**

Compute

$$
\det
\begin{pmatrix}
1 & 2 & 3 \\
1 & 3 & 4 \\
1 & 4 & 6 \\
\end{pmatrix}
$$

by first performing row operations that create as many zeros as possible. State which operations do not change the determinant.

> **Why this exercise:** develops planning instead of mechanically repeating the same procedure.

**Solution**

**1. Writing the Matrix**

Let

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
1 & 3 & 4 \\
1 & 4 & 6 \\
\end{pmatrix}
$$

To simplify the determinant calculation, we will use elementary row operations.

**2. Performing Row Operations**

First, subtract the first row from the second row:

$$
R_2\leftarrow R_2-R_1
$$

Then subtract the first row from the third row:

$$
R_3\leftarrow R_3-R_1
$$

The resulting matrix is

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 2 & 3 \\
\end{pmatrix}
$$

Next, subtract twice the second row from the third row:

$$
R_3\leftarrow R_3-2R_2
$$

This gives

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 0 & 1 \\
\end{pmatrix}
$$

**3. Computing the Determinant**

All the operations used above involve adding a multiple of one row to another row.

Such operations do not change the determinant.

The resulting matrix is upper triangular, so its determinant is the product of its diagonal entries.

$$
\det(A)=1\cdot1\cdot1
$$

$$
\det(A)=1
$$

**4. Explanation of the Row Operations**

The following row operation does not change the determinant:

$$
R_i\leftarrow R_i+cR_j
$$

where $c$ is a scalar and $i\neq j$.

However, swapping two rows changes the sign of the determinant, and multiplying a row by a scalar multiplies the determinant by that scalar.

In this exercise, only determinant-preserving row operations were used.

**Final Answer**

$$
\det(A)=1
$$

The determinant was calculated efficiently by transforming the matrix into upper triangular form without changing its determinant.
