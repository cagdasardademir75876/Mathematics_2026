### Exercise 4. Triangular Matrix

**Problem**

Without expanding the determinant, compute

$$
\det
\begin{pmatrix}
2 & 4 & 1 \\
0 & -3 & 5 \\
0 & 0 & 7
\end{pmatrix}
$$

State the rule for an arbitrary triangular matrix and explain it using this example.

**Solution**

**Part 1: Computing the Determinant**

The given matrix is an **upper triangular matrix** because all entries below the main diagonal are zeros ($0$).

According to the rule for triangular matrices, the determinant of a triangular matrix (upper or lower) is simply equal to the **product of the entries on its main diagonal**.

Applying this rule to the given matrix:

$$
\det = (2) \cdot (-3) \cdot (7)
$$

$$
\det = -6 \cdot 7 = -42
$$

Thus, the determinant is $-42$.

**Part 2: Rule for an Arbitrary Triangular Matrix and Explanation**

- **General Rule:** 
  For any $n \times n$ triangular matrix (where all entries either above or below the main diagonal are zero), the determinant is given by the product of its diagonal elements:
  $$
  \det(A) = a_{11} a_{22} a_{33} \cdots a_{nn} = \prod_{i=1}^{n} a_{ii}
  $$

- **Explanation Using This Example:**
  If we were to evaluate this determinant via cofactor expansion along the first column, we would only have the top-left entry ($2$) multiplied by the determinant of the remaining $2 \times 2$ submatrix:
  $$
  2 \cdot
  \begin{vmatrix}
  -3 & 5 \\
  0 & 7
  \end{vmatrix}
  $$
  For this resulting $2 \times 2$ triangular matrix, expanding again yields $(-3) \cdot (7)$. Combining these steps gives the product of all three diagonal elements: $2 \cdot (-3) \cdot (-7) = -42$. This recursive expansion demonstrates why the determinant of any triangular matrix always collapses to the product of its diagonal entries.
