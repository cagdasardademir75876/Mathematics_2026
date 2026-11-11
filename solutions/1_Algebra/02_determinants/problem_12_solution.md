
### Exercise 12. A Parameter Revealed by a Row Operation

**Problem**

For

$$
A(t)=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 4 & t \\
0 & 1 & 1 \\
\end{pmatrix}
$$

find the values of $t$ for which the matrix is not invertible.

Before computing the determinant, perform the operation

$$
R_2\leftarrow R_2-2R_1
$$

and use the resulting structure. At the end, explain what special thing happens to the rows for the value of the parameter you found.

> **Why this exercise:** combines a parameter, row operations, and recognition of dependence in one short argument.

**Solution**

**1. Applying the Given Row Operation**

We start with

$$
A(t)=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 4 & t \\
0 & 1 & 1 \\
\end{pmatrix}
$$

Apply the required operation:

$$
R_2\leftarrow R_2-2R_1
$$

The second row becomes

$$
(2,4,t)-2(1,2,3)=(0,0,t-6)
$$

Therefore, the resulting matrix is

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 0 & t-6 \\
0 & 1 & 1 \\
\end{pmatrix}
$$

This operation does not change the determinant.

**2. Finding the Determinant**

The determinant can be calculated using the resulting matrix.

Expanding along the second row, which contains two zeros, gives

$$
\det(A(t))=-(t-6)
$$

Therefore,

$$
\det(A(t))=6-t
$$

The matrix is not invertible when its determinant is zero.

Set the determinant equal to zero:

$$
6-t=0
$$

Thus,

$$
t=6
$$

**3. Explaining the Dependence Between the Rows**

When $t=6$, the original matrix becomes

$$
A(6)=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 4 & 6 \\
0 & 1 & 1 \\
\end{pmatrix}
$$

The second row is twice the first row:

$$
R_2=2R_1
$$

Therefore, the rows are linearly dependent.

This explains why the determinant is zero and why the matrix is not invertible for this value of $t$.

**Final Answer**

The matrix is not invertible when

$$
t=6
$$

For this value, the second row is twice the first row, so the rows are linearly dependent and the determinant is zero.
