### Exercise 15. Classifying Three Systems

**Problem**

For each of the following systems, perform only as much elimination as necessary to recognize its type:

**System 1**

$$
\begin{cases}
x+y=2, \\
x-y=0,
\end{cases}
$$

**System 2**

$$
\begin{cases}
x+y=2, \\
2x+2y=4,
\end{cases}
$$

**System 3**

$$
\begin{cases}
x+y=2, \\
2x+2y=5.
\end{cases}
$$

For each, justify the classification: one solution, infinitely many solutions, or no solution.

**Solution**

**System 1: One Solution**

Augmented matrix:

$$
\left[
\begin{array}{cc|c}
1 & 1 & 2 \\
1 & -1 & 0
\end{array}
\right]
$$

Perform $R_2 \leftarrow R_2 - R_1$:

$$
\left[
\begin{array}{cc|c}
1 & 1 & 2 \\
0 & -2 & -2
\end{array}
\right]
$$

We can stop elimination here.
The system is already in row echelon form with $2$ unknowns
and $2$ non-zero pivot positions ($1$ and $-2$).
From $-2y = -2$, we get $y = 1$, and then $x = 1$.
Thus, System 1 has **one solution** (a unique solution).

**System 2: Infinitely Many Solutions**

Augmented matrix:

$$
\left[
\begin{array}{cc|c}
1 & 1 & 2 \\
2 & 2 & 4
\end{array}
\right]
$$

Perform $R_2 \leftarrow R_2 - 2R_1$:

$$
\left[
\begin{array}{cc|c}
1 & 1 & 2 \\
0 & 0 & 0
\end{array}
\right]
$$

We can stop here.
The second row is completely zeros ($0 = 0$),
so there is no contradiction (consistent system).
There are $2$ unknowns and only $1$ pivot column ($x$),
leaving $1$ free variable ($y = t$, $x = 2 - t$).
Thus, System 2 has **infinitely many solutions**.

**System 3: No Solution**

Augmented matrix:

$$
\left[
\begin{array}{cc|c}
1 & 1 & 2 \\
2 & 2 & 5
\end{array}
\right]
$$

Perform $R_2 \leftarrow R_2 - 2R_1$:

$$
\left[
\begin{array}{cc|c}
1 & 1 & 2 \\
0 & 0 & 1
\end{array}
\right]
$$

We can stop immediately.
The second row represents the equation $0x + 0y = 1$,
which simplifies to $0 = 1$.
This is a contradiction, so the system is inconsistent
and System 3 has **no solution**.
