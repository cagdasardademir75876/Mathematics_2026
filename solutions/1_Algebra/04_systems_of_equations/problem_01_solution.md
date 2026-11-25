### Exercise 1. From a System to a Matrix

**Problem**

Write the system

$$
\begin{cases}
2x-y+z=4, \\
x+3y-2z=1, \\
3x+y+z=7.
\end{cases}
$$

in the form $Ax=b$.
Identify the coefficient matrix, the vector of unknowns, and the right-hand side vector. Explain how each row of the matrix corresponds to one equation.

**Solution**

**Part 1: Matrix Form $Ax = b$**

The given system of three linear equations in three unknowns ($x, y, z$) can be written as a single matrix equation $Ax = b$:

$$
\begin{pmatrix}
2 & -1 & 1 \\
1 & 3 & -2 \\
3 & 1 & 1
\end{pmatrix}
\begin{pmatrix}
x \\
y \\
z
\end{pmatrix}
=
\begin{pmatrix}
4 \\
1 \\
7
\end{pmatrix}
$$

**Part 2: Identifying the Matrix Components**

- **Coefficient Matrix ($A$):** Contains the numerical coefficients multiplying the variables, ordered consistently by variable columns ($x$, $y$, $z$):

$$
A =
\begin{pmatrix}
2 & -1 & 1 \\
1 & 3 & -2 \\
3 & 1 & 1
\end{pmatrix}
$$

- **Vector of Unknowns ($x$):** A column vector listing the unknown variables of the system in order:

$$
x =
\begin{pmatrix}
x \\
y \\
z
\end{pmatrix}
$$

- **Right-Hand Side Vector ($b$):** A column vector containing the constant terms on the right-hand side of each equation:

$$
b =
\begin{pmatrix}
4 \\
1 \\
7
\end{pmatrix}
$$

**Part 3: Correspondence Between Rows and Equations**

When performing the matrix-vector multiplication $Ax$, each row of the coefficient matrix $A$ takes the dot product with the column vector of unknowns $x$, and the result is set equal to the corresponding entry in the vector $b$:

- **Row 1:** Multiplying the first row by the vector of unknowns gives:

$$
\begin{pmatrix}
2 & -1 & 1
\end{pmatrix}
\begin{pmatrix}
x \\
y \\
z
\end{pmatrix}
= 2x - 1y + 1z
$$

Setting this equal to the first entry of $b$ recovers the first equation $2x - y + z = 4$.

- **Row 2:** Multiplying the second row by the vector of unknowns gives:

$$
\begin{pmatrix}
1 & 3 & -2
\end{pmatrix}
\begin{pmatrix}
x \\
y \\
z
\end{pmatrix}
= 1x + 3y - 2z
$$

Setting this equal to the second entry of $b$ recovers the second equation $x + 3y - 2z = 1$.

- **Row 3:** Multiplying the third row by the vector of unknowns gives:

$$
\begin{pmatrix}
3 & 1 & 1
\end{pmatrix}
\begin{pmatrix}
x \\
y \\
z
\end{pmatrix}
= 3x + 1y + 1z
$$

Setting this equal to the third entry of $b$ recovers the third equation $3x + y + z = 7$.

In short, the $i$-th row of $A$ records the coefficients of the $i$-th equation, while the $j$-th column of $A$ collects all coefficients belonging to the $j$-th variable across the system.
