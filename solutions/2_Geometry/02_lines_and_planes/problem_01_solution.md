## Question

Find the equation of the line through $A=(1,2)$ and $B=(4,-1)$ in parametric and general form. Identify a direction vector and an example of a normal vector. Check that both points satisfy the equation you obtain.

## Solution

We construct a direction vector from $A$ to $B$,
write the parametric equations, eliminate the parameter $t$
to get the general form, and find a normal vector
perpendicular to the direction vector.

### Direction Vector and Parametric Form

A direction vector is given by:

$$
d = B - A = (4 - 1,\, -1 - 2) = (3, -3)
$$

Using point $A = (1, 2)$ and parameter $t \in \mathbb{R}$,
the parametric form is:

$$
\begin{cases}
x = 1 + 3t, \\
y = 2 - 3t.
\end{cases}
$$

### General Form and Normal Vector

From the first equation, solve for $t$:

$$
t = \frac{x - 1}{3}
$$

Substitute $t$ into the second equation:

$$
y = 2 - 3\left(\frac{x - 1}{3}\right)
$$

$$
y = 2 - (x - 1) = 3 - x
$$

Rearranging gives the general form:

$$
x + y - 3 = 0
$$

In general form $ax + by + c = 0$,
a normal vector is given by the coefficients $(a, b)$:

$$
n = (1, 1)
$$

We verify orthogonality using the dot product:

$$
d \cdot n = (3)(1) + (-3)(1) = 0
$$

### Verification for Points $A$ and $B$

Check $A = (1, 2)$ in $x + y - 3 = 0$:

$$
1 + 2 - 3 = 0
$$

Check $B = (4, -1)$ in $x + y - 3 = 0$:

$$
4 + (-1) - 3 = 0
$$

Both points satisfy the equation, confirming the result.
