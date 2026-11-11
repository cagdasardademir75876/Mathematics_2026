### Exercise 7. Identity Matrix, Zero Matrix, and Powers

**Problem**

For

$$A= \begin{pmatrix} 2 & 1 \\ 0 & 2 \end{pmatrix}$$

compute

$$AI, \qquad IA, \qquad A+0, \qquad A^2, \qquad A^3.$$

Explain the roles of the matrices $I$ and $0$, and describe the pattern you observe in successive powers of $A$.

**Solution**

**Part 1: Basic Operations with Identity and Zero Matrices**

Let $I$ be the $2 \times 2$ identity matrix and $0$ be the $2 \times 2$ zero matrix:

$$I = \begin{pmatrix} 1 & 0 \\ 0 & 1 \end{pmatrix} \qquad 0 = \begin{pmatrix} 0 & 0 \\ 0 & 0 \end{pmatrix}$$

- Compute $AI$:

$$AI = \begin{pmatrix} 2 & 1 \\ 0 & 2 \end{pmatrix} \begin{pmatrix} 1 & 0 \\ 0 & 1 \end{pmatrix} = \begin{pmatrix} 2(1)+1(0) & 2(0)+1(1) \\ 0(1)+2(0) & 0(0)+2(1) \end{pmatrix}$$

$$AI = \begin{pmatrix} 2 & 1 \\ 0 & 2 \end{pmatrix}$$

- Compute $IA$:

$$IA = \begin{pmatrix} 1 & 0 \\ 0 & 1 \end{pmatrix} \begin{pmatrix} 2 & 1 \\ 0 & 2 \end{pmatrix} = \begin{pmatrix} 1(2)+0(0) & 1(1)+0(2) \\ 0(2)+1(0) & 0(1)+1(2) \end{pmatrix}$$

$$IA = \begin{pmatrix} 2 & 1 \\ 0 & 2 \end{pmatrix}$$

- Compute $A+0$:

$$A+0 = \begin{pmatrix} 2+0 & 1+0 \\ 0+0 & 2+0 \end{pmatrix} = \begin{pmatrix} 2 & 1 \\ 0 & 2 \end{pmatrix}$$

**Part 2: Matrix Powers $A^2$ and $A^3$**

- Compute $A^2 = A \cdot A$:

$$A^2 = \begin{pmatrix} 2 & 1 \\ 0 & 2 \end{pmatrix} \begin{pmatrix} 2 & 1 \\ 0 & 2 \end{pmatrix} = \begin{pmatrix} 2(2)+1(0) & 2(1)+1(2) \\ 0(2)+2(0) & 0(1)+2(2) \end{pmatrix}$$

$$A^2 = \begin{pmatrix} 4 & 4 \\ 0 & 4 \end{pmatrix}$$

- Compute $A^3 = A^2 \cdot A$:  $$
A^3 =
\begin{pmatrix}
4 & 4 \\
0 & 4
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
0 & 2
\end{pmatrix}
=
\begin{pmatrix}
4(2)+4(0) & 4(1)+4(2) \\
0(2)+4(0) & 0(1)+4(2)
\end{pmatrix}
$$  $$
A^3 =
\begin{pmatrix}
8 & 12 \\
0 &
