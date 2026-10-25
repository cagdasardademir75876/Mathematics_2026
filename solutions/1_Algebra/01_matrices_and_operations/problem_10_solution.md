### Exercise 10. Columns of a Matrix Product

Given

$$
A=\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1 \\
\end{pmatrix},\qquad B=\begin{pmatrix}
1 & 2 \\
-1 & 0 \\
3 & 1 \\
\end{pmatrix}
$$

The columns of matrix $B$ are:

$$
b_1 = \begin{pmatrix}
1 \\
-1 \\
3 \\
\end{pmatrix}, \qquad b_2 = \begin{pmatrix}
2 \\
0 \\
1 \\
\end{pmatrix}
$$

---

#### 1. Computations of $Ab_1$ and $Ab_2$

**Computation of $Ab_1$:**

$$
Ab_1 = \begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 \\
-1 \\
3 \\
\end{pmatrix}
= \begin{pmatrix}
1(1) + 2(-1) + 0(3) \\
0(1) + 1(-1) + 1(3) \\
\end{pmatrix}
= \begin{pmatrix}
1 - 2 + 0 \\
0 - 1 + 3 \\
\end{pmatrix}
= \begin{pmatrix}
-1 \\
2 \\
\end{pmatrix}
$$

**Computation of $Ab_2$:**

$$
Ab_2 = \begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1 \\
\end{pmatrix}
\begin{pmatrix}
2 \\
0 \\
1 \\
\end{pmatrix}
= \begin{pmatrix}
1(2) + 2(0) + 0(1) \\
0(2) + 1(0) + 1(1) \\
\end{pmatrix}
= \begin{pmatrix}
2 + 0 + 0 \\
0 + 0 + 1 \\
\end{pmatrix}
= \begin{pmatrix}
2 \\
1 \\
\end{pmatrix}
$$

---

#### 2. Computation of $AB$

$$
AB = \begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 & 2 \\
-1 & 0 \\
3 & 1 \\
\end{pmatrix}
$$

$$
AB = \begin{pmatrix}
1(1) + 2(-1) + 0(3) & 1(2) + 2(0) + 0(1) \\
0(1) + 1(-1) + 1(3) & 0(2) + 1(0) + 1(1) \\
\end{pmatrix}
= \begin{pmatrix}
-1 & 2 \\
2 & 1 \\
\end{pmatrix}
$$

---

#### 3. Comparison and Explanation

Comparing the computed matrix $AB$ with the individual products $Ab_1$ and $Ab_2$:

$$
AB = \begin{pmatrix}
-1 & 2 \\
2 & 1 \\
\end{pmatrix}
= \begin{pmatrix}
Ab_1 & \mid & Ab_2 \\
\end{pmatrix}
$$

**Explanation:**

Matrix multiplication $AB$ acts by multiplying the left matrix $A$ separately onto each column vector of the right matrix $B$. 

If $B$ is written in terms of its columns as $B = \begin{pmatrix} b_1 & b_2 \end{pmatrix}$, then applying matrix multiplication gives:

$$
AB = A\begin{pmatrix} b_1 & b_2 \end{pmatrix} = \begin{pmatrix} Ab_1 & Ab_2 \end{pmatrix}
$$

Thus, the $j$-th column of the product matrix $AB$ is always equal to $A$ multiplied by the $j$-th column of $B$.
