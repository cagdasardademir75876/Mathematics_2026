### Exercise 3. Swapping Two Rows

**Problem**

For

$$
A=
\begin{pmatrix}
1 & 2 & 0 \\
0 & 3 & 1 \\
2 & 1 & 1
\end{pmatrix}
$$

compute $\det A$. Then form a matrix $B$ by swapping the first and second rows of $A$.

First predict $\det B$ using a determinant property, and then verify your prediction by calculation.

**Solution**

**Part 1: Computing $\det A$**

We can compute the determinant of $A$ by expanding along the first row:

$$
\det(A) = 1 \cdot
\begin{vmatrix}
3 & 1 \\
1 & 1
\end{vmatrix}
- 2 \cdot
\begin{vmatrix}
0 & 1 \\
2 & 1
\end{vmatrix}
+ 0 \cdot
\begin{vmatrix}
0 & 3 \\
2 & 1
\end{vmatrix}
$$

Calculating the $2 \times 2$ determinants:

$$
\det(A) = 1 \cdot ((3)(1) - (1)(1)) - 2 \cdot ((0)(1) - (1)(2)) + 0
$$

$$
\det(A) = 1 \cdot (3 - 1) - 2 \cdot (0 - 2)
$$

$$
\det(A) = 1(2) - 2(-2) = 2 + 4 = 6
$$

Thus, $\det(A) = 6$.

**Part 2: Forming Matrix $B$ and Predicting $\det B$**

Matrix $B$ is formed by swapping the first and second rows of matrix $A$ ($R_1 \leftrightarrow R_2$):

$$
B =
\begin{pmatrix}
0 & 3 & 1 \\
1 & 2 & 0 \\
2 & 1 & 1
\end{pmatrix}
$$

- **Prediction using Determinant Properties:**
  A fundamental property of determinants states that **swapping any two rows of a matrix multiplies the determinant by $-1$**. 
  Since $B$ is obtained from $A$ by a single row swap, we predict:
  $$
  \det(B) = -\det(A) = -6
  $$

**Part 3: Verifying the Prediction by Calculation**

Let's compute $\det(B)$ directly by expanding along the first row:

$$
\det(B) = 0 \cdot
\begin{vmatrix}
2 & 0 \\
1 & 1
\end{vmatrix}
- 3 \cdot
\begin{vmatrix}
1 & 0 \\
2 & 1
\end{vmatrix}
+ 1 \cdot
\begin{vmatrix}
1 & 2 \\
2 & 1
\end{vmatrix}
$$

Calculating each term:

$$
\det(B) = 0 - 3 \cdot ((1)(1) - (0)(2)) + 1 \cdot ((1)(1) - (2)(2))
$$

$$
\det(B) = 0 - 3(1 - 1 \cdot 0) + 1(1 - 4)
$$

$$
\det(B) = -3(1) + 1(-3) = -3 - 3 = -6
$$

The calculated determinant matches our prediction ($\det(B) = -6$), verifying the property.
