### Exercise 8. Row Operations and Their Reversibility

Given

$$
A=\begin{pmatrix}
1 & 2 & -1 \\
2 & 4 & 1 \\
-1 & 1 & 3 \\
\end{pmatrix}
$$

---

#### 1. Step-by-Step Row Operations

**Step 1: Apply $R_2 \leftarrow R_2 - 2R_1$**

Subtract $2$ times the first row from the second row:
* New $R_2 = (2, 4, 1) - 2(1, 2, -1) = (2, 4, 1) - (2, 4, -2) = (0, 0, 3)$

The matrix becomes:
$$
A_1 = \begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 3 \\
-1 & 1 & 3 \\
\end{pmatrix}
$$

**Step 2: Apply $R_3 \leftarrow R_3 + R_1$**

Add the first row to the third row:
* New $R_3 = (-1, 1, 3) + (1, 2, -1) = (0, 3, 2)$

The matrix becomes:
$$
A_2 = \begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 3 \\
0 & 3 & 2 \\
\end{pmatrix}
$$

**Step 3: Interchange $R_2$ and $R_3$**

Swap the second and third rows:
* New $R_2 = (0, 3, 2)$
* New $R_3 = (0, 0, 3)$

The final matrix becomes:
$$
A_3 = \begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 2 \\
0 & 0 & 3 \\
\end{pmatrix}
$$

---

#### 2. Reversing Operations

To reverse each of the operations and restore the original matrix, we apply the inverse operations in the reverse order (or individually):

1. **Reversing $R_2 \leftarrow R_2 - 2R_1$:**
   * Inverse operation: $R_2 \leftarrow R_2 + 2R_1$

2. **Reversing $R_3 \leftarrow R_3 + R_1$:**
   * Inverse operation: $R_3 \leftarrow R_3 - R_1$

3. **Reversing the row interchange (interchange $R_2$ and $R_3$):**
   * Inverse operation: Interchange $R_2$ and $R_3$ again (swap them back).
