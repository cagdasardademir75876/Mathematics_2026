### Exercise 2. Determinant of a 3×3 Matrix

**Problem**

For

$$
A=
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 4 \\
2 & 1 & 5
\end{pmatrix}
$$

compute $\det A$ using Sarrus' rule. Then perform one simple check using a chosen property of the determinant.

**Solution**

**Part 1: Computing $\det A$ Using Sarrus' Rule**

To apply Sarrus' rule for a $3 \times 3$ matrix, we rewrite the first two columns to the right of the matrix:

$$
\begin{vmatrix}
1 & 2 & -1 \\
0 & 3 & 4 \\
2 & 1 & 5
\end{vmatrix}
\begin{matrix}
1 & 2 \\
0 & 3 \\
2 & 1
\end{matrix}
$$

Next, we sum the products of the elements along the main diagonals (moving downwards from left to right) and subtract the products of the elements along the anti-diagonals (moving upwards from left to right):

- **Downward diagonals:**
  - $(1 \cdot 3 \cdot 5) = 15$
  - $(2 \cdot 4 \cdot 2) = 16$
  - $(-1 \cdot 0 \cdot 1) = 0$
  - **Sum of downward products:** $15 + 16 + 0 = 31$

- **Upward diagonals:**
  - $(2 \cdot 3 \cdot -1) = -6$
  - $(1 \cdot 4 \cdot 1) = 4$
  - $(5 \cdot 0 \cdot 2) = 0$
  - **Sum of upward products:** $-6 + 4 + 0 = -2$

- **Calculating the determinant:**

$$
\det(A) = (\text{Sum of downward products}) - (\text{Sum of upward products})
$$

$$
\det(A) = 31 - (-2) = 31 + 2 = 33
$$

Thus, $\det(A) = 33$.

**Part 2: Checking the Result Using a Determinant Property**

To verify our calculation, we can use the property that **adding a multiple of one row to another row does not change the value of the determinant**.

Let's apply a row operation to introduce zeros and simplify the matrix. We can subtract $2$ times Row 1 from Row 3 ($R_3 \leftarrow R_3 - 2R_1$):

- New Row 3 calculation:
  - $(2 - 2(1), \; 1 - 2(2), \; 5 - 2(-1)) = (0, \; 1 - 4, \; 5 + 2) = (0, -3, 7)$

Let the new matrix be $A'$:

$$
A' =
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 4 \\
0 & -3 & 7
\end{pmatrix}
$$

By row operations preserving the determinant, $\det(A') = \det(A) = 33$. 

Now, we can compute $\det(A')$ by expanding along the first column (since it contains zeros):

$$
\det(A') = 1 \cdot
\begin{vmatrix}
3 & 4 \\
-3 & 7
\end{vmatrix}
- 0 + 0
$$

$$
\det(A') = 1 \cdot ((3)(7) - (4)(-3))
$$

$$
\det(A') = 21 - (-12) = 21 + 12 = 33
$$

Since both methods yield $33$, our calculation using Sarrus' rule is verified as correct.
