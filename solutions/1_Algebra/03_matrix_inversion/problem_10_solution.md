### Exercise 10. Inverse of a Diagonal Matrix

**Problem**

Given

$$
D=
\begin{pmatrix}
2 & 0 & 0 \\
0 & -3 & 0 \\
0 & 0 & 5
\end{pmatrix}
$$

and

$$
E=
\begin{pmatrix}
2 & 0 & 0 \\
0 & 0 & 0 \\
0 & 0 & 5
\end{pmatrix}.
$$

Without using Gauss–Jordan elimination, decide which matrix is invertible. For the invertible matrix, give the inverse and check the result by multiplication.

**Solution**

**Part 1: Determining Invertibility**

A diagonal matrix is invertible if and only if **all** of its main diagonal entries are non-zero. The determinant of a diagonal matrix is simply the product of its diagonal elements:

- For matrix $D$:
  The diagonal entries are $2$, $-3$, and $5$. The determinant is:
  $$
  \det(D) = (2)(-3)(5) = -30 \neq 0
  $$
  Since $\det(D) \neq 0$, matrix $D$ is **invertible**.

- For matrix $E$:
  The diagonal entries are $2$, $0$, and $5$. The determinant is:
  $$
  \det(E) = (2)(0)(5) = 0
  $$
  Since $\det(E) = 0$, matrix $E$ is **not invertible** (singular).

**Part 2: Finding the Inverse of $D$**

For any invertible diagonal matrix, the inverse is obtained by simply taking the reciprocal of each entry along the main diagonal. Therefore, the inverse of $D$ is:

$$
D^{-1} =
\begin{pmatrix}
\frac{1}{2} & 0 & 0 \\
0 & -\frac{1}{3} & 0 \\
0 & 0 & \frac{1}{5}
\end{pmatrix}
$$

**Part 3: Checking the Result by Multiplication**

We verify our result by computing the product $D D^{-1}$ to confirm that it yields the $3 \times 3$ identity matrix $I_3$:

$$
D D^{-1} =
\begin{pmatrix}
2 & 0 & 0 \\
0 & -3 & 0 \\
0 & 0 & 5
\end{pmatrix}
\begin{pmatrix}
\frac{1}{2} & 0 & 0 \\
0 & -\frac{1}{3} & 0 \\
0 & 0 & \frac{1}{5}
\end{pmatrix}
$$

$$
D D^{-1} =
\begin{pmatrix}
2\left(\frac{1}{2}\right) & 0 & 0 \\
0 & (-3)\left(-\frac{1}{3}\right) & 0 \\
0 & 0 & 5\left(\frac{1}{5}\right)
\end{pmatrix}
$$

$$
D D^{-1} =
\begin{pmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{pmatrix}
= I_3
$$

Since $D D^{-1} = I_3$, the computed inverse is verified as correct.
