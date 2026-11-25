### Exercise 3. Inconsistent System

**Problem**

Solve or show that the system is inconsistent:

$$
\begin{cases}
x+2y=3, \\
2x+4y=7.
\end{cases}
$$

Show how the contradiction appears in the matrix after elimination and interpret it in terms of equations.

**Solution**

**Part 1: Gaussian Elimination on the Augmented Matrix**

First, write the augmented matrix $[A \mid b]$ corresponding to the system:

$$
\left[
\begin{array}{cc|c}
1 & 2 & 3 \\
2 & 4 & 7
\end{array}
\right]
$$

To eliminate the entry below the pivot in the first column, perform the row operation $R_2 \leftarrow R_2 - 2R_1$:

$$
\left[
\begin{array}{cc|c}
1 & 2 & 3 \\
2 - 2(1) & 4 - 2(2) & 7 - 2(3)
\end{array}
\right]
$$

$$
\left[
\begin{array}{cc|c}
1 & 2 & 3 \\
0 & 0 & 1
\end{array}
\right]
$$

**Part 2: How the Contradiction Appears in the Matrix**

After elimination, the second row of the augmented matrix is:

$$
\left[
\begin{array}{cc|c}
0 & 0 & 1
\end{array}
\right]
$$

In the coefficient part of the matrix (to the left of the vertical bar), every entry in the second row is $0$, while the entry in the augmented right-hand side column is non-zero ($1$). Whenever a row of zeros on the left corresponds to a non-zero constant $c \neq 0$ on the right:

$$
\left[
\begin{array}{cccc|c}
0 & 0 & \dots & 0 & c
\end{array}
\right]
$$

the matrix represents an inconsistent system.

**Part 3: Interpretation in Terms of Equations and Geometry**

- **Algebraic Interpretation:** Translating the reduced augmented matrix back into a system of linear equations gives:

$$
\begin{cases}
x + 2y = 3, \\
0x + 0y = 1.
\end{cases}
$$

The second equation simplifies to:

$$
0 = 1
$$

which is an impossible statement (a mathematical contradiction) regardless of the values chosen for $x$ and $y$. Therefore, **no solution exists**, and the system is **inconsistent**.

- **Geometric Interpretation:** Each equation represents a straight line in the $xy$-plane. Rewriting both equations in slope-intercept form gives:

$$
y = -\frac{1}{2}x + \frac{3}{2}
$$

and

$$
y = -\frac{1}{2}x + \frac{7}{4}
$$

Both lines have the exact same slope ($-\frac{1}{2}$) but different $y$-intercepts ($\frac{3}{2} \neq \frac{7}{4}$), meaning they are **parallel lines** that never intersect.
