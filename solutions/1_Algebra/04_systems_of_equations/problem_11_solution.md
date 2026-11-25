### Exercise 11. A Parameter in a System of Three Equations

**Problem**

Analyze the number of solutions depending on $t$:

$$
\begin{cases}
x+y+z=1, \\
x+ty+z=2, \\
x+y+tz=3.
\end{cases}
$$

Use elimination and separately analyze the parameter values for which a standard calculation step ceases to be valid.

**Solution**

**Part 1: Elimination on the System**

Write the augmented matrix of the system:

$$
\left[
\begin{array}{ccc|c}
1 & 1 & 1 & 1 \\
1 & t & 1 & 2 \\
1 & 1 & t & 3
\end{array}
\right]
$$

Eliminate the entries below the first pivot ($1$ in row $1$, column $1$) using $R_2 \leftarrow R_2 - R_1$ and $R_3 \leftarrow R_3 - R_1$:

$$
\left[
\begin{array}{ccc|c}
1 & 1 & 1 & 1 \\
0 & t - 1 & 0 & 1 \\
0 & 0 & t - 1 & 2
\end{array}
\right]
$$

Translating the second and third rows back into equations gives:

$$
\begin{cases}
x + y + z = 1, \\
(t - 1)y = 1, \\
(t - 1)z = 2.
\end{cases}
$$

**Part 2: Parameter Values Where a Standard Step Becomes Invalid**

In the next standard step, we would normally divide both $(t - 1)y = 1$ and $(t - 1)z = 2$ by $(t - 1)$ to isolate $y$ and $z$.

- **Critical value:** $t = 1$ (since $t - 1 = 0$).
- **Why the step ceases to be valid:** Division by zero is undefined in arithmetic. At $t = 1$, the factor $(t - 1)$ equals $0$, so dividing by $(t - 1)$ is invalid and we cannot use $t - 1$ as a non-zero pivot divisor. Instead, we must substitute $t = 1$ directly into the eliminated equations.

**Part 3: Case Analysis and Number of Solutions**

- **Case 1: $t = 1$**

Substitute $t = 1$ into the eliminated equations:

$$
\begin{cases}
x + y + z = 1, \\
0 \cdot y = 1, \\
0 \cdot z = 2.
\end{cases}
$$

The second equation gives $0 = 1$ (and the third gives $0 = 2$), which is a contradiction.
Therefore, for $t = 1$, the system is inconsistent and has **no solution**.

- **Case 2: $t \neq 1$**

When $t \neq 1$, we have $t - 1 \neq 0$, so dividing is valid and gives:

$$
y = \frac{1}{t - 1}
$$

$$
z = \frac{2}{t - 1}
$$

Substitute $y$ and $z$ into the first equation $x + y + z = 1$:

$$
x + \frac{1}{t - 1} + \frac{2}{t - 1} = 1
$$

$$
x + \frac{3}{t - 1} = 1
$$

$$
x = 1 - \frac{3}{t - 1} = \frac{t - 4}{t - 1}
$$

Therefore, for every $t \neq 1$, the system has a **unique solution**:

$$
x = \frac{t - 4}{t - 1}, \qquad y = \frac{1}{t - 1}, \qquad z = \frac{2}{t - 1}
$$
