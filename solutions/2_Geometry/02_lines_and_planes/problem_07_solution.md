## Question

For

$$
L:(x,y,z)=(1,1,0)+t(1,-1,0),\qquad \Pi:x+y+z=2,
$$

determine whether the line intersects the plane at one point, is parallel to it, or lies in it. Explain the role of the dot product of the direction vector and the normal vector.

## Solution

We take the dot product of the line's direction vector
and the plane's normal vector to check whether the line
is parallel to the plane, and then test a point of $L$ in $\Pi$.

### Dot Product of Direction and Normal Vectors

From $L$ and $\Pi$:

- Direction vector of $L$: $d = (1, -1, 0)$
- Normal vector of $\Pi$: $n = (1, 1, 1)$

Compute the dot product $d \cdot n$:

$$
d \cdot n = (1)(1) + (-1)(1) + (0)(1) = 1 - 1 + 0 = 0
$$

Because $d \cdot n = 0$, the direction vector $d$
is perpendicular to the normal vector $n$,
which means $L$ is **parallel to** (or lies inside) $\Pi$.

### Testing Whether $L$ Lies in $\Pi$

Take the base point $P_0 = (1, 1, 0)$ on $L$
and substitute it into the equation of $\Pi$:

$$
x + y + z = 1 + 1 + 0 = 2
$$

Since $2 = 2$, the point $P_0$ satisfies the plane equation.
Because $L$ has direction parallel to $\Pi$ and contains
a point of $\Pi$, the entire line **lies in** $\Pi$.

### Role of the Dot Product $d \cdot n$

The dot product $d \cdot n$ measures how much
the line's direction points along the normal to the plane:

- If $d \cdot n \neq 0$, the line is not parallel to the normal's
  orthogonal complement, so it intersects $\Pi$ at **one point**.
- If $d \cdot n = 0$, the line is parallel to $\Pi$;
  we then check a single point of $L$ to distinguish
  between lying **in** $\Pi$ (point satisfies $\Pi$)
  and being strictly **parallel** to $\Pi$ (point does not satisfy $\Pi$).
