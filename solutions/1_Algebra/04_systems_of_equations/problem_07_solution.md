### Exercise 7. Choosing a Method Deliberately

**Problem**

Do not solve all of the following systems completely. For each situation, choose the method that best uses its structure and justify your choice:

1. one system with a triangular coefficient matrix

$$
\begin{cases}
2x-y=3, \\
4y=8;
\end{cases}
$$

2. three systems $Ax=b_i$ with the same invertible matrix $A$, when $A^{-1}$ is already known;
3. one $3\times3$ system for which the inverse matrix is not given and the goal is only to find one solution vector.

For case 1, carry out the chosen method completely. For cases 2 and 3, describe the plan and indicate which part of the computation would be reusable or unnecessary. Do not judge a method by its name alone — refer to the number of right-hand sides and the structure of the matrix.

**Solution**

**Case 1: System with a Triangular Coefficient Matrix**

- **Chosen Method:** Direct back-substitution (without row reduction or matrix inversion).
- **Justification:** There is only $1$ right-hand side, and the coefficient matrix is already upper triangular:

$$
A =
\begin{pmatrix}
2 & -1 \\
0 & 4
\end{pmatrix}
$$

Because the entry below the main diagonal is already $0$, forward elimination is completely unnecessary. Computing $A^{-1}$ would also do extra work when $y$ can be read off directly from the last equation.

- **Complete Execution:**

From the second equation:

$$
4y = 8
$$

$$
y = 2
$$

Substitute $y = 2$ into the first equation:

$$
2x - 2 = 3
$$

$$
2x = 5
$$

$$
x = \frac{5}{2}
$$

Thus, the solution is:

$$
x = \frac{5}{2}, \qquad y = 2
$$

**Case 2: Three Systems $Ax = b_i$ with Known $A^{-1}$**

- **Chosen Method:** Matrix-vector multiplication $x_i = A^{-1}b_i$ for each right-hand side $i = 1, 2, 3$.
- **Justification:** There are $3$ different right-hand side vectors ($b_1, b_2, b_3$) sharing the exact same coefficient matrix $A$, and $A^{-1}$ is already provided.
- **Plan and Reusable vs. Unnecessary Work:**
  - **Reusable part:** The precomputed inverse matrix $A^{-1}$ is reused directly across all three systems without performing any row operations or re-factoring $A$.
  - **Execution plan:** Compute $x_1 = A^{-1}b_1$, $x_2 = A^{-1}b_2$, and $x_3 = A^{-1}b_3$ via three separate matrix-vector products.
  - **Unnecessary part:** Running Gaussian elimination three separate times from scratch (or inverting $A$ again) is completely unnecessary.

**Case 3: One $3 \times 3$ System Without $A^{-1}$ Given**

- **Chosen Method:** Gaussian elimination on the augmented matrix $\left[ A \mid b \right]$ followed by back-substitution.
- **Justification:** There is only $1$ right-hand side vector $b$, the matrix $A$ is general (not given in triangular form), and $A^{-1}$ is unknown.
- **Plan and Reusable vs. Unnecessary Work:**
  - **Execution plan:** Form the $3 \times 4$ augmented matrix $\left[ A \mid b \right]$, apply elementary row operations to reduce the left $3 \times 3$ block to upper triangular (row echelon) form, and solve for the three unknowns via back-substitution.
  - **Unnecessary part:** Computing the full inverse matrix $A^{-1}$ (which requires reducing a $3 \times 6$ augmented matrix $\left[ A \mid I_3 \right]$ all the way to reduced row echelon form) is unnecessary, because $A^{-1}$ will never be reused for additional right-hand sides.
