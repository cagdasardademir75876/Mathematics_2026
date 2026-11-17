
### Exercise 2. Formula for a 2×2 Matrix

**Problem**

Find the inverse of

$$
A=
\begin{pmatrix}
3 & 2 \\
5 & 4
\end{pmatrix}
$$

using the formula for a $2\times2$ matrix. At the end, check the result by computing one product with $A$.

> **Why this exercise:** teaches the simplest explicit formula for an inverse and requires verification using the definition.

**Solution**

For a $2\times2$ matrix

$$
A=
\begin{pmatrix}
a & b \\
c & d
\end{pmatrix}
$$

the inverse is given by

$$
A^{-1}
=
\frac{1}{ad-bc}
\begin{pmatrix}
d & -b \\
-c & a
\end{pmatrix}
$$

provided that the determinant is nonzero.

First, calculate the determinant of $A$:

$$
\det(A)=3\cdot4-2\cdot5
$$

$$
\det(A)=12-10=2
$$

Since $\det(A)=2\neq0$, the inverse exists.

Substitute the matrix entries into the inverse formula:

$$
A^{-1}
=
\frac{1}{2}
\begin{pmatrix}
4 & -2 \\
-5 & 3
\end{pmatrix}
$$

Therefore,

$$
A^{-1}
=
\begin{pmatrix}
2 & -1 \\
-\frac{5}{2} & \frac{3}{2}
\end{pmatrix}
$$

**Verification**

To verify the result, calculate $AA^{-1}$:

$$
AA^{-1}
=
\begin{pmatrix}
3 & 2 \\
5 & 4
\end{pmatrix}
\begin{pmatrix}
2 & -1 \\
-\frac{5}{2} & \frac{3}{2}
\end{pmatrix}
$$

$$
=
\begin{pmatrix}
3\cdot2+2\cdot\left(-\frac{5}{2}\right)
&
3\cdot(-1)+2\cdot\frac{3}{2}
\\
5\cdot2+4\cdot\left(-\frac{5}{2}\right)
&
5\cdot(-1)+4\cdot\frac{3}{2}
\end{pmatrix}
$$

$$
=
\begin{pmatrix}
6-5 & -3+3 \\
10-10 & -5+6
\end{pmatrix}
$$

$$
=
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}
=I
$$

Since the product $AA^{-1}$ equals the identity matrix, the result is verified.

**Final Answer**

$$
A^{-1}
=
\begin{pmatrix}
2 & -1 \\
-\frac{5}{2} & \frac{3}{2}
\end{pmatrix}
$$
