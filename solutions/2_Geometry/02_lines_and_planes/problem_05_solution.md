## Question

Analyze the position of

$$
L_1:(x,y,z)=(1,1,0)+t(1,2,1),
$$

$$
L_2:(x,y,z)=(2,0,1)+s(0,1,-1).
$$

If they intersect, give the intersection point. If not, determine whether they are parallel or skew. Justify the classification.

## Solution

We compare the direction vectors of $L_1$ and $L_2$
to check parallelism, and then test whether the two
parametric equations share a common point $(x, y, z)$.

### Checking Parallelism

From the given equations:

- Direction vector of $L_1$: $d_1 = (1, 2, 1)$
- Direction vector of $L_2$: $d_2 = (0, 1, -1)$

Since $d_2$ is not a scalar multiple of $d_1$
(the first coordinate of $d_2$ is $0$ while $d_1$ has $1$),
the lines are **not parallel**.

### Checking for an Intersection Point

Equate the coordinates of $L_1$ and $L_2$:

$$
\begin{cases}
1 + t = 2, \\
1 + 2t = s, \\
t = 1 - s.
\end{cases}
$$

From the first equation:

$$
1 + t = 2 \implies t = 1
$$

Substitute $t = 1$ into the third equation:

$$
1 = 1 - s \implies s = 0
$$

Now substitute $t = 1$ and $s = 0$ into the second equation:

$$
\text{Left side: } 1 + 2(1) = 3
$$

$$
\text{Right side: } 0
$$

Since $3 \neq 0$, there is no pair $(t, s)$
that satisfies all three equations simultaneously.

### Classification and Justification

Because the lines are **not parallel** and **do not intersect**
in $\mathbb{R}^3$, the lines $L_1$ and $L_2$ are **skew**.
