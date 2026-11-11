### Exercise 8. Row Operations and Their Reversibility

**Problem**

For

$$
A=
\begin{pmatrix}
1 & 2 & -1 \\
2 & 4 & 1 \\
-1 & 1 & 3
\end{pmatrix}
$$

perform, in order:

1. $R_2\leftarrow R_2-2R_1$,
2. $R_3\leftarrow R_3+R_1$,
3. interchange $R_2$ and $R_3$.

Write the matrix after each step. Then, for each of the three operations, state an operation that reverses it.

**Solution**

**Part 1: Performing Elementary Row Operations**

We start with the initial matrix:

$$
A =
\begin{pmatrix}
1 & 2 & -1 \\
2 & 4 & 1 \\
-1 & 1 & 3
\end{pmatrix}
$$

- **Step 1:** $R_2 \leftarrow R_2 - 2R_1$

Subtract 2 times Row 1 from Row 2:
- New $R_2 = (2 - 2(1), \; 4 - 2(2), \; 1 - 2(-1)) = (0, \; 0, \; 3)$

$$
\begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 3 \\
-1 & 1 & 3
\end{pmatrix}
$$

- **Step 2:** $R_3 \leftarrow R_3 + R_1$

Add Row 1 to Row 3:
- New $R_3 = (-1 + 1, \; 1 + 2, \; 3 + (-1)) = (0, \; 3, \; 2)$

$$
\begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 3 \\
0 & 3 & 2
\end{pmatrix}
$$

- **Step 3:** Interchange $R_2$ and $R_3$ ($R_2 \leftrightarrow R_3$)

Swap the second and third rows:

$$
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 2 \\
0 & 0 & 3
\end{pmatrix}
$$

**Part 2: Reversing the Row Operations**

Each elementary row operation is reversible:

1. **Reversing Step 1 ($R_2 \leftarrow R_2 - 2R_1$):**
   - **Inverse Operation:** Add $2R_1$ back to $R_2$, i.e., $R_2 \leftarrow R_2 + 2R_1$.

2. **Reversing Step 2 ($R_3 \leftarrow R_3 + R_1$):**
   - **Inverse Operation:** Subtract $R_1$ from $R_3$, i.e., $R_3 \leftarrow R_3 - R_1$.

3. **Reversing Step 3 ($R_2 \leftrightarrow R_3$):**
   - **Inverse Operation:** Interchange $R_2$ and $R_3$ again, i.e., $R_2 \leftrightarrow R_3$.
