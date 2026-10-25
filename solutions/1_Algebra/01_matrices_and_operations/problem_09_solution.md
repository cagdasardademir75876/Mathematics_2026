### Exercise 9. Composing Transformations

Given

$$
S=\begin{pmatrix}
2 & 0 \\
0 & 1 \\
\end{pmatrix},\qquad R=\begin{pmatrix}
0 & -1 \\
1 & 0 \\
\end{pmatrix},\qquad x=\begin{pmatrix}
1 \\
2 \\
\end{pmatrix}
$$

---

#### 1. Computations of Composed Transformations

**Computation of $RSx$:**

First, apply the scaling matrix $S$ to the vector $x$:
$$
Sx = \begin{pmatrix}
2 & 0 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 \\
2 \\
\end{pmatrix}
= \begin{pmatrix}
2(1) + 0(2) \\
0(1) + 1(2) \\
\end{pmatrix}
= \begin{pmatrix}
2 \\
2 \\
\end{pmatrix}
$$

Next, apply the rotation matrix $R$ to the resulting vector $Sx$:
$$
RSx = \begin{pmatrix}
0 & -1 \\
1 & 0 \\
\end{pmatrix}
\begin{pmatrix}
2 \\
2 \\
\end{pmatrix}
= \begin{pmatrix}
0(2) + (-1)(2) \\
1(2) + 0(2) \\
\end{pmatrix}
= \begin{pmatrix}
-2 \\
2 \\
\end{pmatrix}
$$

**Computation of $SRx$:**

First, apply the rotation matrix $R$ to the vector $x$:
$$
Rx = \begin{pmatrix}
0 & -1 \\
1 & 0 \\
\end{pmatrix}
\begin{pmatrix}
1 \\
2 \\
\end{pmatrix}
= \begin{pmatrix}
0(1) + (-1)(2) \\
1(1) + 0(2) \\
\end{pmatrix}
= \begin{pmatrix}
-2 \\
1 \\
\end{pmatrix}
$$

Next, apply the scaling matrix $S$ to the resulting vector $Rx$:
$$
SRx = \begin{pmatrix}
2 & 0 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
-2 \\
1 \\
\end{pmatrix}
= \begin{pmatrix}
2(-2) + 0(1) \\
0(-2) + 1(1) \\
\end{pmatrix}
= \begin{pmatrix}
-4 \\
1 \\
\end{pmatrix}
$$

---

#### 2. Geometric Interpretation and Comparison

Comparing the results:
$$
RSx = \begin{pmatrix} -2 \\ 2 \end{pmatrix} \neq \begin{pmatrix} -4 \\ 1 \end{pmatrix} = SRx
$$

**Geometric Explanation:**
* In the product $RSx$, the vector $x$ is first stretched horizontally by a factor of $2$ via scaling ($S$), and then rotated $90^\circ$ counterclockwise via $R$. The horizontal stretching happens along the original coordinate axes before the space is rotated.
* In the product $SRx$, the vector $x$ is first rotated $90^\circ$ counterclockwise via $R$, changing the orientation of the coordinates, and then the nonuniform scaling $S$ is applied relative to the *new* axes directions. 

Because matrix multiplication corresponds to the composition of geometric transformations, the final position of the vector depends strongly on the sequence in which these operations are applied. This geometric noncommutativity directly reflects the noncommutative property of matrix multiplication ($RS \neq SR$).
