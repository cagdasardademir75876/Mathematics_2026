### Exercise 12. Homogeneous System

**Problem**

Solve

$$
\begin{cases}
x+2y-z=0, \\
2x+4y-2z=0, \\
x-y+2z=0.
\end{cases}
$$

Give all solutions in parametric form and explain why $(0,0,0)$ always satisfies a homogeneous system.

**Solution**

**Part 1: Gaussian Elimination on the Augmented Matrix**

Write the augmented matrix corresponding to the system:

$$
\left[
\begin{array}{ccc|c}
1 & 2 & -1 & 0 \\
2 & 4 & -2 & 0 \\
1 & -1 & 2 & 0
\end{array}
\right]
$$

- **Step 1:** Eliminate the entries below the first pivot ($1$ in row $1$, column $1$) using $R_2 \leftarrow R_2 - 2R_1$ and $R_3 \leftarrow R_3 - R_1$:

$$
\left[
\begin{array}{ccc|c}
1 & 2 & -1 & 0 \\
0 & 0 & 0 & 0 \\
0 & -3 & 3 & 0
\end{array}
\right]
$$

- **Step 2:** Swap row $2$ and row $3$ ($R_2 \leftrightarrow R_3$) so the zero row is at the bottom:

$$
\left[
\begin{array}{ccc|c}
1 & 2 & -1 & 0 \\
0 & -3 & 3 & 0 \\
0 & 0 & 0 & 0
\end{array}
\right]
$$

- **Step 3:** Scale row $2$ by $-\frac{1}{3}$ ($R_2 \leftarrow -\frac{1}{3}R_2$) to make the second pivot equal to $1$:

$$
\left[
\begin{array}{ccc|c}
1 & 2 & -1 & 0 \\
0 & 1 & -1 & 0 \\
0 & 0 & 0 & 0
\end{array}
\right]
$$

- **Step 4:** Eliminate the entry above the second pivot using $R_1 \leftarrow R_1 - 2R_2$:

$$
\left[
\begin{array}{ccc|c}
1 & 0 & 1 & 0 \\
0 & 1 & -1 & 0 \\
0 & 0 & 0 & 0
\end{array}
\right]
$$

**Part 2: Parametric Form of All Solutions**

In the reduced row echelon form:

- Column $1$ ($x$) has a pivot ($1$).
- Column $2$ ($y$) has a pivot ($1$).
- Column $3$ ($z$) has **no pivot**, so **$z$ is the free variable**.

Let $z = t$, where $t \in \mathbb{R}$. Translating the first two rows back into equations gives:

$$
\begin{cases}
x + z = 0, \\
y - z = 0.
\end{cases}
$$

Expressing $x$ and $y$ in terms of $t$:

$$
x = -t
$$

$$
y = t
$$

$$
z = t
$$

Thus, all solutions in parametric form (for $t \in \mathbb{R}$) are:

$$
x = -t, \qquad y = t, \qquad z = t
$$

Or in vector form:

$$
\mathbf{x} = t\mathbf{v}, \qquad \mathbf{v} =
\begin{pmatrix}
-1 \\
1 \\
1
\end{pmatrix}
$$

**Part 3: Why $(0, 0, 0)$ Always Satisfies a Homogeneous System**

A homogeneous linear system has the matrix form $Ax = \mathbf{0}$, where every constant term on the right-hand side is zero.
When we substitute the zero vector $\mathbf{x} = (0, 0, 0)$ into the left-hand side, each linear combination of variables evaluates to zero because multiplying any coefficient by $0$ gives $0$, and adding zeros gives $0$:

$$
A\mathbf{0} = \mathbf{0}
$$

In this specific problem, setting the parameter $t = 0$ in the parametric solution yields $(x, y, z) = (0, 0, 0)$, confirming that the trivial solution always belongs to the solution set of a homogeneous system.
