# Chapter 10: Vectors

## 1. Exhaustive Theory & Precise ISC Terminology

### 1.1 Scalars and Vectors
*   **Scalar Quantity:** A quantity that has only magnitude and no direction (e.g., mass, volume, temperature, work, distance).
*   **Vector Quantity:** A quantity that has both magnitude and direction, and obeys the laws of vector addition (e.g., displacement, velocity, force, acceleration).

### 1.2 Basic Terminology and Notations
*   **Directed Line Segment:** A line segment with a specified direction. If it starts at $A$ and ends at $B$, it is denoted as $\vec{AB}$.
*   **Magnitude:** The length of the vector $\vec{AB}$ is its magnitude, denoted by $|\vec{AB}|$. It is a non-negative scalar.
*   **Position Vector:** Let $O$ be the origin. The vector $\vec{OP}$ associated with a point $P(x, y, z)$ is called the **Position Vector** of $P$, often denoted by $\vec{r}$.
    *   $\vec{r} = x\hat{i} + y\hat{j} + z\hat{k}$
    *   Magnitude: $|\vec{r}| = \sqrt{x^2 + y^2 + z^2}$

### 1.3 Direction Cosines and Direction Ratios
*   **Direction Angles:** The angles $\alpha, \beta, \gamma$ made by the position vector $\vec{r} = \vec{OP}$ with the positive directions of $x, y, z$-axes respectively.
*   **Direction Cosines (d.c.'s):** The cosine values of the direction angles, i.e., $l = \cos \alpha$, $m = \cos \beta$, $n = \cos \gamma$.
    *   **Fundamental Identity:** $l^2 + m^2 + n^2 = 1$
*   **Direction Ratios (d.r.'s):** Any three numbers $a, b, c$ proportional to the direction cosines.
    *   $l = \frac{a}{\sqrt{a^2+b^2+c^2}}$, $m = \frac{b}{\sqrt{a^2+b^2+c^2}}$, $n = \frac{c}{\sqrt{a^2+b^2+c^2}}$ (with same or alternate signs).
    *   For a vector $\vec{r} = a\hat{i} + b\hat{j} + c\hat{k}$, the scalar components $a, b, c$ are its direction ratios.

### 1.4 Types of Vectors
*   **Zero Vector (Null Vector):** A vector whose initial and terminal points coincide. Denoted by $\vec{0}$. Its magnitude is zero and it has an arbitrary direction.
*   **Unit Vector:** A vector whose magnitude is unity (1). A unit vector in the direction of a given vector $\vec{a}$ is denoted by $\hat{a}$. Formula: $\hat{a} = \frac{\vec{a}}{|\vec{a}|}$.
*   **Co-initial Vectors:** Vectors having the same initial point.
*   **Collinear Vectors:** Vectors which are parallel to the same line, irrespective of their magnitudes and directions.
*   **Equal Vectors:** Two vectors $\vec{a}$ and $\vec{b}$ are equal if they have the same magnitude and the same direction.
*   **Negative of a Vector:** A vector having the same magnitude as a given vector but opposite in direction. Denoted by $-\vec{a}$.
*   **Coplanar Vectors:** Vectors that lie in the same plane or are parallel to the same plane.

### 1.5 Algebra of Vectors
*   **Addition of Vectors:**
    *   **Triangle Law of Vector Addition:** If two vectors are represented by two sides of a triangle in sequence, their sum is represented by the third side taken in the opposite order.
    *   **Parallelogram Law of Vector Addition:** If two vectors are represented by the adjacent sides of a parallelogram, their sum is represented by the diagonal passing through their common point.
*   **Properties of Vector Addition:** Commutative ($\vec{a} + \vec{b} = \vec{b} + \vec{a}$) and Associative.
*   **Multiplication of a Vector by a Scalar:** If $\lambda$ is a scalar and $\vec{a}$ is a vector, $\lambda\vec{a}$ is a vector whose magnitude is $|\lambda||\vec{a}|$ and direction is same as $\vec{a}$ if $\lambda > 0$, and opposite if $\lambda < 0$.

### 1.6 Products of Vectors
*   **Scalar (Dot) Product:** $\vec{a} \cdot \vec{b} = |\vec{a}| |\vec{b}| \cos \theta$, where $\theta$ is the angle between them.
    *   If $\vec{a} \cdot \vec{b} = 0$ (for non-zero vectors), they are **perpendicular/orthogonal**.
    *   Properties: Commutative ($\vec{a} \cdot \vec{b} = \vec{b} \cdot \vec{a}$).
*   **Vector (Cross) Product:** $\vec{a} \times \vec{b} = |\vec{a}| |\vec{b}| \sin \theta \hat{n}$, where $\hat{n}$ is a unit vector perpendicular to both $\vec{a}$ and $\vec{b}$ (Right-Hand Thumb Rule).
    *   If $\vec{a} \times \vec{b} = \vec{0}$ (for non-zero vectors), they are **parallel/collinear**.
    *   Properties: Anti-commutative ($\vec{a} \times \vec{b} = -(\vec{b} \times \vec{a})$).
*   **Scalar Triple Product (STP):** $[\vec{a} \vec{b} \vec{c}] = \vec{a} \cdot (\vec{b} \times \vec{c})$.
    *   Represents the **Volume of a Parallelepiped** with coterminous edges $\vec{a}, \vec{b}, \vec{c}$.
    *   Condition for Coplanarity: $[\vec{a} \vec{b} \vec{c}] = 0$.

## 2. Step-by-Step Derivations & Mechanisms

### 2.1 Section Formula (Internal Division)
**Statement:** The position vector $\vec{r}$ of a point $R$ which divides the line segment joining the points $P$ and $Q$ whose position vectors are $\vec{a}$ and $\vec{b}$ respectively, internally in the ratio $m:n$ is $\vec{r} = \frac{m\vec{b} + n\vec{a}}{m+n}$.
**Derivation:**
1.  Let $O$ be the origin. $\vec{OP} = \vec{a}$, $\vec{OQ} = \vec{b}$, and $\vec{OR} = \vec{r}$.
2.  Given $R$ divides $PQ$ internally in ratio $m:n$, so $\frac{PR}{RQ} = \frac{m}{n} \implies n(PR) = m(RQ)$.
3.  In terms of vectors, since they have the same direction: $n\vec{PR} = m\vec{RQ}$.
4.  Express vectors in terms of position vectors: $\vec{PR} = \vec{r} - \vec{a}$ and $\vec{RQ} = \vec{b} - \vec{r}$.
5.  Substitute into the equation: $n(\vec{r} - \vec{a}) = m(\vec{b} - \vec{r})$.
6.  Expand: $n\vec{r} - n\vec{a} = m\vec{b} - m\vec{r}$.
7.  Group $\vec{r}$ terms: $n\vec{r} + m\vec{r} = m\vec{b} + n\vec{a}$.
8.  Factor out $\vec{r}$: $(m+n)\vec{r} = m\vec{b} + n\vec{a}$.
9.  Final Formula: $\vec{r} = \frac{m\vec{b} + n\vec{a}}{m+n}$. *(For external division, replace $n$ with $-n$)*.

### 2.2 Projection of a Vector on a Line
**Mechanism:** Find the projection of vector $\vec{a}$ on vector $\vec{b}$.
1.  Let $\theta$ be the angle between $\vec{a}$ and $\vec{b}$.
2.  Geometrically, the projection of $\vec{a}$ on $\vec{b}$ is $|\vec{a}|\cos\theta$.
3.  From the definition of Dot Product: $\vec{a} \cdot \vec{b} = |\vec{a}| |\vec{b}| \cos \theta$.
4.  Isolate $|\vec{a}|\cos\theta$: $|\vec{a}|\cos\theta = \frac{\vec{a} \cdot \vec{b}}{|\vec{b}|}$.
5.  This can be rewritten using the unit vector $\hat{b}$: Projection = $\vec{a} \cdot \hat{b}$.
*(ISC Grading Note: Always state the formula $\frac{\vec{a} \cdot \vec{b}}{|\vec{b}|}$ before plugging in components).*

### 2.3 Volume of a Parallelepiped (Scalar Triple Product)
**Derivation:**
1.  Consider a parallelepiped with coterminous edges represented by vectors $\vec{a}$, $\vec{b}$, and $\vec{c}$.
2.  The area of the base parallelogram formed by $\vec{b}$ and $\vec{c}$ is given by $|\vec{b} \times \vec{c}|$.
3.  The direction of $\vec{n} = \vec{b} \times \vec{c}$ is perpendicular to the base.
4.  The height $h$ of the parallelepiped is the projection of vector $\vec{a}$ along the normal $\vec{n}$.
5.  $h = |\vec{a}| |\cos\theta|$, where $\theta$ is the angle between $\vec{a}$ and $\vec{n}$.
6.  Volume $V = \text{Base Area} \times \text{Height} = |\vec{b} \times \vec{c}| \cdot |\vec{a}| |\cos\theta|$.
7.  By definition of dot product: $V = |\vec{a} \cdot (\vec{b} \times \vec{c})| = |[\vec{a} \vec{b} \vec{c}]|$.

### 2.4 Lagrange's Identity
**Statement:** $|\vec{a} \times \vec{b}|^2 = |\vec{a}|^2|\vec{b}|^2 - (\vec{a} \cdot \vec{b})^2$
**Derivation:**
1.  LHS: $|\vec{a} \times \vec{b}|^2 = (|\vec{a}||\vec{b}|\sin\theta)^2 = |\vec{a}|^2|\vec{b}|^2\sin^2\theta$.
2.  Substitute $\sin^2\theta = 1 - \cos^2\theta$: $= |\vec{a}|^2|\vec{b}|^2(1 - \cos^2\theta)$.
3.  Expand: $= |\vec{a}|^2|\vec{b}|^2 - |\vec{a}|^2|\vec{b}|^2\cos^2\theta$.
4.  Recognize the dot product squared: $= |\vec{a}|^2|\vec{b}|^2 - (|\vec{a}||\vec{b}|\cos\theta)^2$.
5.  RHS: $= |\vec{a}|^2|\vec{b}|^2 - (\vec{a} \cdot \vec{b})^2$. (Proved).

## 3. Diagram Blueprints & Labeling Checklists

### 3.1 Triangle & Parallelogram Laws of Addition
**Blueprint for Triangle Law:**
*   Draw vector $\vec{a}$ from point $A$ to $B$. Label with arrow $\rightarrow$ over line $AB$.
*   Draw vector $\vec{b}$ from point $B$ (tail of $\vec{b}$ at head of $\vec{a}$) to $C$.
*   Draw resultant vector $\vec{c}$ from $A$ (initial point) to $C$ (final point).
*   **ISC Checklist:** Show directional arrows clearly. Label vectors as $\vec{a}, \vec{b}, \vec{a}+\vec{b}$. Write statement: $\vec{AB} + \vec{BC} = \vec{AC}$.

**Blueprint for Parallelogram Law:**
*   Draw vectors $\vec{a}$ and $\vec{b}$ co-initiating from origin $O$.
*   Complete the parallelogram $OACB$.
*   Draw the diagonal from $O$ to $C$. This is the resultant $\vec{a} + \vec{b}$.
*   **ISC Checklist:** Label adjacent sides $\vec{OA} = \vec{a}$, $\vec{OB} = \vec{b}$. Label diagonal $\vec{OC} = \vec{a} + \vec{b}$. Use dashed lines for constructing parallel sides $AC$ and $BC$.

### 3.2 Direction Cosines Geometry (3D Axes)
**Blueprint:**
*   Draw standard 3D Cartesian axes: $X, Y, Z$ (ensure right-handed orientation).
*   Draw a position vector $\vec{r}$ from Origin $O$ to point $P(x,y,z)$.
*   Draw curved angle markers from positive $X$-axis to $\vec{OP}$ (label $\alpha$), from $Y$-axis to $\vec{OP}$ (label $\beta$), and from $Z$-axis to $\vec{OP}$ (label $\gamma$).
*   **ISC Checklist:** Axes must be labeled $X, Y, Z$. Origin $O$. Angles $\alpha, \beta, \gamma$ must originate from the axes and terminate at the vector.

### 3.3 Projection of a Vector
**Blueprint:**
*   Draw vector $\vec{b}$ horizontally.
*   Draw vector $\vec{a}$ starting from the same tail (co-initial).
*   Drop a perpendicular from the head of $\vec{a}$ down to the line of vector $\vec{b}$.
*   The segment on $\vec{b}$ from the origin to the foot of the perpendicular is the projection.
*   **ISC Checklist:** Mark the angle $\theta$. Mark the right angle $\perp$ at the foot. Label the projection segment as $|\vec{a}|\cos\theta$.

## 4. "Avoid the Trap" & Distinction Tables

### 4.1 Objective vs Subjective Traps
| Trap Description | How to Avoid / ISC Expectation |
| :--- | :--- |
| **Trap 1: Confusing Direction Ratios (d.r.) and Direction Cosines (d.c.)** | D.c.'s are normalized; their squares sum to 1 ($l^2+m^2+n^2=1$). D.r.'s are just proportional. Always check if $a^2+b^2+c^2=1$ before assuming they are d.c.'s. |
| **Trap 2: Forgetting Vector Notation ($\vec{a}$ vs $a$)** | **CRITICAL ISC SUBJECTIVE PENALTY.** If you write $a$ instead of $\vec{a}$, examiners deduct marks for treating a vector as a scalar. Always use arrows ($\vec{a}$) or caps ($\hat{i}$) appropriately. |
| **Trap 3: Cross Product Commutativity** | $\vec{a} \times \vec{b} \neq \vec{b} \times \vec{a}$. The cross product is **anti-commutative**: $\vec{a} \times \vec{b} = -(\vec{b} \times \vec{a})$. Forgetting the negative sign alters the normal's direction. |
| **Trap 4: Dividing by a Vector** | Division by a vector is undefined. Never write expressions like $\frac{\vec{a}}{\vec{b}}$. You can only divide by a scalar (magnitude), e.g., $\frac{\vec{a}}{|\vec{a}|}$. |
| **Trap 5: Area of Triangle vs Parallelogram** | Area of Triangle = $\frac{1}{2}|\vec{a} \times \vec{b}|$. Area of Parallelogram = $|\vec{a} \times \vec{b}|$. Don't mix up the $\frac{1}{2}$ factor. |

### 4.2 Distinction: Dot Product vs Cross Product
| Feature | Scalar (Dot) Product | Vector (Cross) Product |
| :--- | :--- | :--- |
| **Result** | A Scalar quantity. | A Vector quantity. |
| **Definition** | $\vec{a} \cdot \vec{b} = |\vec{a}||\vec{b}|\cos\theta$ | $\vec{a} \times \vec{b} = |\vec{a}||\vec{b}|\sin\theta \hat{n}$ |
| **Commutativity**| Commutative: $\vec{a} \cdot \vec{b} = \vec{b} \cdot \vec{a}$ | Anti-commutative: $\vec{a} \times \vec{b} = -(\vec{b} \times \vec{a})$ |
| **Perpendicularity**| $\vec{a} \cdot \vec{b} = 0 \implies \vec{a} \perp \vec{b}$ | $\vec{a} \cdot \vec{b} = 0$ provides no info on cross product (unless vectors are null). |
| **Collinearity** | No direct condition (magnitude test needed). | $\vec{a} \times \vec{b} = \vec{0} \implies \vec{a} \parallel \vec{b}$ |
| **Unit Vectors** | $\hat{i} \cdot \hat{i} = 1$, $\hat{i} \cdot \hat{j} = 0$ | $\hat{i} \times \hat{i} = \vec{0}$, $\hat{i} \times \hat{j} = \hat{k}$ |

### 4.3 Coplanarity vs Collinearity
*   **Collinear:** Two vectors are collinear if one is a scalar multiple of the other ($\vec{a} = \lambda\vec{b}$) or their cross product is zero ($\vec{a} \times \vec{b} = \vec{0}$).
*   **Coplanar:** Three vectors are coplanar if their Scalar Triple Product is zero ($[\vec{a} \vec{b} \vec{c}] = 0$).

## 5. High-Yield Worked Model Problems

### Problem 1: Direction Cosines and Unit Vectors
**Question:** Find the direction cosines of the vector joining the points $A(1, 2, -3)$ and $B(-1, -2, 1)$, directed from $A$ to $B$.
**ISC Step-by-Step:**
1.  **Find Vector:** $\vec{AB} = (\text{Position vector of } B) - (\text{Position vector of } A)$.
    $\vec{AB} = (-1 - 1)\hat{i} + (-2 - 2)\hat{j} + (1 - (-3))\hat{k} = -2\hat{i} - 4\hat{j} + 4\hat{k}$.
2.  **Find Magnitude:** $|\vec{AB}| = \sqrt{(-2)^2 + (-4)^2 + 4^2} = \sqrt{4 + 16 + 16} = \sqrt{36} = 6$.
3.  **Find Direction Cosines:** The direction ratios are $a=-2, b=-4, c=4$.
    $l = \frac{a}{|\vec{AB}|} = \frac{-2}{6} = -\frac{1}{3}$
    $m = \frac{b}{|\vec{AB}|} = \frac{-4}{6} = -\frac{2}{3}$
    $n = \frac{c}{|\vec{AB}|} = \frac{4}{6} = \frac{2}{3}$
**Answer:** $(-\frac{1}{3}, -\frac{2}{3}, \frac{2}{3})$
*(NEET/JEE Speed Trick: Form vector, divide coefficients directly by magnitude in your head).*

### Problem 2: Dot Product and Angle Between Vectors
**Question:** Find the angle between two vectors $\vec{a} = \hat{i} + \hat{j} - \hat{k}$ and $\vec{b} = \hat{i} - \hat{j} + \hat{k}$.
**ISC Step-by-Step:**
1.  **State Formula:** $\cos\theta = \frac{\vec{a} \cdot \vec{b}}{|\vec{a}||\vec{b}|}$
2.  **Calculate Dot Product:** $\vec{a} \cdot \vec{b} = (1)(1) + (1)(-1) + (-1)(1) = 1 - 1 - 1 = -1$.
3.  **Calculate Magnitudes:**
    $|\vec{a}| = \sqrt{1^2 + 1^2 + (-1)^2} = \sqrt{3}$
    $|\vec{b}| = \sqrt{1^2 + (-1)^2 + 1^2} = \sqrt{3}$
4.  **Substitute:** $\cos\theta = \frac{-1}{\sqrt{3}\sqrt{3}} = -\frac{1}{3}$
5.  **Final Answer:** $\theta = \cos^{-1}(-\frac{1}{3})$.

### Problem 3: Cross Product and Orthogonal Vectors
**Question:** Find a unit vector perpendicular to both vectors $\vec{a} = 2\hat{i} + \hat{j} + \hat{k}$ and $\vec{b} = \hat{i} - \hat{j} + 2\hat{k}$.
**ISC Step-by-Step:**
1.  **Concept:** A vector perpendicular to both is given by their cross product, $\vec{c} = \vec{a} \times \vec{b}$.
2.  **Calculate Cross Product:**
    $\vec{a} \times \vec{b} = \begin{vmatrix} \hat{i} & \hat{j} & \hat{k} \\ 2 & 1 & 1 \\ 1 & -1 & 2 \end{vmatrix}$
    $= \hat{i}(2 - (-1)) - \hat{j}(4 - 1) + \hat{k}(-2 - 1)$
    $= 3\hat{i} - 3\hat{j} - 3\hat{k}$
3.  **Find Magnitude of Cross Product:**
    $|\vec{a} \times \vec{b}| = \sqrt{3^2 + (-3)^2 + (-3)^2} = \sqrt{9+9+9} = \sqrt{27} = 3\sqrt{3}$.
4.  **Find Unit Vector:**
    $\hat{n} = \pm \frac{\vec{a} \times \vec{b}}{|\vec{a} \times \vec{b}|} = \pm \frac{3\hat{i} - 3\hat{j} - 3\hat{k}}{3\sqrt{3}} = \pm \frac{1}{\sqrt{3}}(\hat{i} - \hat{j} - \hat{k})$.
*(Note: Always include the $\pm$ sign in subjective board exams unless specific direction is asked).*

### Problem 4: Scalar Triple Product and Coplanarity
**Question:** Show that the vectors $\vec{a} = \hat{i} - 2\hat{j} + 3\hat{k}$, $\vec{b} = -2\hat{i} + 3\hat{j} - 4\hat{k}$, and $\vec{c} = \hat{i} - 3\hat{j} + 5\hat{k}$ are coplanar.
**ISC Step-by-Step:**
1.  **State Condition:** Three vectors are coplanar if their Scalar Triple Product $[\vec{a} \vec{b} \vec{c}] = 0$.
2.  **Set up Determinant:**
    $[\vec{a} \vec{b} \vec{c}] = \begin{vmatrix} 1 & -2 & 3 \\ -2 & 3 & -4 \\ 1 & -3 & 5 \end{vmatrix}$
3.  **Evaluate Determinant:**
    $= 1(15 - 12) - (-2)(-10 - (-4)) + 3(6 - 3)$
    $= 1(3) + 2(-6) + 3(3)$
    $= 3 - 12 + 9 = 0$.
4.  **Conclusion:** Since the Scalar Triple Product is zero, the given vectors are coplanar. Hence Proved.
*(JEE Speed Tip: Just mentally check if one vector is a linear combination of the other two, e.g., $\vec{c} = 3\vec{a} + \vec{b}$? Yes! Proved instantly).*
