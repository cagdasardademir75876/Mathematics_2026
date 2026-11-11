### Exercise 12. Formula for a Matrix Power

**Problem**

Let

$$
A=
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
$$

Compute $A^2$, $A^3$, and $A^4$, and use them to formulate a conjecture for $A^n$. Then do not stop after checking one more case: assume the formula is true for $n$, multiply by $A$, and explain why you obtain exactly the formula for $n+1$.

**Solution**

**Part 1: Computing Powers $A^2$, $A^3$, and $A^4$**

- Compute $A^2 = A \cdot A$:

$$
A^2 =
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
$$

$$
A^2 =
\begin{pmatrix}
1(1) + 1(0) & 1(1) + 1(1) \\
0(1) + 1(0) & 0(1) + 1(1)
\end{pmatrix}
$$

$$
A^2 =
\begin{pmatrix}
1 & 2 \\
0 & 1
\end{pmatrix}
$$

- Compute $A^3 = A^2 \cdot A$:

$$
A^3 =
\begin{pmatrix}
1 & 2 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
$$

$$
A^3 =
\begin{pmatrix}
1(1) + 2(0) & 1(1) + 2(1) \\
0(1) + 1(0) & 0(1) + 1(1)
\end{pmatrix}
$$

$$
A^3 =
\begin{pmatrix}
1 & 3 \\
0 & 1
\end{pmatrix}
$$

- Compute $A^4 = A^3 \cdot A$:

$$
A^4 =
\begin{pmatrix}
1 & 3 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
$$

$$
A^4 =
\begin{pmatrix}
1(1) + 3(0) & 1(1) + 3(1) \\
0(1) + 1(0) & 0(1) + 1(1)
\end{pmatrix}
$$

$$
A^4 =
\begin{pmatrix}
1 & 4 \\
0 & 1
\end{pmatrix}
$$

**Part 2: Conjecture for $A^n$**

Observing the computed powers:

$$
A^1 = \begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix}, \quad
A^2 = \begin{pmatrix} 1 & 2 \\ 0 & 1 \end{pmatrix}, \quad
A^3 = \begin{pmatrix} 1 & 3 \\ 0 & 1 \end{pmatrix}, \quad
A^4 = \begin{pmatrix} 1 & 4 \\ 0 & 1 \end{pmatrix}
$$

Based on this pattern, we formulate the conjecture for any positive integer $n$:

$$
A^n =
\begin{pmatrix}
1 & n \\
0 & 1
\end{pmatrix}
$$

**Part 3: Inductive Step (Proof by Induction-like Verification)**

Assume that the formula holds for some arbitrary integer $n$, meaning:

$$
A^n =
\begin{pmatrix}
1 & n \\
0 & 1
\end{pmatrix}
$$

To find $A^{n+1}$, we multiply $A^n$ by $A$:

$$
A^{n+1} = A^n \cdot A
$$

$$
A^{n+1} =
\begin{pmatrix}
1 & n \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
$$

Performing the matrix multiplication:

$$
A^{n+1} =
\begin{pmatrix}
1(1) + n(0) & 1(1) + n(1) \\
0(1) + 1(0) & 0(1) + 1(1)
\end{pmatrix}
$$

Simplifying the entries:

$$
A^{n+1} =
\begin{pmatrix}
1 & 1 + n \\
0 & 1
\end{pmatrix}
$$

$$
A^{n+1} =
\begin{pmatrix}
1 & n + 1 \\
0 & 1
\end{pmatrix}
$$

This resulting expression matches the conjectured formula for $A^n$ with $n$ replaced by $n+1$. Thus, assuming the formula holds for $n$ guarantees that it holds for $n+1$.
