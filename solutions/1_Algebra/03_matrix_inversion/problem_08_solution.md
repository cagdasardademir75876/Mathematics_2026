### Exercise 8. Inverse of a Transformation

**Problem**

The matrix

$$
S=
\begin{pmatrix}
2 & 0 \\
0 & \frac{1}{2}
\end{pmatrix}
$$

describes a scaling of the plane. Find $S^{-1}$ and explain geometrically what the inverse transformation does. Check the action of the pair $S, S^{-1}$ on one simple vector.

**Solution**

**Part 1: Finding the Inverse Matrix $S^{-1}$**

First, compute the determinant of the $2 \times 2$ diagonal matrix $S$:

$$
\det(S) = (2)\left(\frac{1}{2}\right) - (0)(0)
$$

$$
\det(S) = 1 - 0 = 1
$$

Since $\det(S) = 1 \neq 0$, the inverse exists. Applying the $2 \times 2$ inverse formula:

$$
S^{-1} = \frac{1}{1}
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & 2
\end{pmatrix}
$$

$$
S^{-1} =
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & 2
\end{pmatrix}
$$

*(Note: For any diagonal matrix with non-zero diagonal entries, the inverse is simply obtained by taking the reciprocal of each diagonal element).*

**Part 2: Geometric Interpretation of $S$ and $S^{-1}$**

- **Action of $S$:** Multiplying a vector $\begin{pmatrix} x \\ y \end{pmatrix}$ by $S$ produces $\begin{pmatrix} 2x \\ \frac{1}{2}y \end{pmatrix}$. Geometrically, $S$ **stretches** the plane horizontally (along the $x$-axis) by a factor of $2$, and **compresses** the plane vertically (along the $y$-axis) by a factor of $\frac{1}{2}$.

- **Action of $S^{-1}$:** Multiplying a vector $\begin{pmatrix} x \\ y \end{pmatrix}$ by $S^{-1}$ produces $\begin{pmatrix} \frac{1}{2}x \\ 2y \end{pmatrix}$. Geometrically, the inverse transformation $S^{-1}$ **undoes** the action of $S$: it **compresses** the plane horizontally (along the $x$-axis) by a factor of $\frac{1}{2}$, and **stretches** the plane vertically (along the $y$-axis) by a factor of $2$, restoring every point in the plane back to its original position.

**Part 3: Checking the Action on a Simple Vector**

Let us test the pair $S$ and $S^{-1}$ on a simple test vector, for example:

$$
v =
\begin{pmatrix}
3 \\
4
\end{pmatrix}
$$

First, apply the transformation $S$ to $v$:

$$
Sv =
\begin{pmatrix}
2 & 0 \\
0 & \frac{1}{2}
\end{pmatrix}
\begin{pmatrix}
3 \\
4
\end{pmatrix}
$$

$$
Sv =
\begin{pmatrix}
2(3) + 0(4) \\
0(3) + \frac{1}{2}(4)
\end{pmatrix}
$$

$$
Sv =
\begin{pmatrix}
6 \\
2
\end{pmatrix}
$$

Next, apply the inverse transformation $S^{-1}$ to the resulting vector $Sv$:

$$
S^{-1}(Sv) =
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & 2
\end{pmatrix}
\begin{pmatrix}
6 \\
2
\end{pmatrix}
$$

$$
S^{-1}(Sv) =
\begin{pmatrix}
\frac{1}{2}(6) + 0(2) \\
0(6) + 2(2)
\end{pmatrix}
$$

$$
S^{-1}(Sv) =
\begin{pmatrix}
3 \\
4
\end{pmatrix}
= v
$$

Applying $S$ transforms $\begin{pmatrix} 3 \\ 4 \end{pmatrix}$ into $\begin{pmatrix} 6 \\ 2 \end{pmatrix}$, and applying $S^{-1}$ immediately brings it back to $\begin{pmatrix} 3 \\ 4 \end{pmatrix}$, confirming that $S^{-1}$ reverses the geometric effect of $S$.
