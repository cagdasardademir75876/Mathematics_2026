### Exercise 13. A Recurrence Written in Matrix Form

Given

$$F=\begin{pmatrix} 1 & 1 \\ 1 & 0 \\ \end{pmatrix}$$

---

#### 1. Computations of Matrix Powers

**Computation of $F^2$:**

$$F^2 = F \cdot F = \begin{pmatrix} 1 & 1 \\ 1 & 0 \\ \end{pmatrix} \begin{pmatrix} 1 & 1 \\ 1 & 0 \\ \end{pmatrix} = \begin{pmatrix} 1(1) + 1(1) & 1(1) + 1(0) \\ 1(1) + 0(1) & 1(1) + 0(0) \\ \end{pmatrix} = \begin{pmatrix} 2 & 1 \\ 1 & 1 \\ \end{pmatrix}$$

**Computation of $F^3$:**

$$F^3 = F^2 \cdot F = \begin{pmatrix} 2 & 1 \\ 1 & 1 \\ \end{pmatrix} \begin{pmatrix} 1 & 1 \\ 1 & 0 \\ \end{pmatrix} = \begin{pmatrix} 2(1) + 1(1) & 2(1) + 1(0) \\ 1(1) + 1(1) & 1(1) + 1(0) \\ \end{pmatrix} = \begin{pmatrix} 3 & 2 \\ 2 & 1 \\ \end{pmatrix}$$

**Computation of $F^4$:**

$$F^4 = F^3 \cdot F = \begin{pmatrix} 3 & 2 \\ 2 & 1 \\ \end{pmatrix} \begin{pmatrix} 1 & 1 \\ 1 & 0 \\ \end{pmatrix} = \begin{pmatrix} 3(1) + 2(1) & 3(1) + 2(0) \\ 2(1) + 1(1) & 2(1) + 1(0) \\ \end{pmatrix} = \begin{pmatrix} 5 & 3 \\ 3 & 2 \\ \end{pmatrix}$$

**Computation of $F^5$:**

$$F^5 = F^4 \cdot F = \begin{pmatrix} 5 & 3 \\ 3 & 2 \\ \end{pmatrix} \begin{pmatrix} 1 & 1 \\ 1 & 0 \\ \end{pmatrix} = \begin{pmatrix} 5(1) + 3(1) & 5(1) + 3(0) \\ 3(1) + 2(1) & 3(1) + 2(0) \\ \end{pmatrix} = \begin{pmatrix} 8 & 5 \\ 5 & 3 \\ \end{pmatrix}$$

---

#### 2. Relationship with the Fibonacci Sequence

The given sequence is the Fibonacci sequence $(f_n)_{n \ge 0}$:

$$f_0 = 0,\quad f_1 = 1,\quad f_2 = 1,\quad f_3 = 2,\quad f_4 = 3,\quad f_5 = 5,\quad f_6 = 8,\quad \ldots$$

Comparing the entries of the matrix powers with the Fibonacci numbers:

* $F^1 = \begin{pmatrix} 1 & 1 \\ 1 & 0 \end{pmatrix} = \begin{pmatrix} f_2 & f_1 \\ f_1 & f_0 \end{pmatrix}$
* $F^2 = \begin{pmatrix} 2 & 1 \\ 1 & 1 \end{pmatrix} = \begin{pmatrix} f_3 & f_2 \\ f_2 & f_1 \end{pmatrix}$
* $F^3 = \begin{pmatrix} 3 & 2 \\ 2 & 1 \end{pmatrix} = \begin{pmatrix} f_4 & f_3 \\ f_3 & f_2 \end{pmatrix}$
* $F^4 = \begin{pmatrix} 5 & 3 \\ 3 & 2 \end{pmatrix} = \begin{pmatrix} f_5 & f_4 \\ f_4 & f_3 \end{pmatrix}$
* $F^5 = \begin{pmatrix} 8 & 5 \\ 5 & 3 \end{pmatrix} = \begin{pmatrix} f_6 & f_5 \\ f_5 & f_4 \end{pmatrix}$

**Observation:**
For any positive integer $n \ge 1$, the power $F^n$ contains consecutive terms of the Fibonacci sequence:

$$F^n = \begin{pmatrix} f_{n+1} & f_n \\ f_n & f_{n-1} \\ \end{pmatrix}$$

---

#### 3. Recurrence Step Interpretation

**Computation:**

$$F\begin{pmatrix} a \\ b \end{pmatrix} = \begin{pmatrix} 1 & 1 \\ 1 & 0 \end{pmatrix} \begin{pmatrix} a \\ b \end{pmatrix} = \begin{pmatrix} 1(a) + 1(b) \\ 1(a) + 0(b) \end{pmatrix} = \begin{pmatrix} a+b \\ a \end{pmatrix}$$

**Explanation:**
If $\begin{pmatrix} a \\ b \end{pmatrix}$ holds two consecutive terms of a sequence, say $\begin{pmatrix} f_k \\ f_{k-1} \end{pmatrix}$, multiplying by $F$ yields
