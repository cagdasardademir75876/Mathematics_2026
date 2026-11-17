### Exercise 4. Gauss–Jordan

**Problem**

Find $A^{-1}$ using the Gauss–Jordan method for

$$
A=
\begin{pmatrix}
1 & 2 \\
3 & 5
\end{pmatrix}
$$

Show the augmented matrix $[A\mid I]$ after successive operations and explain why obtaining $I$ on the left gives the inverse on the right.

**Solution**

**Part 1: Gauss–Jordan Elimination**

We begin by setting up the augmented matrix $[A \mid I_2]$:

$$
\left[
\begin{array}{cc|cc}
1 & 2 & 1 & 0 \\
3 & 5 & 0 & 1
\end{array}
\right]
$$

- **Step 1:** Eliminate the entry below the pivot in the first column by performing $R_2 \leftarrow R_2 - 3R_1$.
  - Left side calculation: $(3 - 3(1), \, 5 - 3(2)) = (0, -1)$
  - Right side calculation: $(0 - 3(1), \, 1 - 3(0)) = (-3, 1)$

  The augmented matrix becomes:

  $$
  \left[
  \begin{array}{cc|cc}
  1 & 2 & 1 & 0 \\
  0 & -1 & -3 & 1
  \end{array}
  \right]
  $$

- **Step 2:** Scale the second row so that its pivot becomes $1$ by performing $R_2 \leftarrow -R_2$.

  The augmented matrix becomes:

  $$
  \left[
  \begin{array}{cc|cc}
  1 & 2 & 1 & 0 \\
  0 & 1 & 3 & -1
  \end{array}
  \right]
  $$

- **Step 3:** Eliminate the entry above the pivot in the second column by performing $R_1 \leftarrow R_1 - 2R_2$.
  - Left side calculation: $(1 - 2(0), \, 2 - 2(1)) = (1, 0)$
  - Right side calculation: $(1 - 2(3), \, 0 - 2(-1)) = (-5, 2)$

  The augmented matrix reaches reduced row echelon form:

  $$
  \left[
  \begin{array}{cc|cc}
  1 & 0 & -5 & 2 \\
  0 & 1 & 3 & -1
  \end{array}
  \right]
  $$

Since the left side is now the identity matrix $I_2$, the right side gives the inverse matrix $A^{-1}$:

$$
A^{-1} =
\begin{pmatrix}
-5 & 2 \\
3 & -1
\end{pmatrix}
$$

**Part 2: Why Obtaining $I$ on the Left Gives $A^{-1}$ on the Right**

Each elementary row operation applied to a matrix is mathematically equivalent to multiplying that matrix on the left by an elementary matrix $E_i$. 

When we perform a sequence of $k$ row operations ($E_1, E_2, \dots, E_k$) to transform the augmented matrix $[A \mid I]$ into $[I \mid B]$, we are effectively multiplying both sides of the augmented matrix by the product $P = E_k \cdots E_2 E_1$:

$$
P [A \mid I] = [PA \mid PI] = [I \mid B]
$$

From the left block, we see that:

$$
PA = I
$$

By the definition of the matrix inverse, any matrix $P$ that multiplies $A$ to yield the identity matrix $I$ must be $A^{-1}$ (so $P = A^{-1}$). Substituting $P = A^{-1}$ into the right block gives:

$$
B = PI = A^{-1} I = A^{-1}
$$

Therefore, whatever sequence of row operations turns $A$ into $I$ simultaneously transforms $I$ into $A^{-1}$.
