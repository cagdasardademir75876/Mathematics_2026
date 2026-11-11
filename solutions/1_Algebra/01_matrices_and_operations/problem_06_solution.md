### Exercise 6. Transpose

**Problem**

For

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
4 & 5 & 6
\end{pmatrix}
$$

and

$$
B=
\begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3
\end{pmatrix}
$$

compute $A^T$, $B^T$, and $AB$. Then verify in this example that

$$
(AB)^T=B^TA^T.
$$

**Solution**

**Part 1: Computing Transposes $A^T$ and $B^T$**

The transpose of a matrix is obtained by swapping its rows and columns.

- For matrix $A$, its transpose $A^T$ is:

$$
A^T =
\begin{pmatrix}
1 & 4 \\
2 & 5 \\
3 & 6
\end{pmatrix}
$$

- For matrix $B$, its transpose $B^T$ is:

$$
B^T =
\begin{pmatrix}
1 & 2 & -1 \\
0 & 1 & 3
\end{pmatrix}
$$

**Part 2: Computing the Product $AB$**

Multiply matrix $A$ by matrix $B$:

$$
AB =
\begin{pmatrix}
1 & 2 & 3 \\
4 & 5 & 6
\end{pmatrix}
\begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3
\end{pmatrix}
$$

Calculating the entries step-by-step:

$$
AB =
\begin{pmatrix}
1(1) + 2(2) + 3(-1) & 1(0) + 2(1) + 3(3) \\
4(1) + 5(2) + 6(-1) & 4(0) + 5(1) + 6(3)
\end{pmatrix}
$$

Simplifying the entries:

$$
AB =
\begin{pmatrix}
1 + 4 - 3 & 0 + 2 + 9 \\
4 + 10 - 6 & 0 + 5 + 18
\end{pmatrix}
$$

Final product matrix $AB$:

$$
AB =
\begin{pmatrix}
2 & 11 \\
8 & 23
\end{pmatrix}
$$

**Part 3: Verifying $(AB)^T = B^TA^T$**

- Compute the left-hand side, $(AB)^T$:

$$
(AB)^T =
\begin{pmatrix}
2 & 11 \\
8 & 23
\end{pmatrix}^T
$$

$$
(AB)^T =
\begin{pmatrix}
2 & 8 \\
11 & 23
\end{pmatrix}
$$

- Compute the right-hand side, $B^TA^T$:

$$
B^TA^T =
\begin{pmatrix}
1 & 2 & -1 \\
0 & 1 & 3
\end{pmatrix}
\begin{pmatrix}
1 & 4 \\
2 & 5 \\
3 & 6
\end{pmatrix}
$$

Calculating the product entries:

$$
B^TA^T =
\begin{pmatrix}
1(1) + 2(2) + (-1)(3) & 1(4) + 2(5) + (-1)(6) \\
0(1) + 1(2) + 3(3) & 0(4) + 1(5) + 3(6)
\end{pmatrix}
$$

Simplifying the entries:

$$
B^TA^T =
\begin{pmatrix}
1 + 4 - 3 & 4 + 10 - 6 \\
0 + 2 + 9 & 0 + 5 + 18
\end{pmatrix}
$$

Final matrix $B^TA^T$:

$$
B^TA^T =
\begin{pmatrix}
2 & 8 \\
11 & 23
\end{pmatrix}
$$

Since both sides yield the exact same matrix, $(AB)^T = B^TA^T$ is verified.
