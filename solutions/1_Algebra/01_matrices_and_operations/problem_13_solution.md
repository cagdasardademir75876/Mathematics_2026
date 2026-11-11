### Exercise 13. A Recurrence Written in Matrix Form

**Problem**

Let

$$
F=
\begin{pmatrix}
1 & 1 \\
1 & 0
\end{pmatrix}
$$

Compute $F^2$, $F^3$, $F^4$, and $F^5$. Compare the numbers obtained with the sequence

$$
0, 1, 1, 2, 3, 5, 8, \ldots
$$

and describe the relationship you observe. Then compute

$$
F
\begin{pmatrix}
a \\
b
\end{pmatrix}
$$

and explain how this multiplication performs one recurrence step: it creates the sum of two consecutive terms and keeps one of them for the next step.

**Solution**

**Part 1: Computing Powers $F^2$, $F^3$, $F^4$, and $F^5$**

- Compute $F^2 = F \cdot F$:

$$
F^2 =
\begin{pmatrix}
1 & 1 \\
1 & 0
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
1 & 0
\end{pmatrix}
$$

$$
F^2 =
\begin{pmatrix}
1(1) + 1(1) & 1(1) + 1(0) \\
1(1) + 0(1) & 1(1) + 0(0)
\end{pmatrix}
$$

$$
F^2 =
\begin{pmatrix}
2 & 1 \\
1 & 1
\end{pmatrix}
$$

- Compute $F^3 = F^2 \cdot F$:

$$
F^3 =
\begin{pmatrix}
2 & 1 \\
1 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
1 & 0
\end{pmatrix}
$$

$$
F^3 =
\begin{pmatrix}
2(1) + 1(1) & 2(1) + 1(0) \\
1(1) + 1(1) & 1(1) + 1(0)
\end{pmatrix}
$$

$$
F^3 =
\begin{pmatrix}
3 & 2 \\
2 & 1
\end{pmatrix}
$$

- Compute $F^4 = F^3 \cdot F$:

$$
F^4 =
\begin{pmatrix}
3 & 2 \\
2 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
1 & 0
\end{pmatrix}
$$

$$
F^4 =
\begin{pmatrix}
3(1) + 2(1) & 3(1) + 2(0) \\
2(1) + 1(1) & 2(1) + 1(0)
\end{pmatrix}
$$

$$
F^4 =
\begin{pmatrix}
5 & 3 \\
3 & 2
\end{pmatrix}
$$

- Compute $F^5 = F^4 \cdot F$:

$$
F^5 =
\begin{pmatrix}
5 & 3 \\
3 & 2
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
1 & 0
\end{pmatrix}
$$

$$
F^5 =
\begin{pmatrix}
5(1) + 3(1) & 5(1) + 3(0) \\
3(1) + 2(1) & 3(1) + 2(0)
\end{pmatrix}
$$

$$
F^5 =
\begin{pmatrix}
8 & 5 \\
5 & 3
\end{pmatrix}
$$

**Part 2: Relationship with the Fibonacci Sequence**

Comparing the entries of the computed matrix powers with the given sequence $0, 1, 1, 2, 3, 5, 8, \ldots$ (which is the Fibonacci sequence $F_n$):

$$
F^1 = \begin{pmatrix} 1 & 1 \\ 1 & 0 \end{pmatrix}, \quad
F^2 = \begin{pmatrix} 2 & 1 \\ 1 & 1 \end{pmatrix}, \quad
F^3 = \begin{pmatrix} 3 & 2 \\ 2 & 1 \end{pmatrix}, \quad
F^4 = \begin{pmatrix} 5 & 3 \\ 3 & 2 \end{pmatrix}, \quad
F^5 = \begin{pmatrix} 8 & 5 \\ 5 & 3 \end{pmatrix}
$$

In general, the power $F^n$ contains consecutive Fibonacci numbers:

$$
F^n =
\begin{pmatrix}
F_{n+1} & F_n \\
F_n & F_{n-1}
\end{pmatrix}
$$

**Part 3: Matrix-Vector Product and Recurrence Step**

Compute the product of $F$ with an arbitrary vector $\begin{pmatrix} a \\ b \end{pmatrix}$:

$$
\begin{aligned}
F \begin{pmatrix} a \\ b \end{pmatrix} &=
\begin{pmatrix}
1 & 1 \\
1 & 0
\end{pmatrix}
\begin{pmatrix}
a \\
b
\end{pmatrix} \\
&=
\begin{pmatrix}
1(a) + 1(b) \\
1(a) + 0(b)
\end{pmatrix} \\
&=
\begin{pmatrix}
a + b \\
a
\end{pmatrix}
\end{aligned}
$$

**Explanation of the Recurrence Step:**

If we view $a$ and $b$ as two consecutive terms in a sequence (where $a$ is the current term and $b$ is the previous term), multiplying by matrix $F$ performs a single recurrence step:
- The top entry becomes $a + b$, which is the next term in the Fibonacci-like sequence (the sum of the two preceding terms).
- The bottom entry becomes $a$, which retains the current term so it can serve as the "previous" term in the subsequent step.
