### Exercise 6. Transpose

**Problem**

For

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
\end{pmatrix}
\qquad
B=
\begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3 \\
\end{pmatrix}
$$

compute $A^T$, $B^T$, and $AB$. Then verify in this example that

$$
(AB)^T=B^TA^T.
$$

**Solution**

**Part 1: Computing Transposes $A^T$ and $B^T$**

The transpose of a matrix is obtained by swapping its rows and columns.

- For matrix $A$ (size $2 \times 3$), its transpose $A^T$ has size $3 \times 2$:

$$
A^T =
\begin{pmatrix}
1 & 4 \\
2 & 5 \\
3 & 6 \\
\end{pmatrix}
$$

- For matrix $B$ (size $3 \times 2$), its transpose $B^T$ has size $2 \times 3$:

$$
B^T =
\begin{pmatrix}
1 & 2 & -1 \\
0 & 1 & 3 \\
\end{pmatrix}
$$

**Part 2: Computing the Product $AB$**

The matrix $A$ has size $2 \times 3$ and $B$ has size $3 \times 2$, so their product $AB$ is defined and results in a $2 \times 2$ matrix:

$$
AB =
\begin{pmatrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
\end{pmatrix}
\begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3 \\
\end{pmatrix}
$$

Calculating the entries:

$$
AB =
\begin{pmatrix}
1(1) + 2(2) + 3(-1) & 1(0) + 2(1) + 3(3) \\
4(1) + 5(2) + 6(-1) & 4(0) + 5(1) + 6(3) \\
\end{pmatrix}
=
\begin{pmatrix}
1 + 4 - 3 & 0 + 2 + 9 \\
4 + 10 - 6 & 0 + 5 + 18 \\
\end{pmatrix}
=
\begin{pmatrix}
2 & 11 \\
8 & 23 \\
\end{pmatrix}
$$

**Part 3: Verifying $(AB)^T = B^TA^T$**

- First, compute the left-hand side, $(AB)^T$, by transposing the product $AB$:

$$
(AB)^T =
\begin{pmatrix}
2 & 11 \\
8 & 23 \\
\end{pmatrix}^T
=
\begin{pmatrix}
2 & 8 \\
11 & 23 \\
\end{pmatrix}
$$

- Next, compute the right-hand side, $B^TA^T$. The matrix $B^T$ has size $2 \times 3$ and $A^T$ has size $3 \times 2$, so their product is defined and results in a $2 \times 2$ matrix:

$$
B^TA^T =
\begin{pmatrix}
1 & 2 & -1 \\
0 & 1 & 3 \\
\end{pmatrix}
\begin{pmatrix}
1 & 4 \\
2 & 5 \\
3 & 6 \\
\end{pmatrix}
$$

Calculating the entries:

$$
B^TA^T =
\begin{pmatrix}
1(1) + 2(2) + (-1)(3) & 1(4) + 2(5) + (-1)(6) \\
0(1) + 1(2) + 3(3) & 0(4) + 1(5) + 3(6) \\
\end{pmatrix}
$$

Simplifying each entry:

$$
B^TA^T =
\begin{pmatrix}
1 + 4 - 3 & 4 + 10 - 6 \\
0 + 2 + 9 & 0 + 5 + 18 \\
\end{pmatrix}
=
\begin{pmatrix}
2 & 8 \\
11 & 23 \\
\end{pmatrix}
$$

Comparing both sides:

$$
(AB)^T =
\begin{pmatrix}
2 & 8 \\
11 & 23 \\
\end{pmatrix}
\qquad
\text{and}
\qquad
B^TA^T =
\begin{pmatrix}
2 & 8 \\
11 & 23 \\
\end{pmatrix}
$$

Thus, $(AB)^T = B^TA^T$ is successfully verified for this example.
