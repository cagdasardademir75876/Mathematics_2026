### Exercise 12. Formula for a Matrix Power

Given

$$A=\begin{pmatrix} 1 & 1 \\ 0 & 1 \\ \end{pmatrix}$$

---

#### 1. Computations of $A^2$, $A^3$, and $A^4$

**Computation of $A^2$:**

$$A^2 = A \cdot A = \begin{pmatrix} 1 & 1 \\ 0 & 1 \\ \end{pmatrix} \begin{pmatrix} 1 & 1 \\ 0 & 1 \\ \end{pmatrix} = \begin{pmatrix} 1(1) + 1(0) & 1(1) + 1(1) \\ 0(1) + 1(0) & 0(1) + 1(1) \\ \end{pmatrix} = \begin{pmatrix} 1 & 2 \\ 0 & 1 \\ \end{pmatrix}$$

**Computation of $A^3$:**

$$A^3 = A^2 \cdot A = \begin{pmatrix} 1 & 2 \\ 0 & 1 \\ \end{pmatrix} \begin{pmatrix} 1 & 1 \\ 0 & 1 \\ \end{pmatrix} = \begin{pmatrix} 1(1) + 2(0) & 1(1) + 2(1) \\ 0(1) + 1(0) & 0(1) + 1(1) \\ \end{pmatrix} = \begin{pmatrix} 1 & 3 \\ 0 & 1 \\ \end{pmatrix}$$

**Computation of $A^4$:**

$$A^4 = A^3 \cdot A = \begin{pmatrix} 1 & 3 \\ 0 & 1 \\ \end{pmatrix} \begin{pmatrix} 1 & 1 \\ 0 & 1 \\ \end{pmatrix} = \begin{pmatrix} 1(1) + 3(0) & 1(1) + 3(1) \\ 0(1) + 1(0) & 0(1) + 1(1) \\ \end{pmatrix} = \begin{pmatrix} 1 & 4 \\ 0 & 1 \\ \end{pmatrix}$$

---

#### 2. Conjecture for $A^n$

Based on the pattern observed in the powers:
* $A^1 = \begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix}$
* $A^2 = \begin{pmatrix} 1 & 2 \\ 0 & 1 \end{pmatrix}$
* $A^3 = \begin{pmatrix} 1 & 3 \\ 0 & 1 \end{pmatrix}$
* $A^4 = \begin{pmatrix} 1 & 4 \\ 0 & 1 \end{pmatrix}$

We conjecture that for any positive integer $n \ge 1$:

$$A^n = \begin{pmatrix} 1 & n \\ 0 & 1 \\ \end{pmatrix}$$

---

#### 3. Mathematical Induction Proof (Inductive Step)

**Base Step:**
For $n = 1$, $A^1 = \begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix}$, which matches the formula.

**Inductive Hypothesis:**
Assume the formula holds for a positive integer $n$, i.e.,

$$A^n = \begin{pmatrix} 1 & n \\ 0 & 1 \\ \end{pmatrix}$$

**Inductive Step:**
We compute $A^{n+1}$by multiplying$A^n$by$A$:  $$
A^{n+1} = A^n \cdot A = \begin{pmatrix}
1 & n \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}
$$  $$
A^{n+1} = \begin{pmatrix}
1(1) + n(0) & 1(1) + n(1) \\
0(1) + 1(0) & 0(1) + 1(1) \\
\end{pmatrix}
= \begin{pmatrix}
1 & n
