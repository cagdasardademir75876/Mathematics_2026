### Exercise 5. A 3×3 Matrix

**Problem**

Use Gauss–Jordan elimination to find the inverse of

$$
A=
\begin{pmatrix}
1 & 1 & 0 \\
0 & 1 & 1 \\
1 & 0 & 1
\end{pmatrix}
$$

Check the result by multiplication.

**Solution**

**Part 1: Gauss–Jordan Elimination**

We set up the augmented matrix $[A \mid I_3]$:

$$
\left[
\begin{array}{ccc|ccc}
1 & 1 & 0 & 1 & 0 & 0 \\
0 & 1 & 1 & 0 & 1 & 0 \\
1 & 0 & 1 & 0 & 0 & 1
\end{array}
\right]
$$

- **Step 1:** Eliminate the entry below the first pivot in column 1 by performing $R_3 \leftarrow R_3 - R_1$.

  The augmented matrix becomes:

  $$
  \left[
  \begin{array}{ccc|ccc}
  1 & 1 & 0 & 1 & 0 & 0 \\
  0 & 1 & 1 & 0 & 1 & 0 \\
  0 & -1 & 1 & -1 & 0 & 1
  \end{array}
  \right]
  $$

- **Step 2:** Eliminate the entry below the second pivot in column 2 by performing $R_3 \leftarrow R_3 + R_2$.

  The augmented matrix becomes:

  $$
  \left[
  \begin{array}{ccc|ccc}
  1 & 1 & 0 & 1 & 0 & 0 \\
  0 & 1 & 1 & 0 & 1 & 0 \\
  0 & 0 & 2 & -1 & 1 & 1
  \end{array}
  \right]
  $$

- **Step 3:** Scale the third row so that its pivot becomes $1$ by performing $R_3 \leftarrow \frac{1}{2} R_3$.

  The augmented matrix becomes:

  $$
  \left[
  \begin{array}{ccc|ccc}
  1 & 1 & 0 & 1 & 0 & 0 \\
  0 & 1 & 1 & 0 & 1 & 0 \\
  0 & 0 & 1 & -\frac{1}{2} & \frac{1}{2} & \frac{1}{2}
  \end{array}
  \right]
  $$

- **Step 4:** Eliminate the entry above the third pivot in column 3 by performing $R_2 \leftarrow R_2 - R_3$.

  The augmented matrix becomes:

  $$
  \left[
  \begin{array}{ccc|ccc}
  1 & 1 & 0 & 1 & 0 & 0 \\
  0 & 1 & 0 & \frac{1}{2} & \frac{1}{2} & -\frac{1}{2} \\
  0 & 0 & 1 & -\frac{1}{2} & \frac{1}{2} & \frac{1}{2}
  \end{array}
  \right]
  $$

- **Step 5:** Eliminate the entry above the second pivot in column 2 by performing $R_1 \leftarrow R_1 - R_2$.

  The augmented matrix reaches reduced row echelon form:

  $$
  \left[
  \begin{array}{ccc|ccc}
  1 & 0 & 0 & \frac{1}{2} & -\frac{1}{2} & \frac{1}{2} \\
  0 & 1 & 0 & \frac{1}{2} & \frac{1}{2} & -\frac{1}{2} \\
  0 & 0 & 1 & -\frac{1}{2} & \frac{1}{2} & \frac{1}{2}
  \end{array}
  \right]
  $$

Since the left block is now $I_3$, the inverse matrix $A^{-1}$ is given by the right block:

$$
A^{-1} =
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} & \frac{1}{2} \\
\frac{1}{2} & \frac{1}{2} & -\frac{1}{2} \\
-\frac{1}{2} & \frac{1}{2} & \frac{1}{2}
\end{pmatrix}
= \frac{1}{2}
\begin{pmatrix}
1 & -1 & 1 \\
1 & 1 & -1 \\
-1 & 1 & 1
\end{pmatrix}
$$

**Part 2: Checking the Result by Multiplication**

We compute the product $A A^{-1}$ to verify that it equals $I_3$:

$$
A A^{-1} =
\begin{pmatrix}
1 & 1 & 0 \\
0 & 1 & 1 \\
1 & 0 & 1
\end{pmatrix}
\cdot \frac{1}{2}
\begin{pmatrix}
1 & -1 & 1 \\
1 & 1 & -1 \\
-1 & 1 & 1
\end{pmatrix}
$$

$$
A A^{-1} = \frac{1}{2}
\begin{pmatrix}
1(1) + 1(1) + 0(-1) & 1(-1) + 1(1) + 0(1) & 1(1) + 1(-1) + 0(1) \\
0(1) + 1(1) + 1(-1) & 0(-1) + 1(1) + 1(1) & 0(1) + 1(-1) + 1(1) \\
1(1) + 0(1) + 1(-1) & 1(-1) + 0(1) + 1(1) & 1(1) + 0(-1) + 1(1)
\end{pmatrix}
$$

$$
A A^{-1} = \frac{1}{2}
\begin{pmatrix}
1 + 1 + 0 & -1 + 1 + 0 & 1 - 1 + 0 \\
0 + 1 - 1 & 0 + 1 + 1 & 0 - 1 + 1 \\
1 + 0 - 1 & -1 + 0 + 1 & 1 + 0 + 1
\end{pmatrix}
$$

$$
A A^{-1} = \frac{1}{2}
\begin{pmatrix}
2 & 0 & 0 \\
0 & 2 & 0 \\
0 & 0 & 2
\end{pmatrix}
=
\begin{pmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{pmatrix}
= I_3
$$

Since $A A^{-1} = I_3$, the computed inverse is verified as correct.
