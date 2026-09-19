# Chapter 10: Vector Algebra

## 1. Exhaustive Theory & Precise ISC Terminology

A **Vector** has both magnitude and direction. A scalar has only magnitude.
- **Position Vector**: Vector $\vec{r} = \vec{OP}$ from origin $O(0,0,0)$ to point $P(x,y,z)$. $\vec{r} = x\hat{i} + y\hat{j} + z\hat{k}$. Magnitude $|\vec{r}| = \sqrt{x^2+y^2+z^2}$.
- **Direction Cosines ($l, m, n$)**: The cosines of angles $\alpha, \beta, \gamma$ made by the vector with positive x, y, z axes. $l^2 + m^2 + n^2 = 1$.
- **Direction Ratios ($a, b, c$)**: Numbers proportional to direction cosines. For vector $x\hat{i} + y\hat{j} + z\hat{k}$, direction ratios are $x, y, z$.

### Types of Vectors
- **Zero Vector**: Zero magnitude, arbitrary direction ($\vec{0}$).
- **Unit Vector**: Magnitude of 1. Unit vector in direction of $\vec{a}$ is $\hat{a} = \frac{\vec{a}}{|\vec{a}|}$.
- **Collinear Vectors**: Parallel to the same line, irrespective of magnitude and direction. $\vec{a} = \lambda\vec{b}$.
- **Coplanar Vectors**: Vectors lying in the same plane or parallel to the same plane.

### Vector Operations
1. **Addition (Triangle/Parallelogram Law)**: $\vec{AB} + \vec{BC} = \vec{AC}$.
2. **Scalar (Dot) Product**: $\vec{a} \cdot \vec{b} = |\vec{a}| |\vec{b}| \cos\theta$. Result is a scalar. $\vec{a} \cdot \vec{b} = 0 \iff \vec{a} \perp \vec{b}$.
   - Projection of $\vec{a}$ on $\vec{b}$ is $\frac{\vec{a} \cdot \vec{b}}{|\vec{b}|}$.
3. **Vector (Cross) Product**: $\vec{a} \times \vec{b} = |\vec{a}| |\vec{b}| \sin\theta \hat{n}$, where $\hat{n}$ is a unit vector perpendicular to both, given by Right Hand Rule. Result is a vector. $\vec{a} \times \vec{b} = \vec{0} \iff \vec{a} \parallel \vec{b}$.
   - Area of parallelogram with adjacent sides $\vec{a}, \vec{b}$ is $|\vec{a} \times \vec{b}|$. Area of triangle is $\frac{1}{2}|\vec{a} \times \vec{b}|$.
4. **Scalar Triple Product (Box Product)**: $[\vec{a} \vec{b} \vec{c}] = \vec{a} \cdot (\vec{b} \times \vec{c})$. Represents volume of parallelepiped. $[\vec{a} \vec{b} \vec{c}] = 0 \iff \vec{a}, \vec{b}, \vec{c}$ are coplanar.

## 2. Step-by-Step Derivations & Mechanisms

**Mechanism: Finding a vector of magnitude $k$ perpendicular to both $\vec{a}$ and $\vec{b}$:**
1. Compute the cross product $\vec{c} = \vec{a} \times \vec{b}$ using a determinant. This gives a perpendicular vector.
2. Find the magnitude $|\vec{c}|$.
3. Find the unit perpendicular vector $\hat{n} = \pm \frac{\vec{c}}{|\vec{c}|}$.
4. Multiply by magnitude $k$: Required vector = $\pm k \hat{n}$.

## 3. Diagram Blueprints & Labeling Checklists

- **Right Hand Rule for Cross Product**:
  - Draw vectors $\vec{a}$ and $\vec{b}$ tail-to-tail in a horizontal plane.
  - Draw a perpendicular vertical vector $\vec{a} \times \vec{b}$.
  - Label: Curved arrow from $\vec{a}$ to $\vec{b}$ showing fingers curling, thumb points up representing the cross product direction.

## 4. "Avoid the Trap" & Distinction Tables

| Trap / Common Mistake | Strategy / Fact to Remember |
| :--- | :--- |
| Commutativity in Products | Dot product is commutative ($\vec{a}\cdot\vec{b} = \vec{b}\cdot\vec{a}$). Cross product is **anti-commutative** ($\vec{a}\times\vec{b} = -\vec{b}\times\vec{a}$). |
| Mixing up dot and cross | Remember: Dot product yields a SCALAR (number). Cross product yields a VECTOR. |
| Collinear vs Perpendicular checks | $\vec{a} \times \vec{b} = 0 \implies$ parallel/collinear. $\vec{a} \cdot \vec{b} = 0 \implies$ perpendicular. Don't swap them! |

## 5. High-Yield Worked Model Problems

**Problem (ISC Step-by-Step)**: Find the area of a parallelogram whose adjacent sides are determined by the vectors $\vec{a} = \hat{i} - \hat{j} + 3\hat{k}$ and $\vec{b} = 2\hat{i} - 7\hat{j} + \hat{k}$.
**Solution**:
1. Area of parallelogram is given by $|\vec{a} \times \vec{b}|$.
2. Compute $\vec{a} \times \vec{b} = \begin{vmatrix} \hat{i} & \hat{j} & \hat{k} \\ 1 & -1 & 3 \\ 2 & -7 & 1 \end{vmatrix}$.
3. Expansion: $\hat{i}(-1 - (-21)) - \hat{j}(1 - 6) + \hat{k}(-7 - (-2)) = 20\hat{i} + 5\hat{j} - 5\hat{k}$.
4. Calculate magnitude: $|\vec{a} \times \vec{b}| = \sqrt{(20)^2 + (5)^2 + (-5)^2} = \sqrt{400 + 25 + 25} = \sqrt{450}$.
5. Simplify: $\sqrt{450} = 15\sqrt{2}$ sq units.

**Problem (NEET/JEE Speed Method)**: If $\vec{a}, \vec{b}, \vec{c}$ are coplanar vectors, what is the value of $[2\vec{a}-\vec{b} \quad 2\vec{b}-\vec{c} \quad 2\vec{c}-\vec{a}]$?
**Solution**:
The scalar triple product is linear. Using properties of STP and determinants:
$[x\vec{a}+y\vec{b}+z\vec{c} \dots] = \text{Det}(\text{coefficients}) \times [\vec{a}\vec{b}\vec{c}]$.
Det = $\begin{vmatrix} 2 & -1 & 0 \\ 0 & 2 & -1 \\ -1 & 0 & 2 \end{vmatrix} = 2(4 - 0) - (-1)(0 - 1) + 0 = 8 - 1 = 7$.
So result is $7[\vec{a}\vec{b}\vec{c}]$.
Since $\vec{a}, \vec{b}, \vec{c}$ are coplanar, $[\vec{a}\vec{b}\vec{c}] = 0$.
Result = $7 \times 0 = 0$.
