### Exercise 7. Identity Matrix, Zero Matrix, and Powers

Given

$$
A=\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}
$$

---

#### 1. Computations

**Computation of $AI$ and $IA$:**

Let $I$ be the $2 \times 2$ identity matrix:

$$
I=\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
$$

$$
AI = \begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
= \begin{pmatrix}
2(1) + 1(0) & 2(0) + 1(1) \\
0(1) + 2(0) & 0(0) + 2(1) \\
\end{pmatrix}
= \begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix} = A
$$

$$
IA = \begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}
= \begin{pmatrix}
1(2) + 0(0) & 1(1) + 0(2) \\
0(2) + 1(0) & 0(1) + 1(2) \\
\end{pmatrix}
= \begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix} = A
$$

**Computation of $A+0$:**

Let $0$ be the $2 \times 2$ zero matrix:

$$
0=\begin{pmatrix}
0 & 0 \\
0 & 0 \\
\end{pmatrix}
$$

$$
A+0 = \begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}
+
\begin{pmatrix}
0 & 0 \\
0 & 0 \\
\end{pmatrix}
= \begin{pmatrix}
2+0 & 1+0 \\
0+0 & 2+0 \\
\end{pmatrix}
= \begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix} = A
$$

**Computation of $A^2$ and $A^3$:**

$$
A^2 = A \cdot A = \begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}
= \begin{pmatrix}
2(2) + 1(0) & 2(1) + 1(2) \\
0(2) + 2(0) & 0(1) + 2(2) \\
\end{pmatrix}
= \begin{pmatrix}
4 & 4 \\
0 & 4 \\
\end{pmatrix}
$$

$$
A^3 = A^2 \cdot A = \begin{pmatrix}
4 & 4 \\
0 & 4 \\
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}
= \begin{pmatrix}
4(2) + 4(0) & 4(1) + 4(2) \\
0(2) + 4(0) & 0(1) + 4(2) \\
\end{pmatrix}
= \begin{pmatrix}
8 & 12 \\
0 & 8 \\
\end{pmatrix}
$$

---

#### 2. Roles of Neutral Elements and Powers Pattern

* **Role of the Identity Matrix ($I$):** The identity matrix acts as the multiplicative neutral element. Multiplying any compatible matrix by $I$ leaves the matrix unchanged ($AI = IA = A$).
* **Role of the Zero Matrix ($0$):** The zero matrix acts as the additive neutral element. Adding the zero matrix to any matrix of the same size leaves the matrix unchanged ($A + 0 = A$).
* **Pattern in Successive Powers of $A$:**
  * For $A = \begin{pmatrix} 2 & 1 \\ 0 & 2 \end{pmatrix} = \begin{pmatrix} 2^1 & 1 \cdot 2^{0} \\ 0 & 2^1 \end{pmatrix}$
  * For $A^2 = \begin{pmatrix} 4 & 4 \\ 0 & 4 \end{pmatrix} = \begin{pmatrix} 2^2 & 2 \cdot 2^{1} \\ 0 & 2^2 \end{pmatrix}$
  * For $A^3 = \begin{pmatrix} 8 & 12 \\ 0 & 8 \end{pmatrix} = \begin{pmatrix} 2^3 & 3 \cdot 2^{2} \\ 0 & 2^3 \end{pmatrix}$
  
  In general, for any positive integer $n$, the power $A^n$ follows the pattern:
  $$
  A^n = \begin{pmatrix}
  2^n & n \cdot 2^{n-1} \\
  0 & 2^n \\
  \end{pmatrix}
  $$
