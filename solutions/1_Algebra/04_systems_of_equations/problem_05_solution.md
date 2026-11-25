### Exercise 5. Row Echelon Form and Number of Solutions

**Problem**

For the augmented matrix

$$
\begin{pmatrix}
1 & 2 & -1 & \mid & 3 \\
0 & 1 & 2 & \mid & 1 \\
0 & 0 & 0 & \mid & 0
\end{pmatrix}
$$

determine the number of solutions and write them in parametric form. Explain how you know how many variables may be chosen freely.

**Solution**

**Part 1: Number of Solutions**

The given matrix is already in row echelon form:

- The third row is all zeros ($0 = 0$), so there is no contradiction of the form $0 = c$ ($c \neq 0$). Thus, the system is **consistent**.
- There are $3$ unknowns ($x, y, z$) and $2$ pivot positions (entry $(1,1)$ equal to $1$, and entry $(2,2)$ equal to $1$).
- Because the system is consistent and has at least one free variable, it has **infinitely many solutions**.

**Part 2: How Many Variables Can Be Chosen Freely**

In general, for a consistent linear system in row echelon form:

$$
\text{Number of free variables} = \text{Number of unknowns} - \text{Number of pivot columns}
$$

Here, there are $3$ variables in total ($x$, $y$, and $z$), and pivot columns occur in column $1$ and column $2$ ($2$ pivot columns). Column $3$ (corresponding to $z$) has no pivot, so **$1$ variable may be chosen freely** ($z$ is the free variable, while $x$ and $y$ are basic/pivot variables).

**Part 3: Parametric Form of the Solution**

Let the free variable be $z = t$, where $t \in \mathbb{R}$.

From the second row ($y + 2z = 1$), substitute $z = t$:

$$
y + 2t = 1
$$

$$
y = 1 - 2t
$$

From the first row ($x + 2y - z = 3$), substitute $y = 1 - 2t$ and $z = t$:

$$
x + 2(1 - 2t) - t = 3
$$

$$
x + 2 - 4t - t = 3
$$

$$
x + 2 - 5t = 3
$$

$$
x = 1 + 5t
$$

Thus, the general solution in parametric form (for $t \in \mathbb{R}$) is:

$$
x = 1 + 5t, \qquad y = 1 - 2t, \qquad z = t
$$

Or in vector form:

$$
\mathbf{x} = \mathbf{p} + t\mathbf{v}
$$

where:

$$
\mathbf{p} =
\begin{pmatrix}
1 \\
1 \\
0
\end{pmatrix}
\qquad
\mathbf{v} =
\begin{pmatrix}
5 \\
-2 \\
1
\end{pmatrix}
$$
