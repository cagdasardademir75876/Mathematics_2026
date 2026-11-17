### Exercise 13. Undoing a Composite Transformation

**Problem**

The matrices

$$
S=
\begin{pmatrix}
2 & 0 \\
0 & 1
\end{pmatrix}
$$

and

$$
H=
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
$$

describe nonuniform scaling and shear. For $T=HS$, find $T^{-1}$ in two ways:

1. first compute $T$, then its inverse,
2. use $(HS)^{-1}=S^{-1}H^{-1}$.

Compare the results. Additionally compute $H^{-1}S^{-1}$ and verify that the incorrect order gives a different matrix. Explain the rule: “when undoing a composition of operations, we undo them from the end.”

**Solution**

**Method 1: First Compute $T = HS$, Then Find Its Inverse $T^{-1}$**

First, compute the product $T = HS$:

$$
T = HS =
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
2 & 0 \\
0 & 1
\end{pmatrix}
$$

$$
T =
\begin{pmatrix}
1(2) + 1(0) & 1(0) + 1(1) \\
0(2) + 1(0) & 0(0) + 1(1)
\end{pmatrix}
$$

$$
T =
\begin{pmatrix}
2 & 1 \\
0 & 1
\end{pmatrix}
$$

Next, compute the determinant of $T$:

$$
\det(T) = (2)(1) - (1)(0) = 2
$$

Using the $2 \times 2$ inverse formula, we find $T^{-1}$:

$$
T^{-1} = \frac{1}{2}
\begin{pmatrix}
1 & -1 \\
0 & 2
\end{pmatrix}
$$

$$
T^{-1} =
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & 1
\end{pmatrix}
$$

**Method 2: Use the Product Property $(HS)^{-1} = S^{-1}H^{-1}$**

First, find $S^{-1}$ and $H^{-1}$ individually.

For $S$, $\det(S) = (2)(1) - (0)(0) = 2$, so:

$$
S^{-1} = \frac{1}{2}
\begin{pmatrix}
1 & 0 \\
0 & 2
\end{pmatrix}
=
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & 1
\end{pmatrix}
$$

For $H$, $\det(H) = (1)(1) - (1)(0) = 1$, so:

$$
H^{-1} =
\begin{pmatrix}
1 & -1 \\
0 & 1
\end{pmatrix}
$$

Now, compute the product $S^{-1}H^{-1}$:

$$
S^{-1}H^{-1} =
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
1 & -1 \\
0 & 1
\end{pmatrix}
$$

$$
S^{-1}H^{-1} =
\begin{pmatrix}
\frac{1}{2}(1) + 0(0) & \frac{1}{2}(-1) + 0(1) \\
0(1) + 1(0) & 0(-1) + 1(1)
\end{pmatrix}
$$

$$
S^{-1}H^{-1} =
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & 1
\end{pmatrix}
$$

Comparing Method 1 and Method 2, both approaches produce the exact same inverse matrix:

$$
T^{-1} = (HS)^{-1} = S^{-1}H^{-1} =
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & 1
\end{pmatrix}
$$

**Part 3: Computing $H^{-1}S^{-1}$ (Incorrect Order)**

Now we compute the product in the non-reversed order $H^{-1}S^{-1}$:

$$
H^{-1}S^{-1} =
\begin{pmatrix}
1 & -1 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & 1
\end{pmatrix}
$$

$$
H^{-1}S^{-1} =
\begin{pmatrix}
1\left(\frac{1}{2}\right) + (-1)(0) & 1(0) + (-1)(1) \\
0\left(\frac{1}{2}\right) + 1(0) & 0(0) + 1(1)
\end{pmatrix}
$$

$$
H^{-1}S^{-1} =
\begin{pmatrix}
\frac{1}{2} & -1 \\
0 & 1
\end{pmatrix}
$$

Comparing this result to $T^{-1}$, we see that:

$$
H^{-1}S^{-1} =
\begin{pmatrix}
\frac{1}{2} & -1 \\
0 & 1
\end{pmatrix}
\neq
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & 1
\end{pmatrix}
= T^{-1}
$$

The entries in the top-right position differ ($-1$ vs. $-\frac{1}{2}$), verifying that the incorrect order yields a different matrix.

**Part 4: Explanation of the Rule**

When a composite transformation $T = HS$ is applied to a vector $v$, the action is written as $Tv = H(Sv)$:

1. **First**, the scaling matrix $S$ stretches the horizontal component of $v$.
2. **Second**, the shear matrix $H$ shifts the already-stretched vector.

To return the vector to its original state, we must reverse the sequence of events **from the end (Last-In, First-Out)**:

- We must **first** undo the shear $H$ (by applying $H^{-1}$) while the vector is still in its stretched state.
- Only **after** the shear is removed can we undo the horizontal scaling $S$ (by applying $S^{-1}$).

Algebraically, this corresponds to $S^{-1}H^{-1}(HSv) = S^{-1}(H^{-1}H)Sv = S^{-1}ISv = S^{-1}Sv = v$. Applying $H^{-1}S^{-1}$ instead would attempt to shrink the vector before undoing the shear, scaling the shear displacement incorrectly.
