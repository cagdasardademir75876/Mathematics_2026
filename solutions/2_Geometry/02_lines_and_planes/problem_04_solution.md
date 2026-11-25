## Question

Find the equation of the plane through

$$A=(1,0,0),\quad B=(0,1,0),\quad C=(0,0,1).$$

First construct two vectors lying in the plane, and then use the cross product. Check the resulting equation on all three points.

## Solution

We form two direction vectors in the plane from $A$,
take their cross product to obtain a normal vector,
and substitute point $A$ to determine the plane equation.

### Vectors in the Plane and Cross Product

Compute two vectors lying in the plane:

$$u = B - A = (0 - 1,\, 1 - 0,\, 0 - 0) = (-1, 1, 0)$$

$$v = C - A = (0 - 1,\, 0 - 0,\, 1 - 0) = (-1, 0, 1)$$

Compute a normal vector using the cross product $n = u \times v$:

$$n = (-1, 1, 0) \times (-1, 0, 1)$$

$$n = \left( (1)(1) - (0)(0),\, (0)(-1) - (-1)(1),\, (-1)(0) - (1)(-1) \right)$$

$$n = (1, 1, 1)$$

### Equation of the Plane

Using $n = (1, 1, 1)$ and point $A = (1, 0, 0)$:

$$1(x - 1) + 1(y - 0) + 1(z - 0) = 0$$

$$x + y + z - 1 = 0$$

Equivalently:

$$x + y + z = 1$$

### Checking All Three Points

Substitute each point into $x + y + z - 1 = 0$:

- For $A = (1, 0, 0)$:

$$1 + 0 + 0 - 1 = 0$$

- For $B = (0, 1, 0)$:

$$0 + 1 + 0 - 1 = 0$$

- For $C = (0, 0, 1)$:

$$0 + 0 + 1 - 1 = 0$$

All three points satisfy the equation, confirming the plane.
