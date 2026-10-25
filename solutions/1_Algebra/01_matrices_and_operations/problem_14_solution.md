### Exercise 14. Rotation Matrices

The matrix for a rotation through an angle $\theta$ is defined as:

$$R(\theta)=\begin{pmatrix} \cos\theta & -\sin\theta \\ \sin\theta & \cos\theta \\ \end{pmatrix}$$

---

#### 1. Computation of $R(\alpha)R(\beta)$

Multiplying the two rotation matrices $R(\alpha)$ and $R(\beta)$:

$$R(\alpha)R(\beta) = \begin{pmatrix} \cos\alpha & -\sin\alpha \\ \sin\alpha & \cos\alpha \\ \end{pmatrix} \begin{pmatrix} \cos\beta & -\sin\beta \\ \sin\beta & \cos\beta \\ \end{pmatrix}$$

Performing entry-by-entry matrix multiplication:

$$R(\alpha)R(\beta) = \begin{pmatrix} \cos\alpha\cos\beta - \sin\alpha\sin\beta & -\cos\alpha\sin\beta - \sin\alpha\cos\beta \\ \sin\alpha\cos\beta + \cos\alpha\sin\beta & -\sin\alpha\sin\beta + \cos\alpha\cos\beta \\ \end{pmatrix}$$

Factoring out the negative sign in the top-right entry:

$$R(\alpha)R(\beta) = \begin{pmatrix} \cos\alpha\cos\beta - \sin\alpha\sin\beta & -(\sin\alpha\cos\beta + \cos\alpha\sin\beta) \\ \sin\alpha\cos\beta + \cos\alpha\sin\beta & \cos\alpha\cos\beta - \sin\alpha\sin\beta \\ \end{pmatrix}$$

---

#### 2. Verification using Trigonometric Angle-Sum Formulas

Recall the standard angle-sum trigonometric identities:
* $\cos(\alpha+\beta) = \cos\alpha\cos\beta - \sin\alpha\sin\beta$
* $\sin(\alpha+\beta) = \sin\alpha\cos\beta + \cos\alpha\sin\beta$

Substituting these identities directly into the matrix product gives:

$$R(\alpha)R(\beta) = \begin{pmatrix} \cos(\alpha+\beta) & -\sin(\alpha+\beta) \\ \sin(\alpha+\beta) & \cos(\alpha+\beta) \\ \end{pmatrix} = R(\alpha+\beta)$$

Thus, we have shown that $R(\alpha)R(\beta) = R(\alpha+\beta)$.

---

####
