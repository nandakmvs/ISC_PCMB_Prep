# Chapter 10: Vectors

## 1. Exhaustive Theory & Precise ISC Terminology
- **Scalar**: A quantity with only magnitude (e.g., mass, distance).
- **Vector**: A quantity with both magnitude and direction, obeying vector addition laws. Denoted as $\vec{a}$ or $\mathbf{a}$.
- **Position Vector**: The vector $\vec{OP}$ from the origin $O(0,0,0)$ to a point $P(x,y,z)$ is $x\hat{i} + y\hat{j} + z\hat{k}$.
- **Direction Cosines ($l, m, n$)**: The cosines of the angles ($\alpha, \beta, \gamma$) a vector makes with the positive x, y, and z axes. $l^2 + m^2 + n^2 = 1$.
- **Direction Ratios ($a, b, c$)**: Numbers proportional to direction cosines.
- **Collinear Vectors**: Two vectors are collinear if one is a scalar multiple of the other ($\vec{a} = \lambda\vec{b}$).
- **Scalar (Dot) Product**: $\vec{a} \cdot \vec{b} = |\vec{a}| |\vec{b}| \cos\theta$. Result is a scalar.
- **Vector (Cross) Product**: $\vec{a} \times \vec{b} = (|\vec{a}| |\vec{b}| \sin\theta) \hat{n}$. Result is a vector perpendicular to both $\vec{a}$ and $\vec{b}$.
- **Scalar Triple Product (STP)**: $[\vec{a} \ \vec{b} \ \vec{c}] = \vec{a} \cdot (\vec{b} \times \vec{c})$. Represents the volume of a parallelepiped.

## 2. Step-by-Step Derivations & Mechanisms
### Mechanism: Finding Projection of $\vec{a}$ on $\vec{b}$
1. The projection length is given by $|\vec{a}| \cos\theta$.
2. We know $\vec{a} \cdot \vec{b} = |\vec{a}| |\vec{b}| \cos\theta$.
3. Substitute to get: Projection length = $\frac{\vec{a} \cdot \vec{b}}{|\vec{b}|} = \vec{a} \cdot \hat{b}$.
4. If the *projection vector* is asked, multiply the length by the unit vector in direction of $\vec{b}$: $(\frac{\vec{a} \cdot \vec{b}}{|\vec{b}|}) \hat{b}$.

## 3. Diagram Blueprints & Labeling Checklists
- **Cross Product Right-Hand Rule Blueprint**:
  - Draw vectors $\vec{a}$ and $\vec{b}$ tail-to-tail in a plane.
  - *Checklist*: Draw an arc from $\vec{a}$ to $\vec{b}$ (angle $\theta$). Draw the resultant vector $\vec{a} \times \vec{b}$ perpendicular to the plane. Label it with $\hat{n}$.
- **Triangle Law of Addition**:
  - Draw $\vec{a}$. From the *head* of $\vec{a}$, draw $\vec{b}$. 
  - The resultant $\vec{c} = \vec{a} + \vec{b}$ is drawn from the *tail* of $\vec{a}$ to the *head* of $\vec{b}$.

## 4. "Avoid the Trap" & Distinction Tables
| Condition | Implication | Common Trap |
|-----------|-------------|-------------|
| $\vec{a} \cdot \vec{b} = 0$ | Vectors are **Perpendicular** | Assuming one of them must be zero. (They can be non-zero and orthogonal). |
| $\vec{a} \times \vec{b} = \vec{0}$ | Vectors are **Parallel / Collinear** | Writing $0$ instead of the null vector $\vec{0}$. Cross product yields a vector! |
| $[\vec{a} \ \vec{b} \ \vec{c}] = 0$ | Vectors are **Coplanar** | Forgetting this condition when proving 4 points are coplanar (form 3 vectors first). |

## 5. High-Yield Worked Model Problems

### Q1. (ISC Step-by-Step Subjective)
**Find a unit vector perpendicular to both $\vec{a} = 2\hat{i} + \hat{j} + \hat{k}$ and $\vec{b} = \hat{i} - \hat{j} + 2\hat{k}$.**
*Step 1*: The cross product gives a perpendicular vector. Let $\vec{c} = \vec{a} \times \vec{b}$.
$\vec{c} = \begin{vmatrix} \hat{i} & \hat{j} & \hat{k} \\ 2 & 1 & 1 \\ 1 & -1 & 2 \end{vmatrix}$
$= \hat{i}(2 - (-1)) - \hat{j}(4 - 1) + \hat{k}(-2 - 1)$
$= 3\hat{i} - 3\hat{j} - 3\hat{k}$.
*Step 2*: Find the magnitude of $\vec{c}$.
$|\vec{c}| = \sqrt{3^2 + (-3)^2 + (-3)^2} = \sqrt{9 + 9 + 9} = \sqrt{27} = 3\sqrt{3}$.
*Step 3*: Write the unit vector $\hat{c}$.
$\hat{c} = \pm \frac{\vec{c}}{|\vec{c}|} = \pm \frac{3\hat{i} - 3\hat{j} - 3\hat{k}}{3\sqrt{3}} = \pm (\frac{1}{\sqrt{3}}\hat{i} - \frac{1}{\sqrt{3}}\hat{j} - \frac{1}{\sqrt{3}}\hat{k})$.

### Q2. (JEE Speed Method)
**If $|\vec{a} + \vec{b}| = |\vec{a} - \vec{b}|$, find the angle between $\vec{a}$ and $\vec{b}$.**
*Shortcut*: Square both sides directly.
$|\vec{a}|^2 + |\vec{b}|^2 + 2\vec{a}\cdot\vec{b} = |\vec{a}|^2 + |\vec{b}|^2 - 2\vec{a}\cdot\vec{b}$.
$4\vec{a}\cdot\vec{b} = 0 \implies \vec{a}\cdot\vec{b} = 0$.
Angle is $90^\circ$ or $\frac{\pi}{2}$.
