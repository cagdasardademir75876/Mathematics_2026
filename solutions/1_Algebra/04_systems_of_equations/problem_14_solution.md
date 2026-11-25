### Exercise 14. A Small Change in the Right-Hand Side

**Problem**

Compare the systems

$$
\begin{cases}
x+y=2, \\
2x-y=1, \\
3x=3
\end{cases}
$$

and

$$
\begin{cases}
x+y=2, \\
2x-y=1, \\
3x=3.1.
\end{cases}
$$

Check the consistency of each system and explain why a small change in one number can change the type of the system.

**Solution**

**Part 1: Consistency of the First System**

Consider the first system:

$$
\begin{cases}
x + y = 2, \\
2x - y = 1, \\
3x = 3.
\end{cases}
$$

From the third equation:

$$
3x = 3
$$

$$
x = 1
$$

Substitute $x = 1$ into the first equation:

$$
1 + y = 2
$$

$$
y = 1
$$

Check the second equation with $(x, y) = (1, 1)$:

$$
2(1) - 1 = 2 - 1 = 1
$$

Since $(x, y) = (1, 1)$ satisfies all three equations,
the first system is **consistent** (unique solution: $x = 1, y = 1$).

**Part 2: Consistency of the Second System**

Consider the second system:

$$
\begin{cases}
x + y = 2, \\
2x - y = 1, \\
3x = 3.1.
\end{cases}
$$

Write its augmented matrix:

$$
\left[
\begin{array}{cc|c}
1 & 1 & 2 \\
2 & -1 & 1 \\
3 & 0 & 3.1
\end{array}
\right]
$$

Eliminate below row $1$ using $R_2 \leftarrow R_2 - 2R_1$
and $R_3 \leftarrow R_3 - 3R_1$:

$$
\left[
\begin{array}{cc|c}
1 & 1 & 2 \\
0 & -3 & -3 \\
0 & -3 & -2.9
\end{array}
\right]
$$

Subtract row $2$ from row $3$ ($R_3 \leftarrow R_3 - R_2$):

$$
\left[
\begin{array}{cc|c}
1 & 1 & 2 \\
0 & -3 & -3 \\
0 & 0 & 0.1
\end{array}
\right]
$$

The third row gives:

$$
0x + 0y = 0.1
$$

$$
0 = 0.1
$$

This is a contradiction, so the second system has **no solution**
and is **inconsistent**.

**Part 3: Why a Small Change Changes the System Type**

- **Overdetermined system:** There are $3$ equations in only $2$ unknowns ($x$ and $y$).
  Two non-parallel lines already fix a single intersection $(1, 1)$,
  so the third equation is an extra condition.
- **Exact compatibility:** In the first system, $3x = 3$ matches the sum of the first two equations:

$$
(x + y) + (2x - y) = 2 + 1
$$

$$
3x = 3
$$

  Thus, all three lines meet at $(1, 1)$.
- **Effect of changing $3$ to $3.1$:** The third line shifts to $x = \frac{3.1}{3} \neq 1$.
  The three lines no longer share a common point,
  and the extra equation conflicts with the first two.
  Even a $0.1$ change turns a consistent system into an inconsistent one.
