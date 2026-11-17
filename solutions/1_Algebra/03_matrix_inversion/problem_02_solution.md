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

**Solution**

**Part 1: Computing the Determinant**

For a general $2 \times 2$ matrix

$$
M =
\begin{pmatrix}
a & b \\
c & d
\end{pmatrix}
$$

the inverse exists if and only if $\det(M) = ad - bc \neq 0$, and is given by the formula:

$$
M^{-1} = \frac{1}{ad - bc}
\begin{pmatrix}
d & -b \\
-c & a
\end{pmatrix}
$$

First, compute the determinant of $A$:

$$
\det(A) = (3)(4) - (2)(5)
$$

$$
\det(A) = 12 - 10 = 2
$$

Since $\det(A) = 2 \neq 0$, the matrix $A$ is invertible.

**Part 2: Applying the $2 \times 2$ Inverse Formula**

Substitute $a = 3$, $b = 2$, $c = 5$, $d = 4$, and $\det(A) = 2$ into the formula:

$$
A^{-1} = \frac{1}{2}
\begin{pmatrix}
4 & -2 \\
-5 & 3
\end{pmatrix}
$$

Multiplying each entry inside the matrix by the scalar $\frac{1}{2}$:

$$
A^{-1} =
\begin{pmatrix}
\frac{4}{2} & \frac{-2}{2} \\
\frac{-5}{2} & \frac{3}{2}
\end{pmatrix}
$$

$$
A^{-1} =
\begin{pmatrix}
2 & -1 \\
-\frac{5}{2} & \frac{3}{2}
\end{pmatrix}
$$

**Part 3: Checking the Result**

To verify that $A^{-1}$ is indeed the inverse of $A$, we compute the product $A A^{-1}$ and confirm that it equals the $2 \times 2$ identity matrix $I_2$:

$$
A A^{-1} =
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
A A^{-1} =
\begin{pmatrix}
3(2) + 2\left(-\frac{5}{2}\right) & 3(-1) + 2\left(\frac{3}{2}\right) \\
5(2) + 4\left(-\frac{5}{2}\right) & 5(-1) + 4\left(\frac{3}{2}\right)
\end{pmatrix}
$$

$$
A A^{-1} =
\begin{pmatrix}
6 - 5 & -3 + 3 \\
10 - 10 & -5 + 6
\end{pmatrix}
$$

$$
A A^{-1} =
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}
= I_2
$$

Since $A A^{-1} = I_2$, the computed inverse is verified as correct.
