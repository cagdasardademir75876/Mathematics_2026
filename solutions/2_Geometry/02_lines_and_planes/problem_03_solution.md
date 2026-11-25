## Question

Find the equation of the plane through $P=(1,-2,3)$ and perpendicular to $n=(2,1,-1)$. Check the result by substituting the point $P$ and explain the role of the normal vector.

## Solution

A plane through $P = (x_0, y_0, z_0)$ perpendicular
to a normal vector $n = (a, b, c)$ consists of all points
$X = (x, y, z)$ such that the displacement vector
$X - P$ is orthogonal to $n$, meaning $n \cdot (X - P) = 0$.

### Constructing the Plane Equation

Using $P = (1, -2, 3)$, $X = (x, y, z)$,
and $n = (2, 1, -1)$:

$$
(2, 1, -1) \cdot (x - 1,\, y + 2,\, z - 3) = 0
$$

Expand the dot product:

$$
2(x - 1) + 1(y + 2) - 1(z - 3) = 0
$$

Distribute and simplify:

$$
2x - 2 + y + 2 - z + 3 = 0
$$

$$
2x + y - z + 3 = 0
$$

### Checking Point $P = (1, -2, 3)$

Substitute $x = 1$, $y = -2$, and $z = 3$
into the plane equation:

$$
2(1) + (-2) - (3) + 3 = 2 - 2 - 3 + 3 = 0
$$

The equation holds, so $P$ lies on the plane.

### Role of the Normal Vector

The normal vector $n = (2, 1, -1)$ fixes the
**orientation (tilt)** of the plane in $\mathbb{R}^3$:

- Every vector lying in the plane is perpendicular
  to $n$, so its dot product with $n$ is $0$.
- The components $(2, 1, -1)$ appear directly
  as the coefficients of $x$, $y$, and $z$
  in the linear equation $2x + y - z + 3 = 0$.
- Shifting the plane parallel to itself keeps
  the same normal vector $n$ and only changes
  the constant term.
