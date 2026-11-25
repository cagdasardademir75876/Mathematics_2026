## Question

Given

$$
\Pi_1:x+y+z=1,\qquad \Pi_2:x-y=2.
$$

First use the normal vectors to decide whether the planes are parallel. If not, compute the angle between them and explain why the normal vectors alone are enough for this calculation.

## Solution

We extract the normal vectors from the plane equations,
test whether one is a scalar multiple of the other,
and use the dot product and vector norms to find the angle.

### Normal Vectors and Parallelism Check

Reading the coefficients of $x, y, z$:

- Normal vector of $\Pi_1$: $n_1 = (1, 1, 1)$
- Normal vector of $\Pi_2$: $n_2 = (1, -1, 0)$

Since there is no scalar $k$ such that $n_2 = k n_1$
(for instance, $1 \cdot k = 1 \implies k = 1$,
but $1 \cdot 1 = 1 \neq -1$),
the normal vectors are not parallel,
so the planes $\Pi_1$ and $\Pi_2$ are **not parallel**.

### Angle Between the Planes

Compute the dot product $n_1 \cdot n_2$:

$$
n_1 \cdot n_2 = (1)(1) + (1)(-1) + (1)(0) = 0
$$

Compute the lengths (norms) of $n_1$ and $n_2$:

$$
\|n_1\| = \sqrt{1^2 + 1^2 + 1^2} = \sqrt{3}
$$

$$
\|n_2\| = \sqrt{1^2 + (-1)^2 + 0^2} = \sqrt{2}
$$

Using the angle formula between the normals:

$$
\cos\theta = \frac{|n_1 \cdot n_2|}{\|n_1\|\,\|n_2\|}
= \frac{0}{\sqrt{3}\,\sqrt{2}} = 0
$$

Thus, the angle between the planes is:

$$
\theta = 90^\circ \quad \left(\text{or } \frac{\pi}{2}\right)
$$

### Why Normal Vectors Alone Are Enough

Each plane is uniquely determined up to translation
by its normal direction:

- Rotating a plane in space rotates its normal vector
  by the exact same angle.
- Therefore, the angle between two intersecting planes
  equals the acute (or right) angle between their
  normal vectors, without needing to find their
  line of intersection.
