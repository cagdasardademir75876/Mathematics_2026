
### Exercise 14. A System of Equations and the Determinant

**Problem**

Consider the system $Ax=b$, where

$$
A=
\begin{pmatrix}
1 & 2 \\
k & 4 \\
\end{pmatrix}.
$$

For which values of $k$ does the system have exactly one solution for every $b$? For the remaining value, give an example of a right-hand side $b$ for which the system has infinitely many solutions, and an example for which it has no solution.

> **Why this exercise:** connects the determinant with uniqueness of solutions and requires distinguishing the exceptional cases.

**Solution**

**1. Finding the Values of $k$**

A square linear system $Ax=b$ has exactly one solution for every right-hand side $b$ if and only if the coefficient matrix $A$ is invertible.

A matrix is invertible if and only if its determinant is nonzero.

First, calculate the determinant:

$$
\det(A)=
\begin{vmatrix}
1 & 2 \\
k & 4
\end{vmatrix}
$$

Using the formula for a $2\times2$ determinant,

$$
\det(A)=1\cdot4-2\cdot k
$$

Therefore,

$$
\det(A)=4-2k
$$

The matrix is invertible when

$$
4-2k\neq0
$$

Solving this inequality gives

$$
k\neq2
$$

Thus, the system has exactly one solution for every $b$ when $k\neq2$.

**2. The Exceptional Case: $k=2$**

When $k=2$, the coefficient matrix becomes

$$
A=
\begin{pmatrix}
1 & 2 \\
2 & 4 \\
\end{pmatrix}
$$

The second row is twice the first row.

Therefore, the determinant is zero, and the matrix is not invertible.

The system becomes

$$
\begin{cases}
x+2y=b_1, \\
2x+4y=b_2.
\end{cases}
$$

The second equation is twice the first equation on the left-hand side.

Consequently, the system has either infinitely many solutions or no solution, depending on the right-hand side.

**3. Example with Infinitely Many Solutions**

Choose

$$
b=
\begin{pmatrix}
1 \\
2 \\
\end{pmatrix}
$$

The system becomes

$$
\begin{cases}
x+2y=1, \\
2x+4y=2.
\end{cases}
$$

The second equation is exactly twice the first equation.

Therefore, both equations represent the same line.

There are infinitely many solutions. For example, we can express them as

$$
x=1-2y
$$

where $y$ can be any real number.

**4. Example with No Solution**

Now choose

$$
b=
\begin{pmatrix}
1 \\
0 \\
\end{pmatrix}
$$

The system becomes

$$
\begin{cases}
x+2y=1, \\
2x+4y=0.
\end{cases}
$$

Dividing the second equation by $2$ gives

$$
x+2y=0
$$

The two equations contradict each other because the same expression cannot equal both $1$ and $0$.

Therefore, this system has no solution.

**Final Answer**

The system has exactly one solution for every $b$ when

$$
k\neq2
$$

For $k=2$:

- If $b=(1,2)^T$, the system has infinitely many solutions.
- If $b=(1,0)^T$, the system has no solution.

This demonstrates that a zero determinant means the coefficient matrix is not invertible, so a unique solution for every right-hand side is not guaranteed.
