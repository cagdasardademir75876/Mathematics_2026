
### Exercise 1. Definition of the Inverse

**Problem**

For

$$
A=
\begin{pmatrix}
2 & 1 \\
1 & 1 \\
\end{pmatrix},
\qquad
B=
\begin{pmatrix}
1 & -1 \\
-1 & 2 \\
\end{pmatrix}
$$

check, without using a formula, whether $B=A^{-1}$. Compute $AB$ and $BA$ and relate the result to the definition of the inverse.

> **Why this exercise:** starts from the definition of the inverse through multiplication before any formulas or computational methods are introduced.

**Solution**

**1. Definition of the Inverse**

A square matrix $B$ is the inverse of a square matrix $A$ if multiplying them in either order gives the identity matrix.

For two $2\times2$ matrices, the identity matrix is

$$
I=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
$$

Therefore, to check whether $B=A^{-1}$, we need to calculate both $AB$ and $BA$.

**2. Computing $AB$**

Using the given matrices,

$$
AB=
\begin{pmatrix}
2 & 1 \\
1 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 & -1 \\
-1 & 2 \\
\end{pmatrix}
$$

Multiplying the rows of $A$ by the columns of $B$ gives

$$
AB=
\begin{pmatrix}
2\cdot1+1\cdot(-1) & 2\cdot(-1)+1\cdot2 \\
1\cdot1+1\cdot(-1) & 1\cdot(-1)+1\cdot2 \\
\end{pmatrix}
$$

Simplifying,

$$
AB=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
=I
$$

**3. Computing $BA$**

Now reverse the order of multiplication:

$$
BA=
\begin{pmatrix}
1 & -1 \\
-1 & 2 \\
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
1 & 1 \\
\end{pmatrix}
$$

Multiplying the rows of $B$ by the columns of $A$ gives

$$
BA=
\begin{pmatrix}
1\cdot2+(-1)\cdot1 & 1\cdot1+(-1)\cdot1 \\
(-1)\cdot2+2\cdot1 & (-1)\cdot1+2\cdot1 \\
\end{pmatrix}
$$

Simplifying,

$$
BA=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
=I
$$

**4. Relating the Results to the Definition**

Both matrix products give the identity matrix:

$AB=I$ and $BA=I$.

According to the definition of an inverse matrix, if two square matrices multiply in both orders to give the identity matrix, they are inverses of each other.

Therefore, $B$ is the inverse of $A$.

**Final Answer**

$$
AB=BA=I
$$

Thus,

$$
B=A^{-1}
$$

The matrix $B$ is indeed the inverse of matrix $A$, as confirmed by both multiplication orders.
