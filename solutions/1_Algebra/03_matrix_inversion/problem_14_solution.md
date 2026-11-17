### Exercise 14. A Matrix That Is Its Own Inverse

**Problem**

Assume that a square matrix $A$ satisfies

$$
A^2=I.
$$

Show that

$$
A^{-1}=A.
$$

Then give an example of a $2\times2$ matrix different from $I$ and $-I$ that satisfies this condition, and verify it by multiplication.

**Solution**

**Part 1: Proof that $A^{-1} = A$**

By definition, the inverse of a matrix $A$ is a matrix $A^{-1}$ such that:

$$
A A^{-1} = I \quad \text{and} \quad A^{-1} A = I
$$

We are given the matrix equation:

$$
A^2 = I
$$

By definition of matrix powers, $A^2$ can be written as:

$$
A \cdot A = I
$$

Comparing this equation $A \cdot A = I$ directly with the definition of the inverse $A \cdot A^{-1} = I$, it follows immediately that:

$$
A^{-1} = A
$$

*(Alternatively, multiplying both sides of $A^2 = I$ by $A^{-1}$ on the left yields $A^{-1}(A A) = A^{-1}I \implies (A^{-1}A)A = A^{-1} \implies I A = A^{-1} \implies A = A^{-1}$)*.

**Part 2: Example of a $2 \times 2$ Matrix Satisfying $A^2 = I$**

Consider the matrix:

$$
A =
\begin{pmatrix}
0 & 1 \\
1 & 0
\end{pmatrix}
$$

This matrix is clearly different from both the identity matrix $I = \begin{pmatrix} 1 & 0 \\ 0 & 1 \end{pmatrix}$ and its negative $-I = \begin{pmatrix} -1 & 0 \\ 0 & -1 \end{pmatrix}$.

**Part 3: Verification by Multiplication**

We compute $A^2$ by multiplying $A$ by itself:

$$
A^2 = A \cdot A =
\begin{pmatrix}
0 & 1 \\
1 & 0
\end{pmatrix}
\begin{pmatrix}
0 & 1 \\
1 & 0
\end{pmatrix}
$$

$$
A^2 =
\begin{pmatrix}
0(0) + 1(1) & 0(1) + 1(0) \\
1(0) + 0(1) & 1(1) + 0(0)
\end{pmatrix}
$$

$$
A^2 =
\begin{pmatrix}
0 + 1 & 0 + 0 \\
0 + 0 & 1 + 0
\end{pmatrix}
$$

$$
A^2 =
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}
= I
$$

Since $A^2 = I$, the matrix satisfies the given condition, and consequently $A^{-1} = A$.
