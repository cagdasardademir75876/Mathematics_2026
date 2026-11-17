### Exercise 9. Matrix Equation

**Problem**

Given

$$
A=
\begin{pmatrix}
1 & 2 \\
0 & 1
\end{pmatrix}
$$

and

$$
B=
\begin{pmatrix}
3 & 1 \\
2 & 4
\end{pmatrix}.
$$

Solve the equation $AX=B$ for $X$. Before calculating, decide on which side of the equation $A^{-1}$ must be used. Then check the result by computing $AX$.

**Solution**

**Part 1: Deciding Which Side to Multiply by $A^{-1}$**

Because matrix multiplication is generally not commutative ($AB \neq BA$), the order of multiplication is critical. In the equation

$$
AX = B
$$

the matrix $A$ multiplies $X$ on the **left**. To isolate $X$, we must multiply both sides of the equation by $A^{-1}$ on the **left** as well:

$$
A^{-1}(AX) = A^{-1}B
$$

By the associative property of matrix multiplication, this simplifies to:

$$
(A^{-1}A)X = A^{-1}B
$$

$$
IX = A^{-1}B
$$

$$
X = A^{-1}B
$$

Note: Multiplying on the right would yield $AXA^{-1} = BA^{-1}$, which does not isolate $X$ because $A$ and $A^{-1}$ are separated by $X$.

**Part 2: Finding $A^{-1}$ and Solving for $X$**

First, compute the determinant of $A$:

$$
\det(A) = (1)(1) - (2)(0) = 1
$$

Since $\det(A) = 1 \neq 0$, $A$ is invertible. Applying the $2 \times 2$ inverse formula:

$$
A^{-1} = \frac{1}{1}
\begin{pmatrix}
1 & -2 \\
0 & 1
\end{pmatrix}
$$

$$
A^{-1} =
\begin{pmatrix}
1 & -2 \\
0 & 1
\end{pmatrix}
$$

Now substitute $A^{-1}$ and $B$ into $X = A^{-1}B$:

$$
X =
\begin{pmatrix}
1 & -2 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
3 & 1 \\
2 & 4
\end{pmatrix}
$$

Performing the matrix multiplication:

$$
X =
\begin{pmatrix}
1(3) + (-2)(2) & 1(1) + (-2)(4) \\
0(3) + 1(2) & 0(1) + 1(4)
\end{pmatrix}
$$

$$
X =
\begin{pmatrix}
3 - 4 & 1 - 8 \\
0 + 2 & 0 + 4
\end{pmatrix}
$$

$$
X =
\begin{pmatrix}
-1 & -7 \\
2 & 4
\end{pmatrix}
$$

**Part 3: Checking the Result by Computing $AX$**

To verify our solution, we substitute $X$ back into the original equation $AX = B$:

$$
AX =
\begin{pmatrix}
1 & 2 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
-1 & -7 \\
2 & 4
\end{pmatrix}
$$

$$
AX =
\begin{pmatrix}
1(-1) + 2(2) & 1(-7) + 2(4) \\
0(-1) + 1(2) & 0(-7) + 1(4)
\end{pmatrix}
$$

$$
AX =
\begin{pmatrix}
-1 + 4 & -7 + 8 \\
0 + 2 & 0 + 4
\end{pmatrix}
$$

$$
AX =
\begin{pmatrix}
3 & 1 \\
2 & 4
\end{pmatrix}
= B
$$

Since $AX = B$, the matrix $X$ is verified as correct.
