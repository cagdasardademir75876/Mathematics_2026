### Exercise 6. Solving a System Using the Inverse

**Problem**

Solve

$$
Ax=b,
$$

where

$$
A=
\begin{pmatrix}
2 & 1 \\
1 & 3
\end{pmatrix}
$$

and

$$
b=
\begin{pmatrix}
5 \\
7
\end{pmatrix}
$$

using $x=A^{-1}b$. Then substitute the resulting vector back into the equation and check the result.

**Solution**

**Part 1: Finding the Inverse Matrix $A^{-1}$**

First, we compute the determinant of the $2 \times 2$ matrix $A$:

$$
\det(A) = (2)(3) - (1)(1)
$$

$$
\det(A) = 6 - 1 = 5
$$

Since $\det(A) = 5 \neq 0$, the inverse $A^{-1}$ exists and can be found using the $2 \times 2$ inverse formula:

$$
A^{-1} = \frac{1}{5}
\begin{pmatrix}
3 & -1 \\
-1 & 2
\end{pmatrix}
$$

**Part 2: Solving for $x$ Using $x = A^{-1}b$**

Multiply $A^{-1}$ on the right by the vector $b$:

$$
x = A^{-1}b = \frac{1}{5}
\begin{pmatrix}
3 & -1 \\
-1 & 2
\end{pmatrix}
\begin{pmatrix}
5 \\
7
\end{pmatrix}
$$

Performing the matrix-vector multiplication:

$$
x = \frac{1}{5}
\begin{pmatrix}
3(5) + (-1)(7) \\
(-1)(5) + 2(7)
\end{pmatrix}
$$

$$
x = \frac{1}{5}
\begin{pmatrix}
15 - 7 \\
-5 + 14
\end{pmatrix}
$$

$$
x = \frac{1}{5}
\begin{pmatrix}
8 \\
9
\end{pmatrix}
$$

Distributing the scalar $\frac{1}{5}$ gives the solution vector $x$:

$$
x =
\begin{pmatrix}
\frac{8}{5} \\
\frac{9}{5}
\end{pmatrix}
$$

**Part 3: Checking the Result by Substitution**

To verify our solution, we substitute $x$ back into the original equation $Ax = b$:

$$
Ax =
\begin{pmatrix}
2 & 1 \\
1 & 3
\end{pmatrix}
\begin{pmatrix}
\frac{8}{5} \\
\frac{9}{5}
\end{pmatrix}
$$

$$
Ax =
\begin{pmatrix}
2\left(\frac{8}{5}\right) + 1\left(\frac{9}{5}\right) \\
1\left(\frac{8}{5}\right) + 3\left(\frac{9}{5}\right)
\end{pmatrix}
$$

$$
Ax =
\begin{pmatrix}
\frac{16}{5} + \frac{9}{5} \\
\frac{8}{5} + \frac{27}{5}
\end{pmatrix}
$$

$$
Ax =
\begin{pmatrix}
\frac{25}{5} \\
\frac{35}{5}
\end{pmatrix}
$$

$$
Ax =
\begin{pmatrix}
5 \\
7
\end{pmatrix}
= b
$$

Since $Ax = b$, the solution vector $x$ is verified as correct.
