### Exercise 4. Matrix Multiplication and Noncommutativity

Given
$$
A=\begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix}
$$

and

$$
B=\begin{pmatrix}
2 & 0 \\
3 & 1 \\
\end{pmatrix}
$$

---

#### 1. Computations

**Computation of $AB$:**

$$
AB = \begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
2 & 0 \\
3 & 1 \\
\end{pmatrix}
$$

$$
AB = \begin{pmatrix}
1(2) + 2(3) & 1(0) + 2(1) \\
0(2) + 1(3) & 0(0) + 1(1) \\
\end{pmatrix}
= \begin{pmatrix}
8 & 2 \\
3 & 1 \\
\end{pmatrix}
$$

**Computation of $BA$:**

$$
BA = \begin{pmatrix}
2 & 0 \\
3 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix}
$$

$$
BA = \begin{pmatrix}
2(1) + 0(0) & 2(2) + 0(1) \\
3(1) + 1(0) & 3(2) + 1(1) \\
\end{pmatrix}
= \begin{pmatrix}
2 & 4 \\
3 & 7 \\
\end{pmatrix}
$$

---

#### 2. Analysis of Noncommutativity

Comparing the two results:

$$
AB = \begin{pmatrix} 8 & 2 \\ 3 & 1 \\\end{pmatrix} \neq \begin{pmatrix} 2 & 4 \\ 3 & 7 \\\end{pmatrix} = BA
$$

Therefore, $AB \neq BA$.

In real-number arithmetic, multiplication is commutative, meaning that the order of factors does not change the product ($a \cdot b = b \cdot a$). 

In contrast, matrix multiplication is **noncommutative**. This means that changing the order in which two matrices are multiplied generally produces a different result (or can even render the operation undefined due to incompatible dimensions). Consequently, the left-to-right order of matrices must be strictly preserved during calculations.
