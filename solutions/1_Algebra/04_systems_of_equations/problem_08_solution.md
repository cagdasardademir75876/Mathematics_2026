### Exercise 8. Two Systems with the Same Coefficient Matrix

**Problem**

Solve by elimination the two systems

$$
\begin{cases}
2x+y=5, \\
x-y=1,
\end{cases}
$$

$$
\begin{cases}
2x+y=1, \\
x-y=4.
\end{cases}
$$

Compare the successive elimination steps. Which part of the calculation is the same in both cases, and why?

**Solution**

**Part 1: Solving the First System**

Write the augmented matrix for the first system:

$$
\left[
\begin{array}{cc|c}
2 & 1 & 5 \\
1 & -1 & 1
\end{array}
\right]
$$

- **Step 1:** Swap rows $R_1$ and $R_2$ ($R_1 \leftrightarrow R_2$) to place $1$ in the pivot position:

$$
\left[
\begin{array}{cc|c}
1 & -1 & 1 \\
2 & 1 & 5
\end{array}
\right]
$$

- **Step 2:** Eliminate the entry below the first pivot using $R_2 \leftarrow R_2 - 2R_1$:

$$
\left[
\begin{array}{cc|c}
1 & -1 & 1 \\
0 & 3 & 3
\end{array}
\right]
$$

- **Step 3:** Scale row $2$ by $\frac{1}{3}$ ($R_2 \leftarrow \frac{1}{3}R_2$):

$$
\left[
\begin{array}{cc|c}
1 & -1 & 1 \\
0 & 1 & 1
\end{array}
\right]
$$

- **Step 4:** Eliminate the entry above the second pivot using $R_1 \leftarrow R_1 + R_2$:

$$
\left[
\begin{array}{cc|c}
1 & 0 & 2 \\
0 & 1 & 1
\end{array}
\right]
$$

Thus, the solution to the first system is:

$$
x = 2, \qquad y = 1
$$

**Part 2: Solving the Second System**

Write the augmented matrix for the second system:

$$
\left[
\begin{array}{cc|c}
2 & 1 & 1 \\
1 & -1 & 4
\end{array}
\right]
$$

- **Step 1:** Swap rows $R_1$ and $R_2$ ($R_1 \leftrightarrow R_2$):

$$
\left[
\begin{array}{cc|c}
1 & -1 & 4 \\
2 & 1 & 1
\end{array}
\right]
$$

- **Step 2:** Eliminate the entry below the first pivot using $R_2 \leftarrow R_2 - 2R_1$:

$$
\left[
\begin{array}{cc|c}
1 & -1 & 4 \\
0 & 3 & -7
\end{array}
\right]
$$

- **Step 3:** Scale row $2$ by $\frac{1}{3}$ ($R_2 \leftarrow \frac{1}{3}R_2$):

$$
\left[
\begin{array}{cc|c}
1 & -1 & 4 \\
0 & 1 & -\frac{7}{3}
\end{array}
\right]
$$

- **Step 4:** Eliminate the entry above the second pivot using $R_1 \leftarrow R_1 + R_2$:

$$
\left[
\begin{array}{cc|c}
1 & 0 & \frac{5}{3} \\
0 & 1 & -\frac{7}{3}
\end{array}
\right]
$$

Thus, the solution to the second system is:

$$
x = \frac{5}{3}, \qquad y = -\frac{7}{3}
$$

**Part 3: Comparison and Explanation**

- **What is identical in both cases:**
  - The exact sequence of elementary row operations ($R_1 \leftrightarrow R_2$, $R_2 \leftarrow R_2 - 2R_1$, $R_2 \leftarrow \frac{1}{3}R_2$, and $R_1 \leftarrow R_1 + R_2$) is completely identical.
  - Every intermediate matrix to the left of the vertical bar (the coefficient part) passes through the exact same states, ending in the $2 \times 2$ identity matrix $I_2$.
- **What differs:** Only the numbers in the rightmost augmented column (the right-hand side vector $b$) change at each step.
- **Why this happens:** Which row operations are required to create zeros and normalize pivots depends **exclusively on the entries of the coefficient matrix $A$**. Since both systems share the exact same coefficient matrix:

$$
A =
\begin{pmatrix}
2 & 1 \\
1 & -1
\end{pmatrix}
$$

the elimination procedure itself is completely independent of the right-hand side vector $b$ (in fact, both systems could be solved simultaneously in a single doubly-augmented matrix $\left[ A \mid b_1 \mid b_2 \right]$).
