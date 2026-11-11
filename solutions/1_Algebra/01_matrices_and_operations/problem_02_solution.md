### Exercise 2. Addition and Scalar Multiplication

**Problem**

For

$$
A=
\begin{pmatrix}
1 & 2 \\
-1 & 3 \\
\end{pmatrix}
\qquad
B=
\begin{pmatrix}
4 & -2 \\
0 & 5 \\
\end{pmatrix}
$$

compute

$$
A+B, \qquad A-B, \qquad 3A-2B.
$$

Explain why matrix addition is possible only for matrices of the same size.

**Solution**

**Part 1: Matrix Operations**

- Compute $A+B$:

$$
A+B =
\begin{pmatrix}
1+4 & 2+(-2) \\
-1+0 & 3+5 \\
\end{pmatrix}
=
\begin{pmatrix}
5 & 0 \\
-1 & 8 \\
\end{pmatrix}
$$

- Compute $A-B$:

$$
A-B =
\begin{pmatrix}
1-4 & 2-(-2) \\
-1-0 & 3-5 \\
\end{pmatrix}
=
\begin{pmatrix}
-3 & 4 \\
-1 & -2 \\
\end{pmatrix}
$$

- Compute $3A-2B$:

First, calculate the scalar multiples $3A$ and $2B$:

$$
3A =
\begin{pmatrix}
3(1) & 3(2) \\
3(-1) & 3(3) \\
\end{pmatrix}
=
\begin{pmatrix}
3 & 6 \\
-3 & 9 \\
\end{pmatrix}
$$

$$
2B =
\begin{pmatrix}
2(4) & 2(-2) \\
2(0) & 2(5) \\
\end{pmatrix}
=
\begin{pmatrix}
8 & -4 \\
0 & 10 \\
\end{pmatrix}
$$

Subtract $2B$ from $3A$:

$$
3A-2B =
\begin{pmatrix}
3-8 & 6-(-4) \\
-3-0 & 9-10 \\
\end{pmatrix}
=
\begin{pmatrix}
-5 & 10 \\
-3 & -1 \\
\end{pmatrix}
$$

**Part 2: Compatibility Requirement for Addition**

Matrix addition is defined entry-by-entry, meaning that the entry in row $i$ and column $j$ of the sum matrix is obtained by adding the corresponding entry $a_{ij}$ of the first matrix to $b_{ij}$ of the second matrix. 

If two matrices have different dimensions, at least one entry in one matrix will not have a corresponding entry in the other matrix. Therefore, matrix addition is defined only when both matrices have the exact same size (the same number of rows and columns).
