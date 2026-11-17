### Exercise 11. Parameter and Invertibility

**Problem**

For

$$
A(t)=
\begin{pmatrix}
1 & t \\
t & 1
\end{pmatrix}
$$

find all $t$ for which the matrix is invertible, and then give a formula for $A(t)^{-1}$. Explain what happens to this formula at the excluded values.

**Solution**

**Part 1: Finding Values of $t$ for Which the Matrix is Invertible**

A square matrix is invertible if and only if its determinant is non-zero. First, we compute the determinant of $A(t)$:

$$
\det(A(t)) = (1)(1) - (t)(t)
$$

$$
\det(A(t)) = 1 - t^2
$$

The matrix $A(t)$ is invertible when $\det(A(t)) \neq 0$:

$$
1 - t^2 \neq 0
$$

$$
t^2 \neq 1
$$

$$
t \neq 1 \quad \text{and} \quad t \neq -1
$$

Therefore, the matrix $A(t)$ is invertible for all real numbers $t$ except **$t = 1$ and $t = -1$** (i.e., $t \in \mathbb{R} \setminus \{-1, 1\}$).

**Part 2: Formula for $A(t)^{-1}$**

Using the explicit inverse formula for a $2 \times 2$ matrix, we divide by the determinant $\det(A(t)) = 1 - t^2$ and swap/negate the appropriate entries:

$$
A(t)^{-1} = \frac{1}{1 - t^2}
\begin{pmatrix}
1 & -t \\
-t & 1
\end{pmatrix}
$$

Distributing the scalar $\frac{1}{1 - t^2}$ across the matrix entries, the inverse can also be written as:

$$
A(t)^{-1} =
\begin{pmatrix}
\frac{1}{1 - t^2} & -\frac{t}{1 - t^2} \\
-\frac{t}{1 - t^2} & \frac{1}{1 - t^2}
\end{pmatrix}
$$

**Part 3: What Happens at the Excluded Values ($t = 1$ and $t = -1$)**

At the excluded values $t = 1$ and $t = -1$:

- The determinant becomes $\det(A(\pm 1)) = 1 - (\pm 1)^2 = 0$.
- In the formula for $A(t)^{-1}$, this results in division by zero (e.g., terms like $\frac{1}{1 - t^2}$ become undefined).
- Geometrically and algebraically, the matrix becomes **singular** (non-invertible) because when $t = 1$ or $t = -1$, the two rows of the matrix become linearly dependent (either identical or exact scalar multiples of each other), meaning the transformation collapses dimensions and cannot be undone.
