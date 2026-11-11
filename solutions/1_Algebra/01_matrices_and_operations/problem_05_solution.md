### Exercise 5. Matrix Times Vector

**Problem**

Let

$$
A=
\begin{pmatrix}
2 & -1 \\
1 & 3 \\
\end{pmatrix}
\qquad
x=
\begin{pmatrix}
4 \\
2 \\
\end{pmatrix}
$$

Compute $Ax$. Then express $Ax$ as a linear combination of the columns of $A$, with coefficients coming from the vector $x$.

**Solution**

**Part 1: Computing $Ax$**

Compute the matrix-vector product by multiplying each row of $A$ by the vector $x$:

$$
Ax =
\begin{pmatrix}
2 & -1 \\
1 & 3 \\
\end{pmatrix}
\begin{pmatrix}
4 \\
2 \\
\end{pmatrix}
=
\begin{pmatrix}
2(4) + (-1)(2) \\
1(4) + 3(2) \\
\end{pmatrix}
=
\begin{pmatrix}
8 - 2 \\
4 + 6 \\
\end{pmatrix}
=
\begin{pmatrix}
6 \\
10 \\
\end{pmatrix}
$$

**Part 2: Linear Combination of Column Vectors**

A matrix-vector product $Ax$ can also be interpreted as a linear combination of the columns of $A$, where the scalar coefficients are the entries of the vector $x$.

Let the columns of $A$ be denoted as $c_1$ and $c_2$:

$$
c_1 = 
\begin{pmatrix}
2 \\
1 \\
\end{pmatrix}
\qquad
c_2 = 
\begin{pmatrix}
-1 \\
3 \\
\end{pmatrix}
$$

Using the entries of $x = \begin{pmatrix} 4 \\ 2 \end{pmatrix}$ as coefficients, the product $Ax$ is expressed as:

$$
Ax = 4 c_1 + 2 c_2
$$

Substituting the column vectors:

$$
Ax = 4
\begin{pmatrix}
2 \\
1 \\
\end{pmatrix}
+
2
\begin{pmatrix}
-1 \\
3 \\
\end{pmatrix}
=
\begin{pmatrix}
8 \\
4 \\
\end{pmatrix}
+
\begin{pmatrix}
-2 \\
6 \\
\end{pmatrix}
=
\begin{pmatrix}
6 \\
10 \\
\end{pmatrix}
$$

Both methods yield the same resulting vector.
