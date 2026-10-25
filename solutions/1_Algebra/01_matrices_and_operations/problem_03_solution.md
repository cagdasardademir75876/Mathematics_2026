### Exercise 3. When Can Matrices Be Multiplied?

The sizes of the given matrices are:

$$
A_{2\times3},\qquad B_{3\times4},\qquad C_{4\times2},\qquad D_{2\times2}
$$

---

#### 1. Dimension Compatibility Rule

Matrix multiplication $M \times N$ is defined if and only if the number of columns in the left matrix $M$ equals the number of rows in the right matrix $N$. 

If $M$ has dimensions $m \times p$ and $N$ has dimensions $p \times n$, then the product $MN$ is defined and has dimensions $m \times n$.

---

#### 2. Evaluation of Matrix Products

* **Product $AB$:**
  * Dimensions: $(2\times3) \cdot (3\times4)$
  * Compatibility: Inner dimensions match ($3 = 3$).
  * **Defined:** Yes, the result has size **$2 \times 4$**.

* **Product $BA$:**
  * Dimensions: $(3\times4) \cdot (2\times3)$
  * Compatibility: Inner dimensions do not match ($4 \neq 2$).
  * **Defined:** No.

* **Product $BC$:**
  * Dimensions: $(3\times4) \cdot (4\times2)$
  * Compatibility: Inner dimensions match ($4 = 4$).
  * **Defined:** Yes, the result has size **$3 \times 2$**.

* **Product $CB$:**
  * Dimensions: $(4\times2) \cdot (3\times4)$
  * Compatibility: Inner dimensions do not match ($2 \neq 3$).
  * **Defined:** No.

* **Product $AC$:**
  * Dimensions: $(2\times3) \cdot (4\times2)$
  * Compatibility: Inner dimensions do not match ($3 \neq 4$).
  * **Defined:** No.

* **Product $CA$:**
  * Dimensions: $(4\times2) \cdot (2\times3)$
  * Compatibility: Inner dimensions match ($2 = 2$).
  * **Defined:** Yes, the result has size **$4 \times 3$**.

* **Product $AD$:**
  * Dimensions: $(2\times3) \cdot (2\times2)$
  * Compatibility: Inner dimensions do not match ($3 \neq 2$).
  * **Defined:** No.

* **Product $DA$:**
  * Dimensions: $(2\times2) \cdot (2\times3)$
  * Compatibility: Inner dimensions match ($2 = 2$).
  * **Defined:** Yes, the result has size **$2 \times 3$**.****
