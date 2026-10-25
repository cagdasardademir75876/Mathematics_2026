### Exercise 6. Transpose

Given

$$
A=\begin{pmatrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
\end{pmatrix}
$$

and

$$
B=\begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3 \\
\end{pmatrix}
$$

---

#### 1. Transposes of Matrices $A$ and $B$

**Computation of $A^T$:**

$$
A^T = \begin{pmatrix}
1 & 4 \\
2 & 5 \\
3 & 6 \\
\end{pmatrix}
$$

**Computation of $B^T$:**

$$
B^T = \begin{pmatrix}
1 & 2 & -1 \\
0 & 1 & 3 \\
\end{pmatrix}
$$

---

#### 2. Computation of $AB$ and Its Transpose

**Computation of $AB$:**

$$
AB = \begin{pmatrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
\end{pmatrix}
\begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3 \\
\end{pmatrix}
$$

$$
AB = \begin{pmatrix}
1(1) + 2(2) + 3(-1) & 1(0) + 2(1) + 3(3) \\
4(1) + 5(2) + 6(-1) & 4(0) + 5(1) + 6(3) \\
\end{pmatrix}
= \begin{pmatrix}
2 & 11 \\
8 & 23 \\
\end{pmatrix}
$$

**Computation of $(AB)^T$:**

$$
(AB)^T = \begin{pmatrix}
2 & 8 \\
11 & 23 \\
\end{pmatrix}
$$

---

#### 3. Computation of $B^TA^T$ and Verification

**Computation of $B^TA^T$:**

$$
B^TA^T = \begin{pmatrix}
1 & 2 & -1 \\
0 & 1 & 3 \\
\end{pmatrix}
\begin{pmatrix}
1 & 4 \\
2 & 5 \\
3 & 6 \\
\end{pmatrix}
$$

$$
B^TA^T = \begin{pmatrix}
1(1) + 2(2) + (-1)(3) & 1(4) + 2(5) + (-1)(6) \\
0(1) + 1(2) + 3(3) & 0(4) + 1(5) + 3(6) \\
\end{pmatrix}
= \begin{pmatrix}
2 & 8 \\
11 & 23 \\
\end{pmatrix}
$$

**Verification:**

Comparing the results from the previous steps, we find that:

$$
(AB)^T = \begin{pmatrix}
2 & 8 \\
11 & 23 \\
\end{pmatrix}
= B^TA^T
$$

Thus, the property $(AB)^T = B^TA^T$ is successfully verified for this example.
