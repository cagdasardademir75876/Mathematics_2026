
### Solution

#### Part 1: Computing the Determinant

The given matrix is an **upper triangular matrix** because all entries below the main diagonal are zero.

For any triangular matrix, the determinant is equal to the product of the entries on its main diagonal.

Therefore:

$$
\det(A) = 2 \cdot (-3) \cdot 7
$$

$$
\boxed{\det(A) = -42}
$$

#### Part 2: General Rule for Triangular Matrices

For any \(n \times n\) triangular matrix (upper or lower), the determinant is the product of all diagonal entries.

The general formula is:

$$
\boxed{\det(A) = \prod_{i=1}^{n} a_{ii}}
$$

#### Part 3: Explanation Using This Example

In the given matrix, the diagonal entries are \(2\), \(-3\), and \(7\).

All entries below the main diagonal are zero. This means that the determinant can be calculated directly by multiplying the diagonal entries without expanding the determinant.

Thus:

$$
\det(A) = 2 \cdot (-3) \cdot 7 = -42
$$

This example demonstrates that the determinant of any triangular matrix is always equal to the product of its main diagonal entries.

> **Why this exercise:** reinforces an important property of triangular matrices.
