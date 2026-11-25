## Question

Find the intersection point of

$$
(x,y,z)=(1,0,2)+t(1,2,-1)
$$

with the plane $x+y+z=4$. Check the result by substituting it into both descriptions.

## Solution

We write the parametric coordinates of the line,
substitute them into the plane equation to solve for $t$,
and plug that parameter back into the line equation.

### Finding the Parameter $t$ and Intersection Point

The parametric equations of the line are:

$$
\begin{cases}
x = 1 + t, \\
y = 2t, \\
z = 2 - t.
\end{cases}
$$

Substitute these into $x + y + z = 4$:

$$
(1 + t) + (2t) + (2 - t) = 4
$$

Combine like terms:

$$
(1 + 2) + (1 + 2 - 1)t = 4
$$

$$
3 + 2t = 4
$$

Solve for $t$:

$$
2t = 1 \implies t = \frac{1}{2}
$$

Substitute $t = \frac{1}{2}$ back into the line equation:

$$
P = \left(1, 0, 2\right) + \frac{1}{2}(1, 2, -1)
$$

$$
P = \left(1 + \frac{1}{2},\, 0 + 1,\, 2 - \frac{1}{2}\right)
= \left(\frac{3}{2},\, 1,\, \frac{3}{2}\right)
$$

### Checking in Both Descriptions

- **In the line equation:** Setting $t = \frac{1}{2}$ in
  $(1, 0, 2) + t(1, 2, -1)$ directly gives
  $\left(\frac{3}{2}, 1, \frac{3}{2}\right)$.
- **In the plane equation $x + y + z = 4$:**

$$
\frac{3}{2} + 1 + \frac{3}{2} = 3 + 1 = 4
$$

The point $\left(\frac{3}{2}, 1, \frac{3}{2}\right)$
satisfies both descriptions.
