### Exercise 5. Matrix Times Vector

Given

$$
A=\begin{pmatrix}
2 & -1 \\
1 & 3 \\
\end{pmatrix}
$$

and

$$
x=\begin{pmatrix}
4 \\
2 \\
\end{pmatrix}
$$

---

#### 1. Computation of $Ax$

$$
Ax = \begin{pmatrix}
2 & -1 \\
1 & 3 \\
\end{pmatrix}
\begin{pmatrix}
4 \\
2 \\
\end{pmatrix}
= \begin{pmatrix}
2(4) + (-1)(2) \\
1(4) + 3(2) \\
\end{pmatrix}
= \begin{pmatrix}
8 - 2 \\
4 + 6 \\
\end{pmatrix}
= \begin{pmatrix}
6 \\
10 \\
\end{pmatrix}
$$

---

#### 2. Linear Combination of Columns

Let the columns of matrix $A$ be denoted as $c_1$ and $c_2$:

$$
c_1 = \begin{pmatrix}
2 \\
1 \\
\end{pmatrix}, \qquad c_2 = \begin{pmatrix}
-1 \\
3 \\
\end{pmatrix}
$$

The entries of the vector $x$ serve as the scalar coefficients. Multiplying a matrix by a vector can be interpreted as a linear combination of the columns of the matrix:

$$
Ax = 4c_1 + 2c_2
$$

$$
Ax = 4\begin{pmatrix}
2 \\
1 \\
\end{pmatrix} + 2\begin{pmatrix}
-1 \\
3 \\
\end{pmatrix}
$$

$$
Ax = \begin{pmatrix}
8 \\
4 \\
\end{pmatrix} + \begin{pmatrix}
-2 \\
6 \\
\end{pmatrix}
= \begin{pmatrix}
6 \\
10 \\
\end{pmatrix}
$$
