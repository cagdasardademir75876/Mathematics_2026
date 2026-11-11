### Exercise 15. Associativity of Multiplication and Different Calculation Paths

**Problem**

Given

$$A= \begin{pmatrix} 1 & 2 & 0 \\ 0 & 1 & 1 \end{pmatrix}, \quad B= \begin{pmatrix} 1 & 0 \\ 2 & 1 \\ -1 & 3 \end{pmatrix}, \quad C= \begin{pmatrix} 2 & 1 \\ 0 & -1 \end{pmatrix}$$

Compute $(AB)C$ and $A(BC)$. Compare the results and the number of intermediate operations. Explain what associativity of matrix multiplication means in this example.

**Solution**

**Part 1: Computing Path 1 — $(AB)C$**

- Step 1.1: Compute $AB$ (size $2 \times 3$ times $3 \times 2$, resulting in a $2 \times 2$ matrix):

$$AB = \begin{pmatrix} 1 & 2 & 0 \\ 0 & 1 & 1 \end{pmatrix} \begin{pmatrix} 1 & 0 \\ 2 & 1 \\ -1 & 3 \end{pmatrix}$$

$$AB = \begin{pmatrix} 1(1) + 2(2) + 0(-1) & 1(0) + 2(1) + 0(3) \\ 0(1) + 1(2) + 1(-1) & 0(0) + 1(1) + 1(3) \end{pmatrix}$$

$$AB = \begin{pmatrix} 1 + 4 + 0 & 0 + 2 + 0 \\ 0 + 2 - 1 & 0 + 1 + 3 \end{pmatrix}$$

$$AB = \begin{pmatrix} 5 & 2 \\ 1 & 4 \end{pmatrix}$$

- Step 1.2: Compute $(AB)C$ by multiplying the resulting matrix $AB$ by $C$ (size $2 \times 2$ times $2 \times 2$):

$$(AB)C = \begin{pmatrix} 5 & 2 \\ 1 & 4 \end{pmatrix} \begin{pmatrix} 2 & 1 \\ 0 & -1 \end{pmatrix}$$

$$(AB)C = \begin{pmatrix} 5(2) + 2(0) & 5(1) + 2(-1) \\ 1(2) + 4(0) & 1(1) + 4(-1) \end{pmatrix}$$

$$(AB)C = \begin{pmatrix} 10 + 0 & 5 - 2 \\ 2 + 0 & 1 - 4 \end{pmatrix}$$

$$(AB)C = \begin{pmatrix} 10 & 3 \\ 2 & -3 \end{pmatrix}$$

**Part 2: Computing Path 2 — $A(BC)$**

- Step 2.1: Compute $BC$ (size $3 \times 2$ times $2 \times 2$, resulting in a $3 \times 2$ matrix):

$$BC = \begin{pmatrix} 1 & 0 \\ 2 & 1 \\ -1 & 3 \end{pmatrix} \begin{pmatrix} 2 & 1 \\ 0 & -1 \end{pmatrix}$$

$$BC = \begin{pmatrix} 1(2) + 0(0) & 1(1) + 0(-1) \\ 2(2) + 1(0) & 2(1) + 1(-1) \\ -1(2) + 3(0) & -1(1) + 3(-1) \end{pmatrix}$$

$$BC = \begin{pmatrix} 2 + 0 & 1 + 0 \\ 4 + 0 & 2 - 1 \\ -2 + 0 & -1 - 3 \end{pmatrix}$$

$$BC = \begin{pmatrix} 2 & 1 \\ 4 & 1 \\ -2 & -4 \end{pmatrix}$$

- Step 2.2: Compute $A(BC)$ by multiplying matrix $A$ by the resulting matrix $BC$ (size $2 \times 3$ times $3 \times 2$, resulting in a $2 \times 2$ matrix):

$$A(BC) = \begin{pmatrix} 1 & 2 & 0 \\ 0 & 1 & 1 \end{pmatrix} \begin{pmatrix} 2 & 1 \\ 4 & 1 \\ -2 & -4 \end{pmatrix}$$

$$A(BC) = \begin{pmatrix} 1(2) + 2(4) + 0(-2) & 1(1) + 2(1) + 0(-4) \\ 0(2) + 1(4) + 1(-2) & 0(1) + 1(1) + 1(-4) \end{pmatrix}$$

$$A(BC) = \begin{pmatrix} 2 + 8 + 0 & 1 + 2 + 0 \\ 0 + 4 - 2 & 0 + 1 - 4 \end{pmatrix}$$

$$A(BC) = \begin{pmatrix} 10 & 3 \\ 2 & -3 \end{pmatrix}$$

**Part 3: Comparison of Results and Operations**

- **Results Comparison:** 
  Both calculation paths yield the exact same final matrix:
  $$(AB)C = A(BC) = \begin{pmatrix} 10 & 3 \\ 2 & -3 \end{pmatrix}$$

- **Comparison of Intermediate Operations (Computational Complexity):**
  - **Path 1 ($(AB)C$):** We first multiply a $(2 \times 3)$ matrix by a $(3 \times 2)$ matrix (requiring $2 \times 2 \times 3 = 12$ scalar multiplications), then multiply the resulting $(2 \times 2)$ matrix by another $(2 \times 2)$ matrix (requiring $2 \times 2 \times 2 = 8$ scalar multiplications), totaling **
