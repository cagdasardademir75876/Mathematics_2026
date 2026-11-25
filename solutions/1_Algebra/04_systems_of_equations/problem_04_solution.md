### Exercise 4. Infinitely Many Solutions

**Problem**

Solve

$$
\begin{cases}
x+y+z=2, \\
2x+2y+2z=4, \\
x-y+z=0.
\end{cases}
$$

Give the solution in parametric form, identify a free variable, and for one chosen parameter value check that the resulting point really satisfies the system.

**Solution**

**Part 1: Gaussian Elimination on the Augmented Matrix**

First, write the augmented matrix corresponding to the system:

$$
\left[
\begin{array}{ccc|c}
1 & 1 & 1 & 2 \\
2 & 2 & 2 & 4 \\
1 & -1 & 1 & 0
\end{array}
\right]
$$

**Step 1:** Eliminate the entries below the first pivot ($1$ in row $1$, column $1$) using $R_2 \leftarrow R_2 - 2R_1$ and $R_3 \leftarrow R_3 - R_1$:

$$
\left[
\begin{array}{ccc|c}
1 & 1 & 1 & 2 \\
0 & 0 & 0 & 0 \\
0 & -2 & 0 & -2
\end{array}
\right]
$$

**Step 2:** Swap row $2$ and row $3$ ($R_2 \leftrightarrow R_3$) so the zero row moves to the bottom:

$$
\left[
\begin{array}{ccc|c}
1 & 1 & 1 & 2 \\
0 & -2 & 0 & -2 \\
0 & 0 & 0 & 0
\end{array}
\right]
$$

**Step 3:** Scale row $2$ by $-\frac{1}{2}$ ($R_2 \leftarrow -\frac{1}{2}R_2$) to make the second pivot equal to $1$:

$$
\left[
\begin{array}{ccc|c}
1 & 1 & 1 & 2 \\
0 & 1 & 0 & 1 \\
0 & 0 & 0 & 0
\end{array}
\right]
$$

**Step 4:** Eliminate the entry above the second pivot using $R_1 \leftarrow R_1 - R_2$:

$$
\left[
\begin{array}{ccc|c}
1 & 0 & 1 & 1 \\
0 & 1 & 0 & 1 \\
0 & 0 & 0 & 0
\end{array}
\right]
$$

The third row is completely zeros ($0 = 0$), meaning the system is consistent and has **infinitely many solutions**.

**Part 2: Identifying the Free Variable and Parametric Form**

In the reduced row echelon form:

- Column $1$ ($x$) has a leading pivot ($1$).
- Column $2$ ($y$) has a leading pivot ($1$).
- Column $3$ ($z$) has **no pivot**, so **$z$ is the free variable**.

Let $z = t$, where $t \in \mathbb{R}$ is an arbitrary real parameter. Translating the first two rows back into equations gives:

$$
\begin{cases}
x + z = 1, \\
y = 1.
\end{cases}
$$

Solving for the basic variables $x$ and $y$ in terms of $t$:

$$
x = 1 - t
$$

$$
y = 1
$$

$$
z = t
$$

Thus, the general solution in parametric vector form (for $t \in \mathbb{R}$) is:

$$
\begin{aligned}
\begin{pmatrix}
x \\
y \\
z
\end{pmatrix}
&=
\begin{pmatrix}
1 \\
1 \\
0
\end{pmatrix}
+ t
\begin{pmatrix}
-1 \\
0 \\
1
\end{pmatrix}
\end{aligned}
$$

**Part 3: Checking a Chosen Parameter Value**

Choose the parameter value $t = 2$. Substituting $t = 2$ into the parametric formulas gives the specific point:

$$
x = 1 - 2 = -1
$$

$$
y = 1
$$

$$
z = 2
$$

So the candidate solution point is $(x, y, z) = (-1, 1, 2)$. Substitute these values into all three original equations to verify:

- **First equation:**

$$
x + y + z = (-1) + 1 + 2 = 2
$$

Matches the right-hand side $2$.

- **Second equation:**

$$
2x + 2y + 2z = 2(-1) + 2(1) + 2(2) = -2 + 2 + 4 = 4
$$

Matches the right-hand side $4$.

- **Third equation:**

$$
x - y + z = (-1) - 1 + 2 = 0
$$

Matches the right-hand side $0$.

Since $(-1, 1, 2)$ satisfies all three equations, the parametric solution is verified.
