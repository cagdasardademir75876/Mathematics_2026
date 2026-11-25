### Exercise 9. A System from a Sum Condition

**Problem**

Find numbers $x,y$ satisfying

$$
x+y=10,\qquad 2x+5y=32.
$$

Solve the system and explain geometrically why the solution is unique.

**Solution**

**Part 1: Solving the System by Elimination**

Write the augmented matrix of the system:

$$
\left[
\begin{array}{cc|c}
1 & 1 & 10 \\
2 & 5 & 32
\end{array}
\right]
$$

- **Step 1:** Eliminate the entry below the first pivot using $R_2 \leftarrow R_2 - 2R_1$:

$$
\left[
\begin{array}{cc|c}
1 & 1 & 10 \\
0 & 3 & 12
\end{array}
\right]
$$

- **Step 2:** Scale row $2$ by $\frac{1}{3}$ ($R_2 \leftarrow \frac{1}{3}R_2$):

$$
\left[
\begin{array}{cc|c}
1 & 1 & 10 \\
0 & 1 & 4
\end{array}
\right]
$$

- **Step 3:** Back-substitute $y = 4$ into the first equation $x + y = 10$:

$$
x + 4 = 10
$$

$$
x = 6
$$

Thus, the unique solution is:

$$
x = 6, \qquad y = 4
$$

**Part 2: Geometric Explanation of Uniqueness**

Each linear equation in two variables represents a straight line in the $xy$-plane. Rewriting both equations in slope-intercept form ($y = mx + b$):

- First line:

$$
y = -x + 10 \qquad (\text{slope } m_1 = -1)
$$

- Second line:

$$
y = -\frac{2}{5}x + \frac{32}{5} \qquad (\text{slope } m_2 = -\frac{2}{5})
$$

Because the two lines have **different slopes** ($m_1 = -1 \neq -\frac{2}{5} = m_2$), they are not parallel and cannot coincide. In Euclidean geometry, any two non-parallel lines in a plane must intersect at **exact one point**, which here is $(6, 4)$.

---

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
