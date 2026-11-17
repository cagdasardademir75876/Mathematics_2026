### Exercise 12. Finding Inverses Without Starting from Scratch

**Problem**

It is known that

$$
A^{-1}=
\begin{pmatrix}
2 & -1 \\
-3 & 2
\end{pmatrix}.
$$

Without finding $A$, compute $(3A)^{-1}$, $(A^T)^{-1}$, and $(A^2)^{-1}$. Justify each result using the appropriate property.

**Solution**

**Part 1: Computing $(3A)^{-1}$**

- **Property:** For any invertible matrix $A$ and any non-zero scalar $c$, the inverse of the scalar multiple is given by:

$$
(cA)^{-1} = \frac{1}{c} A^{-1}
$$

Justification: $(3A)\left(\frac{1}{3}A^{-1}\right) = \left(3 \cdot \frac{1}{3}\right)(AA^{-1}) = 1 \cdot I = I$.

- **Calculation:** Applying this property with $c = 3$:

$$
(3A)^{-1} = \frac{1}{3} A^{-1} = \frac{1}{3}
\begin{pmatrix}
2 & -1 \\
-3 & 2
\end{pmatrix}
$$

$$
(3A)^{-1} =
\begin{pmatrix}
\frac{2}{3} & -\frac{1}{3} \\
-1 & \frac{2}{3}
\end{pmatrix}
$$

**Part 2: Computing $(A^T)^{-1}$**

- **Property:** The inverse of the transpose of an invertible matrix equals the transpose of its inverse:

$$
(A^T)^{-1} = (A^{-1})^T
$$

Justification: Taking the transpose of $A A^{-1} = I$ gives $(A A^{-1})^T = I^T \implies (A^{-1})^T A^T = I$, showing that $(A^{-1})^T$ is the inverse of $A^T$.

- **Calculation:** Taking the transpose of $A^{-1}$ (swapping rows and columns):

$$
(A^T)^{-1} = (A^{-1})^T =
\begin{pmatrix}
2 & -3 \\
-1 & 2
\end{pmatrix}
$$

**Part 3: Computing $(A^2)^{-1}$**

- **Property:** For any invertible matrix $A$ and positive integer $k$, the inverse of a power of $A$ equals the same power of $A^{-1}$ (which also follows from the product rule $(AB)^{-1} = B^{-1}A^{-1}$ applied to $A \cdot A$):

$$
(A^2)^{-1} = (A^{-1})^2
$$

Justification: $A^2 (A^{-1})^2 = (AA)(A^{-1}A^{-1}) = A(AA^{-1})A^{-1} = A I A^{-1} = A A^{-1} = I$.

- **Calculation:** Squaring the matrix $A^{-1}$:

$$
(A^2)^{-1} = (A^{-1})^2 =
\begin{pmatrix}
2 & -1 \\
-3 & 2
\end{pmatrix}
\begin{pmatrix}
2 & -1 \\
-3 & 2
\end{pmatrix}
$$

$$
(A^2)^{-1} =
\begin{pmatrix}
2(2) + (-1)(-3) & 2(-1) + (-1)(2) \\
(-3)(2) + 2(-3) & (-3)(-1) + 2(2)
\end{pmatrix}
$$

$$
(A^2)^{-1} =
\begin{pmatrix}
4 + 3 & -2 - 2 \\
-6 - 6 & 3 + 4
\end{pmatrix}
$$

$$
(A^2)^{-1} =
\begin{pmatrix}
7 & -4 \\
-12 & 7
\end{pmatrix}
$$
