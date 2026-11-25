### Exercise 10. A Polynomial Through Three Points

**Problem**

Find a polynomial $p(x)=ax^2+bx+c$ whose graph passes through $(0,1)$, $(1,3)$, and $(2,9)$. Reduce the problem to a system of equations and check the result by substituting all three points.

**Solution**

**Part 1: Reducing the Problem to a Linear System**

For the graph of $p(x) = ax^2 + bx + c$ to pass through a point $(x_i, y_i)$, the coefficients $a, b, c$ must satisfy $p(x_i) = y_i$:

- Point $(0, 1)$ gives $p(0) = 1$:

$$
a(0)^2 + b(0) + c = 1
$$

$$
c = 1
$$

- Point $(1, 3)$ gives $p(1) = 3$:

$$
a(1)^2 + b(1) + c = 3
$$

$$
a + b + c = 3
$$

- Point $(2, 9)$ gives $p(2) = 9$:

$$
a(2)^2 + b(2) + c = 9
$$

$$
4a + 2b + c = 9
$$

This yields a system of three linear equations in the unknown coefficients $a, b, c$:

$$
\begin{cases}
c = 1, \\
a + b + c = 3, \\
4a + 2b + c = 9.
\end{cases}
$$

**Part 2: Solving the System**

From the first equation, we immediately have:

$$
c = 1
$$

Substitute $c = 1$ into the remaining two equations:

$$
\begin{cases}
a + b + 1 = 3, \\
4a + 2b + 1 = 9.
\end{cases}
$$

Simplifying gives:

$$
\begin{cases}
a + b = 2, \\
4a + 2b = 8.
\end{cases}
$$

Divide the second equation by $2$:

$$
2a + b = 4
$$

Subtract $a + b = 2$ from $2a + b = 4$:

$$
(2a + b) - (a + b) = 4 - 2
$$

$$
a = 2
$$

Substitute $a = 2$ back into $a + b = 2$:

$$
2 + b = 2
$$

$$
b = 0
$$

Thus, the coefficients are $a = 2$, $b = 0$, and $c = 1$, giving the quadratic polynomial:

$$
p(x) = 2x^2 + 1
$$

**Part 3: Verification by Substituting All Three Points**

- Check $(0, 1)$:

$$
p(0) = 2(0)^2 + 1 = 0 + 1 = 1
$$

- Check $(1, 3)$:

$$
p(1) = 2(1)^2 + 1 = 2 + 1 = 3
$$

- Check $(2, 9)$:

$$
p(2) = 2(2)^2 + 1 = 8 + 1 = 9
$$

All three points lie on the graph of $p(x) = 2x^2 + 1$, confirming the result.
