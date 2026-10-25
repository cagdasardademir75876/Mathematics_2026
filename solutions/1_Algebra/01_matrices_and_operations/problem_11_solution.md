### Exercise 11. When Do Matrices Commute?

Given

$$A=\begin{pmatrix} 1 & 1 \\ 0 & 1 \\ \end{pmatrix},\qquad B=\begin{pmatrix} a & b \\ c & d \\ \end{pmatrix}$$

---

#### 1. Computations of $AB$ and $BA$

**Computation of $AB$:**

$$AB = \begin{pmatrix} 1 & 1 \\ 0 & 1 \\ \end{pmatrix} \begin{pmatrix} a & b \\ c & d \\ \end{pmatrix}$$

$$AB = \begin{pmatrix} 1(a) + 1(c) & 1(b) + 1(d) \\ 0(a) + 1(c) & 0(b) + 1(d) \\ \end{pmatrix} = \begin{pmatrix} a+c & b+d \\ c & d \\ \end{pmatrix}$$

**Computation of $BA$:**

$$BA = \begin{pmatrix} a & b \\ c & d \\ \end{pmatrix} \begin{pmatrix} 1 & 1 \\ 0 & 1 \\ \end{pmatrix}$$

$$BA = \begin{pmatrix} a(1) + b(0) & a(1) + b(1) \\ c(1) + d(0) & c(1) + d(1) \\ \end{pmatrix} = \begin{pmatrix} a & a+b \\ c & c+d \\ \end{pmatrix}$$

---

#### 2. Deriving Conditions for $AB = BA$

For $AB$ to equal $BA$, their corresponding entries must be equal:

1. **Top-left entry:** $a+c = a \implies c = 0$
2. **Top-right entry:** $b+d = a+b \implies d = a$
3. **Bottom-left entry:** $c = c$ (always true)
4. **Bottom-right entry:** $d = c+d \implies c = 0$

Thus, the required conditions on $a, b, c, d$ are:

$$c = 0 \qquad \text{and} \qquad d = a$$

---

#### 3. General Form of Matrix $B$

Substituting $c = 0$ and $d = a$ into matrix $B$ gives its general form:

$$B = \begin{pmatrix} a & b \\ 0 & a \\ \end{pmatrix}$$

where $a$ and $b$ can be any real numbers. 

Therefore, any matrix that commutes with $A$ must have equal diagonal entries ($a$) and a zero in the lower-left entry ($c = 0$), while the upper-right entry ($b$) can take any arbitrary value.
