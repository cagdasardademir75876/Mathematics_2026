### Exercise 10. Columns of a Matrix Product

**Problem**

Given

$$
A=
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1
\end{pmatrix}
$$

and

$$
B=
\begin{pmatrix}
1 & 2 \\
-1 & 0 \\
3 & 1
\end{pmatrix}
$$

Denote the columns of $B$ by $b_1,b_2$.

1. Compute $Ab_1$ and $Ab_2$.
2. Compute the matrix $AB$.
3. Compare the results and explain why the columns of $AB$ are exactly the vectors $Ab_1$ and $Ab_2$.

**Solution**

**Part 1: Computing $Ab_1$ and $Ab_2$**

Let the columns of $B$ be denoted as $b_1$ and $b_2$:

$$
b_1 =
\begin{pmatrix}
1 \\
-1 \\
3
\end{pmatrix}
\qquad
b_2 =
\begin{pmatrix}
2 \\
0 \\
1
\end{pmatrix}
$$

- Compute $Ab_1$:

$$
Ab_1 =
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1
\end{pmatrix}
\begin{pmatrix}
1 \\
-1 \\
3
\end{pmatrix}
=
\begin{pmatrix}
1(1) + 2(-1) + 0(3) \\
0(1) + 1(-1) + 1(3)
\end{pmatrix}
$$

$$
Ab_1 =
\begin{pmatrix}
1 - 2 + 0 \\
0 - 1 + 3
\end{pmatrix}
=
\begin{pmatrix}
-1 \\
2
\end{pmatrix}
$$

- Compute $Ab_2$:

$$
Ab_2 =
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1
\end{pmatrix}
\begin{pmatrix}
2 \\
0 \\
1
\end{pmatrix}
=
\begin{pmatrix}
1(2) + 2(0) + 0(1) \\
0(2) + 1(0) + 1(1)
\end{pmatrix}
$$

$$
Ab_2 =
\begin{pmatrix}
2 + 0 + 0 \\
0 + 0 + 1
\end{pmatrix}
=
\begin{pmatrix}
2 \\
1
\end{pmatrix}
$$

**Part 2: Computing the Matrix Product $AB$**

Multiply matrix $A$ (size $2 \times 3$) by matrix $B$ (size $3 \times 2$) to obtain a $2 \times 2$ matrix:

$$
AB =
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 2 \\
-1 & 0 \\
3 & 1
\end{pmatrix}
$$

Calculating the entries:

$$
AB =
\begin{pmatrix}
1(1) + 2(-1) + 0(3) & 1(2) + 2(0) + 0(1) \\
0(1) + 1(-1) + 1(3) & 0(2) + 1(0) + 1(1)
\end{pmatrix}
$$

Simplifying each entry:

$$
AB =
\begin{pmatrix}
1 - 2 + 0 & 2 + 0 + 0 \\
0 - 1 + 3 & 0 + 0 + 1
\end{pmatrix}
=
\begin{pmatrix}
-1 & 2 \\
2 & 1
\end{pmatrix}
$$

**Part 3: Comparison and Explanation**

Comparing the results:

$$
AB =
\begin{pmatrix}
-1 & 2 \\
2 & 1
\end{pmatrix}
\qquad
\text{where the columns are }
Ab_1 = \begin{pmatrix} -1 \\ 2 \end{pmatrix}
\text{ and }
Ab_2 = \begin{pmatrix} 2 \\ 1 \end{pmatrix}
$$

**Why the columns of $AB$ are $Ab_1$ and $Ab_2$:**

By definition of matrix multiplication, multiplying a matrix $A$ by another matrix $B = \begin{pmatrix} b_1 & b_2 \end{pmatrix}$ evaluates each column of the product by applying matrix $A$ to each individual column vector of $B$. Therefore, the $j$-th column of the product matrix $AB$ is precisely $A$ multiplied by the $j$-th column of $B$ (i.e., $Ab_j$).
