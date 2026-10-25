### Exercise 15. Associativity of Multiplication and Different Calculation Paths

Given

$$A=\begin{pmatrix} 1 & 2 & 0 \\ 0 & 1 & 1 \\ \end{pmatrix},\quad B=\begin{pmatrix} 1 & 0 \\ 2 & 1 \\ -1 & 3 \\ \end{pmatrix},\quad C=\begin{pmatrix} 2 & 1 \\ 0 & -1 \\ \end{pmatrix}$$

---

#### 1. Computation of $(AB)C$

**Step 1: Compute $AB$**

$$AB = \begin{pmatrix} 1 & 2 & 0 \\ 0 & 1 & 1 \\ \end{pmatrix} \begin{pmatrix} 1 & 0 \\ 2 & 1 \\ -1 & 3 \\ \end{pmatrix}$$

$$AB = \begin{pmatrix} 1(1) + 2(2) + 0(-1) & 1(0) + 2(1) + 0(3) \\ 0(1) + 1(2) + 1(-1) & 0(0) + 1(1) + 1(3) \\ \end{pmatrix} = \begin{pmatrix} 5 & 2 \\ 1 & 4 \\ \end{pmatrix}$$

**Step 2: Multiply by $C$ to get $(AB)C$**

$$(AB)C = \begin{pmatrix} 5 & 2 \\ 1 & 4 \\ \end{pmatrix} \begin{pmatrix} 2 & 1 \\ 0 & -1 \\ \end{pmatrix}$$

$$(AB)C = \begin{pmatrix} 5(2) + 2(0) & 5(1) + 2(-1) \\ 1(2) + 4(0) & 1(1) + 4(-1) \\ \end{pmatrix} = \begin{pmatrix} 10 & 3 \\ 2 & -3 \\ \end{pmatrix}$$

---

#### 2
