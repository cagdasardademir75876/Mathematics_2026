### Exercise 6. A System with a Parameter — Which Cases Actually Occur?

**Problem**

Analyze, depending on the parameter $a$, the system

$$
\begin{cases}
x+y=2, \\
ax+ay=4.
\end{cases}
$$

Among the three possibilities — exactly one solution, infinitely many solutions, no solution — determine which actually occur and for which values of $a$. If one type cannot occur, explain why.

**Solution**

**Part 1: Augmented Matrix and Elimination**

Write the augmented matrix of the system:

$$
\left[
\begin{array}{cc|c}
1 & 1 & 2 \\
a & a & 4
\end{array}
\right]
$$

Perform the row operation $R_2 \leftarrow R_2 - aR_1$:

$$
\left[
\begin{array}{cc|c}
1 & 1 & 2 \\
0 & 0 & 4 - 2a
\end{array}
\right]
$$

The reduced second row corresponds to the equation:

$$
0x + 0y = 4 - 2a
$$

which simplifies to:

$$
0 = 4 - 2a
$$

**Part 2: Case Analysis by Parameter $a$**

- **Case 1:** $a = 2$

Substitute $a = 2$ into the simplified second equation:

$$
0 = 4 - 2(2) = 0
$$

The second equation is always satisfied ($0 = 0$).
The system reduces to the single independent equation $x + y = 2$.
Setting $y = t$ ($t \in \mathbb{R}$) gives $x = 2 - t$.
Therefore, for $a = 2$, the system has **infinitely many solutions**.

- **Case 2:** $a \neq 2$

When $a \neq 2$, the right-hand side of the second equation satisfies:

$$
4 - 2a \neq 0
$$

Thus, the second row gives the contradictory statement:

$$
0 = 4 - 2a \quad (\text{where } 4 - 2a \neq 0)
$$

which is impossible for any $x$ and $y$.
Therefore, for all $a \neq 2$, the system has **no solution** (it is inconsistent).

**Part 3: Which Cases Actually Occur and Why One Cannot**

- **Infinitely many solutions:** Occurs when $a = 2$.
- **No solution:** Occurs when $a \neq 2$.
- **Exactly one solution:** Cannot occur for any value of $a$.

**Why a unique solution is impossible:**

In the given system, the left-hand side of the second equation is always a scalar multiple ($a$ times) of the first equation:

$$
ax + ay = a(x + y)
$$

Thus, the coefficient matrix always has rank at most $1$, because its determinant is identically zero:

$$
\det(A) = (1)(a) - (1)(a) = 0
$$

Because the two equations never have linearly independent left-hand sides, their lines in the $xy$-plane are either **parallel and distinct** ($a \neq 2$, no intersection) or **coincident** ($a = 2$, infinitely many intersections).
They can never intersect at a single point.
