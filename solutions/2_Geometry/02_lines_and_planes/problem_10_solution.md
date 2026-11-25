## Question

Find the orthogonal projection of $P=(2,1,3)$ onto the plane $x+y+z=3$, and then find the reflection of $P$ across this plane. Check that the midpoint of the segment joining the point and its reflection lies on the plane.

## Solution

We move from $P$ along the normal vector $n$ to the plane
until reaching the intersection point $P'$, which is the
orthogonal projection, and then continue the same step
to obtain the reflection $P^*$.

### Orthogonal Projection $P'$ onto $x+y+z=3$

The normal vector of $\Pi: x + y + z = 3$ is:

$$
n = (1, 1, 1)
$$

A line through $P = (2, 1, 3)$ perpendicular to $\Pi$ is:

$$
r(t) = (2, 1, 3) + t(1, 1, 1) = (2 + t,\, 1 + t,\, 3 + t)
$$

Substitute into $x + y + z = 3$:

$$
(2 + t) + (1 + t) + (3 + t) = 3
$$

$$
6 + 3t = 3 \implies 3t = -3 \implies t = -1
$$

Plug $t = -1$ back into $r(t)$ to get the projection $P'$:

$$
P' = (2 - 1,\, 1 - 1,\, 3 - 1) = (1, 0, 2)
$$

### Reflection $P^*$ Across the Plane

Since $P'$ is the midpoint of $P$ and $P^*$:

$$
P^* = P + 2(P' - P) = 2P' - P
$$

Compute $P^*$:

$$
P^* = 2(1, 0, 2) - (2, 1, 3)
$$

$$
P^* = (2 - 2,\, 0 - 1,\, 4 - 3) = (0, -1, 1)
$$

### Checking the Midpoint of $P$ and $P^*$

Compute the midpoint $M$ of $P = (2, 1, 3)$ and $P^* = (0, -1, 1)$:

$$
M = \left(
\frac{2 + 0}{2},\,
\frac{1 + (-1)}{2},\,
\frac{3 + 1}{2}
\right)
= (1, 0, 2)
$$

Substitute $M = (1, 0, 2)$ into the plane equation $x + y + z = 3$:

$$
1 + 0 + 2 = 3
$$

The midpoint lies on the plane (and equals $P'$),
confirming both the projection and the reflection.
