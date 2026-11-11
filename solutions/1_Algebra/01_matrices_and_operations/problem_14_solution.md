### Exercise 14. Rotation Matrices

**Problem**

The matrix for a rotation through an angle $\theta$ is

$$
R(\theta)=
\begin{pmatrix}
\cos\theta & -\sin\theta \\
\sin\theta & \cos\theta
\end{pmatrix}
$$

Compute $R(\alpha)R(\beta)$ and, using the angle-sum formulas for sine and cosine, show that

$$
R(\alpha)R(\beta)=R(\alpha+\beta).
$$

Explain the result geometrically.

**Solution**

**Part 1: Computing the Product $R(\alpha)R(\beta)$**

Multiply the two rotation matrices:

$$
R(\alpha)R(\beta) =
\begin{pmatrix}
\cos\alpha & -\sin\alpha \\
\sin\alpha & \cos\alpha
\end{pmatrix}
\begin{pmatrix}
\cos\beta & -\sin\beta \\
\sin\beta & \cos\beta
\end{pmatrix}
$$

Computing each entry of the resulting product matrix using standard matrix multiplication:

- Top-left entry:

$$
(\cos\alpha)(\cos\beta) + (-\sin\alpha)(\sin\beta) = \cos\alpha\cos\beta - \sin\alpha\sin\beta
$$

- Top-right entry:

$$
(\cos\alpha)(-\sin\beta) + (-\sin\alpha)(\cos\beta) = -(\cos\alpha\sin\beta + \sin\alpha\cos\beta)
$$

- Bottom-left entry:

$$
(\sin\alpha)(\cos\beta) + (\cos\alpha)(\sin\beta) = \sin\alpha\cos\beta + \cos\alpha\sin\beta
$$

- Bottom-right entry:

$$
(\sin\alpha)(-\sin\beta) + (\cos\alpha)(\cos\beta) = \cos\alpha\cos\beta - \sin\alpha\sin\beta
$$

Combining these entries into the product matrix:

$$
R(\alpha)R(\beta) =
\begin{pmatrix}
\cos\alpha\cos\beta - \sin\alpha\sin\beta & -(\sin\alpha\cos\beta + \cos\alpha\sin\beta) \\
\sin\alpha\cos\beta + \cos\alpha\sin\beta & \cos\alpha\cos\beta - \sin\alpha\sin\beta
\end{pmatrix}
$$

**Part 2: Applying Angle-Sum Formulas**

Recall the trigonometric angle-sum identities:
- $\cos(\alpha + \beta) = \cos\alpha\cos\beta - \sin\alpha\sin\beta$
- $\sin(\alpha + \beta) = \sin\alpha\cos\beta + \cos\alpha\sin\beta$

Substituting these identities into the entries of our matrix:

$$
R(\alpha)R(\beta) =
\begin{pmatrix}
\cos(\alpha+\beta) & -\sin(\alpha+\beta) \\
\sin(\alpha+\beta) & \cos(\alpha+\beta)
\end{pmatrix}
$$

By definition, this is precisely the rotation matrix for the combined angle $\alpha + \beta$:

$$
R(\alpha)R(\beta) = R(\alpha+\beta)
$$

**Part 3: Geometric Explanation**

Geometrically, multiplying the rotation matrix $R(\beta)$ by $R(\alpha)$ represents performing two successive rotations about the origin:
1. First, rotating a vector by an angle $\beta$.
2. Second, rotating the resulting vector by an angle $\alpha$.

Composing a rotation of angle $\beta$ followed by a rotation of angle $\alpha$ is equivalent to performing a single rotation by the total accumulated angle $\alpha + \beta$. Thus, matrix multiplication accurately reflects the composition of geometric rotations.
