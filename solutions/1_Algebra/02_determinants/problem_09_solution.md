
### Exercise 9. Area and the Determinant

**Problem**

The vectors

$$
u=
\begin{pmatrix}
3 \\
1 \\
\end{pmatrix},
\qquad
v=
\begin{pmatrix}
1 \\
4 \\
\end{pmatrix}
$$

span a parallelogram. Compute its area using a determinant. Then reverse the order of the vectors and explain what changes in the determinant and what does not change in the area.

> **Why this exercise:** gives the determinant a geometric interpretation and distinguishes its sign from the value of the area.

**Solution**

**1. Computing the determinant**

The area of a parallelogram spanned by two vectors in $\mathbb{R}^2$ is equal to the absolute value of the determinant formed by placing the vectors as columns of a matrix.

Therefore,

$$
\det(u,v)=
\det
\begin{pmatrix}
3 & 1 \\
1 & 4
\end{pmatrix}
$$

Using the determinant formula for a $2\times2$ matrix,

$$
\det(u,v)=3\cdot4-1\cdot1
$$

$$
\det(u,v)=12-1=11
$$

The area is the absolute value of this determinant:

$$
S=|\det(u,v)|=|11|=11
$$

**2. Reversing the Order of the Vectors**

If we reverse the order of the vectors, the matrix becomes

$$
\det(v,u)=
\det
\begin{pmatrix}
1 & 3 \\
4 & 1
\end{pmatrix}
$$

Calculating the determinant,

$$
\det(v,u)=1\cdot1-3\cdot4
$$

$$
\det(v,u)=1-12=-11
$$

The new area is

$$
S=|\det(v,u)|=|-11|=11
$$

**3. Explanation**

Reversing the order of two columns changes the sign of the determinant but does not change its absolute value.

The determinant changes from $11$ to $-11$, while the area remains $11$.

Geometrically, the sign of the determinant represents the orientation of the ordered vectors. Reversing their order changes the orientation, but the parallelogram itself remains the same.

**Final Answer**

The area of the parallelogram is

$$
S=11
$$

The original determinant is $11$, and the determinant after reversing the vectors is $-11$. The area does not change because it is calculated using the absolute value of the determinant.
