### Exercise 11. When Do Matrices Commute?

**Problem**

Given

$$
A=
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
$$

and

$$
B=
\begin{pmatrix}
a & b \\
c & d
\end{pmatrix}
$$

Find the conditions on $a,b,c,d$ under which $AB=BA$. Describe the general form of all such matrices $B$.

**Solution**

**Part 1: Computing $AB$ and $BA$**

- Compute the product $AB$:

$$
AB =
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
a & b \\
c & d
\end{pmatrix}
$$

$$
AB =
\begin{pmatrix}
1(a) + 1(c) & 1(b) + 1(d) \\
0(a) + 1(c) & 0(b) + 1(d)
\end{pmatrix}
$$

$$
AB =
\begin{pmatrix}
a + c & b + d \\
c & d
\end{pmatrix}
$$

- Compute the product $BA$:

$$
BA =
\begin{pmatrix}
a & b \\
c & d
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
$$

$$
BA =
\begin{pmatrix}
a(1) + b(0) & a(1) + b(1) \\
c(1) + d(0) & c(1) + d(1)
\end{pmatrix}
$$

$$
BA =
\begin{pmatrix}
a & a + b \\
c & c + d
\end{pmatrix}
$$

**Part 2: Finding the Conditions for $AB = BA$**

Equating the corresponding entries of $AB$ and $BA$:

$$
\begin{pmatrix}
a + c & b + d \\
c & d
\end{pmatrix}
=
\begin{pmatrix}
a & a + b \\
c & c + d
\end{pmatrix}
$$

This gives the following system of equations for the entries:
1. $a + c = a \implies c = 0$
2. $b + d = a + b \implies d = a$
3. $c = c$ (trivially satisfied since $c = 0$)
4. $d = c + d \implies c = 0$ (consistent with the first condition)

Thus, the conditions for $AB = commutator$ to hold are:
- $c = 0$
- $d = a$
- $a$ and $b$ can be any arbitrary real numbers.

**Part 3: General Form of Matrix $B$**

Substituting these conditions back into matrix $B$:

$$
B =
\begin{pmatrix}
a & b \\
0 & a
\end{pmatrix}
$$

**Conclusion:** 
All matrices $B$ that commute with $A$ must have upper-triangular form where the diagonal entries are equal ($a = d$) and the bottom-left entry is zero ($c = 0$).
