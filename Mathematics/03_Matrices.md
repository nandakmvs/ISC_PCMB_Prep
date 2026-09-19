# Chapter 3: Matrices

## 1. Exhaustive Theory & Precise ISC Terminology

A **Matrix** is an ordered rectangular array of numbers or functions. Plural is matrices.
**Order of a Matrix**: A matrix with $m$ rows and $n$ columns is of order $m \times n$.
**Elements**: $a_{ij}$ denotes the element in the $i$-th row and $j$-th column.

### Types of Matrices
1. **Column Matrix**: Has only one column (order $m \times 1$).
2. **Row Matrix**: Has only one row (order $1 \times n$).
3. **Square Matrix**: Number of rows equals number of columns ($m = n$).
4. **Diagonal Matrix**: A square matrix whose non-diagonal elements are zero ($a_{ij} = 0$ for $i \neq j$).
5. **Scalar Matrix**: A diagonal matrix where all diagonal elements are equal.
6. **Identity Matrix (I)**: A scalar matrix where all diagonal elements are 1.
7. **Zero/Null Matrix (O)**: All elements are zero.

### Matrix Operations
- **Equality**: Two matrices are equal if they have the same order and corresponding elements are equal.
- **Addition**: Defined only for matrices of the same order. Add corresponding elements.
- **Scalar Multiplication**: Multiply every element by the scalar $k$.
- **Matrix Multiplication ($AB$)**: Defined if number of columns of A = number of rows of B. The element $c_{ij}$ is the dot product of the $i$-th row of A and the $j$-th column of B. Not commutative ($AB \neq BA$ generally).

