### Exercise 2. Gaussian Elimination — One Solution

**Problem**

Solve using Gaussian elimination:

$$
\begin{cases}
x+y+z=6, \\
2x-y+z=3, \\
x+2y-z=2.
\end{cases}
$$

After solving, substitute the result into all equations and check consistency.

**Solution**

**Part 1: Setting Up the Augmented Matrix and Forward Elimination**

The augmented matrix $[A \mid b]$ corresponding to the given system is:

$$
\left[
\begin{array}{ccc|c}
1 & 1 & 1 & 6 \\
2 & -1 & 1 & 3 \\
1 & 2 & -1 & 2
\end{array}
\right]
$$

**Step 1:** Eliminate the entries below the first pivot ($1$ in row $1$, column $1$) using $R_2 \leftarrow R_2 - 2R_1$ and $R_3 \leftarrow R_3 - R_1$:

$$
\left[
\begin{array}{ccc|c}
1 & 1 & 1 & 6 \\
0 & -3 & -1 & -9 \\
0 & 1 & -2 & -4
\end{array}
\right]
$$

**Step 2:** Swap row $2$ and row $3$ ($R_2 \leftrightarrow R_3$) to obtain a clean pivot of $1$ in the second column:

$$
\left[
\begin{array}{ccc|c}
1 & 1 & 1 & 6 \\
0 & 1 & -2 & -4 \\
0 & -3 & -1 & -9
\end{array}
\right]
$$

**Step 3:** Eliminate the entry below the second pivot ($1$ in row $2$, column $2$) using $R_3 \leftarrow R_3 + 3R_2$:

$$
\left[
\begin{array}{ccc|c}
1 & 1 & 1 & 6 \\
0 & 1 & -2 & -4 \\
0 & 0 & -7 & -21
\end{array}
\right]
$$

The matrix is now in upper triangular (row echelon) form with three non-zero pivots ($1$, $1$, and $-7$), which indicates a unique solution.

**Part 2: Back-Substitution**

From the third row, we have:

$$
-7z = -21
$$

$$
z = 3
$$

Substitute $z = 3$ into the equation from the second row:

$$
y - 2z = -4
$$

$$
y - 2(3) = -4
$$

$$
y - 6 = -4
$$

$$
y = 2
$$

Substitute $y = 2$ and $z = 3$ into the equation from the first row:

$$
x + y + z = 6
$$

$$
x + 2 + 3 = 6
$$

$$
x + 5 = 6
$$

$$
x = 1
$$

Thus, the unique solution is $(x, y, z) = (1, 2, 3)$.

**Part 3: Substitution and Consistency Check**

Substitute $x = 1$, $y = 2$, and $z = 3$ into each of the original equations:

- **First equation:**

$$
x + y + z = 1 + 2 + 3 = 6
$$

This matches the right-hand side $6$.

- **Second equation:**

$$
2x - y + z = 2(1) - 2 + 3 = 2 - 2 + 3 = 3
$$

This matches the right-hand side $3$.

- **Third equation:**

$$
x + 2y - z = 1 + 2(2) - 3 = 1 + 4 - 3 = 2
$$

This matches the right-hand side $2$.

Since $(x, y, z) = (1, 2, 3)$ satisfies all three equations simultaneously without contradiction, the system is **consistent** and has **exactly one solution**.
