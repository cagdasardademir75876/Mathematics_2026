## Question

Compute:

1. the distance from $P=(2,3)$ to the line $3x+4y-10=0$,
2. the distance from $Q=(2,-1,3)$ to the plane $2x-2y+z-4=0$.

Compare the two formulas and explain their common connection with the normal direction.

## Solution

Both distances measure the perpendicular segment from a point
to a flat object (line or plane) along the normal vector,
obtained by projecting a connecting vector onto the unit normal.

### 1. Distance from $P=(2,3)$ to $3x+4y-10=0$

Here $a = 3$, $b = 4$, $c = -10$, and $(x_0, y_0) = (2, 3)$:

$$
d(P, L) = \frac{|ax_0 + by_0 + c|}{\sqrt{a^2 + b^2}}
$$

Substitute the values:

$$
d(P, L) = \frac{|3(2) + 4(3) - 10|}{\sqrt{3^2 + 4^2}}
$$

$$
d(P, L) = \frac{|6 + 12 - 10|}{\sqrt{9 + 16}}
= \frac{|8|}{\sqrt{25}} = \frac{8}{5}
$$

### 2. Distance from $Q=(2,-1,3)$ to $2x-2y+z-4=0$

Here $a = 2$, $b = -2$, $c = 1$, $d_0 = -4$,
and $(x_0, y_0, z_0) = (2, -1, 3)$:

$$
d(Q, \Pi) = \frac{|ax_0 + by_0 + cz_0 + d_0|}{\sqrt{a^2 + b^2 + c^2}}
$$

Substitute the values:

$$
d(Q, \Pi) = \frac{|2(2) - 2(-1) + 1(3) - 4|}{\sqrt{2^2 + (-2)^2 + 1^2}}
$$

$$
d(Q, \Pi) = \frac{|4 + 2 + 3 - 4|}{\sqrt{4 + 4 + 1}}
= \frac{|5|}{\sqrt{9}} = \frac{5}{3}
$$

### Comparison and Connection with the Normal Direction

- **Same structure in $\mathbb{R}^2$ and $\mathbb{R}^3$:**
  Both formulas take the absolute value of plugging the point
  into the implicit equation and divide by the norm
  of the normal vector ($\|(a, b)\|$ or $\|(a, b, c)\|$).
- **Normal vector mechanism:** If $R$ is any point on the
  line or plane, the vector $R - P$ projected onto
  the unit normal $\hat{n} = \frac{n}{\|n\|}$ has length
  $|(R - P) \cdot \hat{n}|$, which simplifies to the
  exact distance formula above.
