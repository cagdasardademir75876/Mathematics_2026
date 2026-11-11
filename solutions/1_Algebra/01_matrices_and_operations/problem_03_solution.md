### Exercise 3. When Can Matrices Be Multiplied?

**Problem**

The matrix sizes are

$$
A_{2\times3}, \qquad B_{3\times4}, \qquad C_{4\times2}, \qquad D_{2\times2}
$$

For the products

$$
AB, \quad BA, \quad BC, \quad CB, \quad AC, \quad CA, \quad AD, \quad DA
$$

determine whether they are defined. If so, state the size of the result. Justify each decision using the dimension compatibility condition.

**Solution**

Two matrices $M$ and $N$ can be multiplied in the order $MN$ if and only if the number of columns of $M$ is equal to the number of rows of $N$. If the dimensions are $M_{m\times n}$ and $N_{n\times p}$, the product is defined and has the resulting size $m\times p$.

- **Product $AB$:**
  - Dimensions: $A_{2\times 3}$ and $B_{3\times 4}$.
  - The number of columns of $A$ ($3$) matches the number of rows of $B$ ($3$).
  - **Status:** Defined. 
  - **Result size:** $2 \times 4$.

- **Product $BA$:**
  - Dimensions: $B_{3\times 4}$ and $A_{2\times 3}$.
  - The number of columns of $B$ ($4$) does not match the number of rows of $A$ ($2$).
  - **Status:** Not defined.

- **Product $BC$:**
  - Dimensions: $B_{3\times 4}$ and $C_{4\times 2}$.
  - The number of columns of $B$ ($4$) matches the number of rows of $C$ ($4$).
  - **Status:** Defined.
  - **Result size:** $3 \times 2$.

- **Product $CB$:**
  - Dimensions: $C_{4\times 2}$ and $B_{3\times 4}$.
  - The number of columns of $C$ ($2$) does not match the number of rows of $B$ ($3$).
  - **Status:** Not defined.

- **Product $AC$:**
  - Dimensions: $A_{2\times 3}$ and $C_{4\times 2}$.
  - The number of columns of $A$ ($3$) does not match the number of rows of $C$ ($4$).
  - **Status:** Not defined.

- **Product $CA$:**
  - Dimensions: $C_{4\times 2}$ and $A_{2\times 3}$.
  - The number of columns of $C$ ($2$) matches the number of rows of $A$ ($2$).
  - **Status:** Defined.
  - **Result size:** $4 \times 3$.

- **Product $AD$:**
  - Dimensions: $A_{2\times 3}$ and $D_{2\times 2}$.
  - The number of columns of $A$ ($3$) does not match the number of rows of $D$ ($2$).
  - **Status:** Not defined.

- **Product $DA$:**
  - Dimensions: $D_{2\times 2}$ and $A_{2\times 3}$.
  - The number of columns of $D$ ($2$) matches the number of rows of $A$ ($2$).
  - **Status:** Defined.
  - **Result size:** $2 \times 3$.
