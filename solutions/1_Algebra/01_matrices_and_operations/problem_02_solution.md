### Exercise 2. Addition and Scalar Multiplication

Given

$$
A=\begin{pmatrix}
1 & 2 \\
-1 & 3 \\
\end{pmatrix}
$$

and

$$
B=\begin{pmatrix}
4 & -2 \\
0 & 5 \\
\end{pmatrix}
$$

---

#### 1. Computations

**Computation of $A+B$:**

$$
A+B = \begin{pmatrix}
1+4 & 2+(-2) \\
-1+0 & 3+5 \\
\end{pmatrix}
= \begin{pmatrix}
5 & 0 \\
-1 & 8 \\
\end{pmatrix}
$$

**Computation of $A-B$:**

$$
A-B = \begin{pmatrix}
1-4 & 2-(-2) \\
-1-0 & 3-5 \\
\end{pmatrix}
= \begin{pmatrix}
-3 & 4 \\
-1 & -2 \\
\end{pmatrix}
$$

**Computation of $3A-2B$:**

First, calculate the scalar multiples:

$$
3A = \begin{pmatrix}
3 & 6 \\
-3 & 9 \\
\end{pmatrix}
$$

$$
2B = \begin{pmatrix}
8 & -4 \\
0 & 10 \\
\end{pmatrix}
$$

Subtracting $2B$ from $3A$:

$$
3A-2B = \begin{pmatrix}
3-8 & 6-(-4) \\
-3-0 & 9-10 \\
\end{pmatrix}
= \begin{pmatrix}
-5 & 10 \\
-3 & -1 \\
\end{pmatrix}
$$

---

#### 2. Dimension Compatibility Requirement

Matrix addition and subtraction are defined element-wise, meaning that the entry in row $i$ and column $j$ of the first matrix is added to (or subtracted from) the entry in row $i$ and column $j$ of the second matrix. 

If two matrices have different sizes, there is no one-to-one correspondence between their entries, leaving some entries without a corresponding term to pair with. Therefore, matrix addition is defined only for matrices of the same dimensions.