### Transpose & Special Matrices
**Transpose ($A^T$ or $A'$):** Matrix obtained by interchanging rows and columns.
- **Symmetric Matrix**: $A^T = A$ ($a_{ij} = a_{ji}$).
- **Skew-Symmetric Matrix**: $A^T = -A$ ($a_{ij} = -a_{ji}$). Diagonal elements must be zero.

**Invertible Matrices**: If there exists a matrix $B$ such that $AB = BA = I$, then $B$ is the **Inverse** of $A$, denoted $A^{-1}$. Only non-singular square matrices have inverses.

## 2. Step-by-Step Derivations & Mechanisms

**Theorem: Any square matrix can be expressed as the sum of a symmetric and a skew-symmetric matrix.**
Let $A$ be a square matrix. We can write:
$A = \frac{1}{2}(A + A^T) + \frac{1}{2}(A - A^T)$
Let $P = \frac{1}{2}(A + A^T)$ and $Q = \frac{1}{2}(A - A^T)$.
Check $P^T = [\frac{1}{2}(A + A^T)]^T = \frac{1}{2}(A^T + (A^T)^T) = \frac{1}{2}(A^T + A) = P$. (So P is symmetric).
Check $Q^T = [\frac{1}{2}(A - A^T)]^T = \frac{1}{2}(A^T - (A^T)^T) = \frac{1}{2}(A^T - A) = -Q$. (So Q is skew-symmetric).
Hence proved.

**Mechanism for Finding Inverse using Elementary Row Operations:**
1. Write $A = IA$.
2. Apply a sequence of elementary row operations (swapping rows, multiplying a row by a scalar, adding a multiple of one row to another) to the $A$ on the LHS until it becomes $I$.
3. Simultaneously apply the exact same operations to the $I$ on the RHS.
4. When LHS becomes $I$, the RHS becomes $A^{-1}$.

## 3. Diagram Blueprints & Labeling Checklists

- **Matrix Multiplication Blueprint**:
  - Matrix $A_{m \times n} \times B_{n \times p} = C_{m \times p}$.
  - Draw arrows: horizontal arrow across a row in $A$, vertical arrow down a column in $B$.
  - This visualizes the dot product forming a single element in $C$.

## 4. "Avoid the Trap" & Distinction Tables

| Concept 1 | Concept 2 | Key Distinction / Trap |
| :--- | :--- | :--- |
| Commutativity in Addition | Commutativity in Multiplication | $A+B = B+A$ always holds. $AB = BA$ **rarely holds**. Never assume $AB=BA$. |
| Transpose of Sum | Transpose of Product | $(A+B)^T = A^T + B^T$. However, $(AB)^T = B^T A^T$ (Reversal Law). The order swaps! |
| Null Matrix Product | Real Number product | If $AB = 0$, it is NOT necessary that $A = 0$ or $B = 0$. Two non-zero matrices can have a zero product. |

## 5. High-Yield Worked Model Problems

**Problem (ISC Step-by-Step)**: Express matrix $A = \begin{pmatrix} 1 & 5 \\ -1 & 2 \end{pmatrix}$ as the sum of a symmetric and a skew-symmetric matrix.
**Solution**:
1. Find $A^T = \begin{pmatrix} 1 & -1 \\ 5 & 2 \end{pmatrix}$.
2. Symmetric part $P = \frac{1}{2}(A + A^T) = \frac{1}{2} \left[ \begin{pmatrix} 1 & 5 \\ -1 & 2 \end{pmatrix} + \begin{pmatrix} 1 & -1 \\ 5 & 2 \end{pmatrix} \right] = \frac{1}{2} \begin{pmatrix} 2 & 4 \\ 4 & 4 \end{pmatrix} = \begin{pmatrix} 1 & 2 \\ 2 & 2 \end{pmatrix}$.
3. Skew-Symmetric part $Q = \frac{1}{2}(A - A^T) = \frac{1}{2} \left[ \begin{pmatrix} 1 & 5 \\ -1 & 2 \end{pmatrix} - \begin{pmatrix} 1 & -1 \\ 5 & 2 \end{pmatrix} \right] = \frac{1}{2} \begin{pmatrix} 0 & 6 \\ -6 & 0 \end{pmatrix} = \begin{pmatrix} 0 & 3 \\ -3 & 0 \end{pmatrix}$.
4. Conclusion: $A = P + Q = \begin{pmatrix} 1 & 2 \\ 2 & 2 \end{pmatrix} + \begin{pmatrix} 0 & 3 \\ -3 & 0 \end{pmatrix}$.

**Problem (NEET/JEE Speed Method)**: If $A = \begin{pmatrix} \alpha & \beta \\ \gamma & -\alpha \end{pmatrix}$ is such that $A^2 = I$, then find the relation between $\alpha, \beta, \gamma$.
**Solution**:
$A^2 = \begin{pmatrix} \alpha & \beta \\ \gamma & -\alpha \end{pmatrix} \begin{pmatrix} \alpha & \beta \\ \gamma & -\alpha \end{pmatrix} = \begin{pmatrix} \alpha^2+\beta\gamma & \alpha\beta-\beta\alpha \\ \gamma\alpha-\alpha\gamma & \beta\gamma+\alpha^2 \end{pmatrix} = \begin{pmatrix} \alpha^2+\beta\gamma & 0 \\ 0 & \alpha^2+\beta\gamma \end{pmatrix}$.
Since $A^2 = I = \begin{pmatrix} 1 & 0 \\ 0 & 1 \end{pmatrix}$, we equate elements:
$\alpha^2 + \beta\gamma = 1 \implies 1 - \alpha^2 - \beta\gamma = 0$.
Speed tip: For a $2 \times 2$ matrix $A$ where trace (sum of diagonal elements) is 0, $A^2 = \text{det}(A) \cdot I$. Wait, $A^2 - (\text{Tr})A + \text{Det}(A)I = 0$ (Cayley-Hamilton theorem). Here Tr = 0, so $A^2 = -\text{Det}(A) I$. Thus $-\text{Det}(A) = 1 \implies -(-\alpha^2-\beta\gamma) = 1 \implies \alpha^2+\beta\gamma=1$.
