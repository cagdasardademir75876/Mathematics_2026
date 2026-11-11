### Exercise 4. Matrix Multiplication and Noncommutativity

**Problem**

For

$$
A=
\begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix}
\qquad
B=
\begin{pmatrix}
2 & 0 \\
3 & 1 \\
\end{pmatrix}
$$

compute $AB$ and $BA$. Is $AB=BA$? Use this example to explain what noncommutativity of matrix multiplication means.

**Solution**

**Part 1: Computing $AB$ and $BA$**

- Compute the product $AB$:

$$
AB =
\begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
2 & 0 \\
3 & 1 \\
\end{pmatrix}
=
\begin{pmatrix}
1(2) + 2(3) & 1(0) + 2(1) \\
0(2) + 1(3) & 0(0) + 1(1) \\
\end{pmatrix}
=
\begin{pmatrix}
8 & 2 \\
3 & 1 \\
\end{pmatrix}
$$

- Compute the product $BA$:

$$
BA =
\begin{pmatrix}
2 & 0 \\
3 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix}
=
\begin{pmatrix}
2(1) + 0(0) & 2(2) + 0(1) \\
3(1) + 1(0) & 3(2) + 1(1) \\
\end{pmatrix}
=
\begin{pmatrix}
2 & 4 \\
3 & 7 \\
\end{pmatrix}
$$

**Part 2: Comparison ($AB$ versus $BA$)**

Comparing the resulting matrices:

$$
AB =
\begin{pmatrix}
8 & 2 \\
3 & 1 \\
\end{pmatrix}
\quad \neq \quad
BA =
\begin{pmatrix}
2 & 4 \\
3 & 7 \\
\end{pmatrix}
$$

Therefore, $AB \neq BA$.

**Part 3: Explanation of Noncommutativity**

In ordinary arithmetic for real numbers, multiplication is commutative, meaning that $ab = ba$ for any two numbers $a$ and $b$. 

As demonstrated by this example, matrix multiplication does not generally possess this property. The noncommutativity of matrix multiplication means that changing the order of the factors in a matrix product alters the final result. Even when both products $AB$ and $BA$ are well-defined and have the same dimensions, they are not guaranteed to be equal.
