### Exercise 9. Composing Transformations

**Problem**

Let

$$S= \begin{pmatrix} 2 & 0 \\ 0 & 1 \end{pmatrix}$$

and

$$R= \begin{pmatrix} 0 & -1 \\ 1 & 0 \end{pmatrix}$$

The matrix $S$ describes nonuniform scaling, while $R$ describes a $90^\circ$ counterclockwise rotation.
For

$$x= \begin{pmatrix} 1 \\ 2 \end{pmatrix}$$

compute $RSx$ and $SRx$. Compare the results and explain geometrically why the order of these transformations matters.

**Solution**

**Part 1: Computing $RSx$ and $SRx$**

- **Compute $RSx$ (Scale first, then Rotate):**

First, apply scaling $S$ to vector $x$:

$$Sx = \begin{pmatrix} 2 & 0 \\ 0 & 1 \end{pmatrix} \begin{pmatrix} 1 \\ 2 \end{pmatrix} = \begin{pmatrix} 2(1) + 0(2) \\ 0(1) + 1(2) \end{pmatrix} = \begin{pmatrix} 2 \\ 2 \end{pmatrix}$$

Next, apply rotation $R$ to the result $Sx$:

$$RSx = \begin{pmatrix} 0 & -1 \\ 1 & 0 \end{pmatrix} \begin{pmatrix} 2 \\ 2 \end{pmatrix} = \begin{pmatrix} 0(2) + (-1)(2) \\ 1(2) + 0(2) \end{pmatrix}$$

$$RSx = \begin{pmatrix} -2 \\ 2 \end{pmatrix}$$

- **Compute $SRx$ (Rotate first, then Scale):**

First, apply rotation $R$to vector$x$:  $$
Rx =
\begin{pmatrix}
0 & -1 \\
1 & 0
\end{pmatrix}
\begin{pmatrix}
1 \\
2
\
