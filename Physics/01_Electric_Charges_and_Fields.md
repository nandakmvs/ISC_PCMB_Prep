# Chapter 01: Electric Charges and Fields

## 1. Exhaustive Theory & Precise ISC Terminology

*   **Electric Charge ($q$)**: An intrinsic property of elementary particles of matter which gives rise to electric force between various objects.
*   **Quantization of Charge**: The fact that all observable charges are always some integral multiple of elementary charge ($e = 1.6 \times 10^{-19}$ C). Mathematically, **$q = ne$** where $n \in \mathbb{Z}$.
*   **Conservation of Charge**: The total charge of an isolated system remains constant.
*   **Coulomb's Law**: The electrostatic force of interaction between two point charges is directly proportional to the product of the charges and inversely proportional to the square of the distance between them.
    *   Formula: **$F = \frac{1}{4\pi\epsilon_0} \frac{|q_1 q_2|}{r^2}$**
    *   **Permittivity of Free Space ($\epsilon_0$)**: $8.854 \times 10^{-12} \text{ C}^2\text{N}^{-1}\text{m}^{-2}$.
*   **Principle of Superposition**: Force on any charge due to a number of other charges is the vector sum of all the forces on that charge due to the other charges, taken one at a time.
*   **Electric Field ($\vec{E}$)**: The electric force per unit positive test charge. **$\vec{E} = \lim_{q_0 \to 0} \frac{\vec{F}}{q_0}$**.
*   **Electric Field Lines**: An imaginary curve drawn in such a way that the tangent at any point gives the direction of the electric field at that point. They originate from positive charges and terminate on negative charges. They **never intersect**.
*   **Electric Dipole**: A pair of equal and opposite point charges separated by a small distance.
    *   **Electric Dipole Moment ($\vec{p}$)**: A vector quantity whose magnitude is $q \times 2a$ (where $2a$ is the dipole length) and directed from negative to positive charge.
*   **Torque on a Dipole**: $\vec{\tau} = \vec{p} \times \vec{E}$.
*   **Electric Flux ($\Phi_E$)**: The total number of electric field lines crossing a given area. **$\Phi_E = \oint \vec{E} \cdot d\vec{A}$**.
*   **Gauss's Theorem**: The total electric flux through any closed surface is equal to $\frac{1}{\epsilon_0}$ times the net charge enclosed by the surface. **$\oint \vec{E} \cdot d\vec{A} = \frac{q_{\text{enclosed}}}{\epsilon_0}$**.

## 2. Step-by-Step Derivations & Mechanisms

### A. Electric Field on the Axial Line of a Dipole
1.  Consider a dipole with charges $-q$ and $+q$ separated by $2a$.
2.  Let $P$ be a point on the axis at distance $r$ from the center $O$.
3.  Field due to $+q$: $E_+ = \frac{1}{4\pi\epsilon_0} \frac{q}{(r-a)^2}$ (directed away).
4.  Field due to $-q$: $E_- = \frac{1}{4\pi\epsilon_0} \frac{q}{(r+a)^2}$ (directed towards).
5.  Net field $E_{axial} = E_+ - E_- = \frac{1}{4\pi\epsilon_0} \left[ \frac{q}{(r-a)^2} - \frac{q}{(r+a)^2} \right]$.
6.  Simplify: $E_{axial} = \frac{1}{4\pi\epsilon_0} \frac{q(4ar)}{(r^2-a^2)^2} = \frac{1}{4\pi\epsilon_0} \frac{2pr}{(r^2-a^2)^2}$.
7.  For short dipole ($r \gg a$): **$E_{axial} \approx \frac{1}{4\pi\epsilon_0} \frac{2p}{r^3}$**.

### B. Electric Field due to an Infinitely Long Straight Uniformly Charged Wire
1.  Let $\lambda$ be the linear charge density.
2.  Consider a cylindrical Gaussian surface of radius $r$ and length $l$ coaxial with the wire.
3.  By Gauss's law: $\oint \vec{E} \cdot d\vec{A} = \frac{q_{enc}}{\epsilon_0}$.
4.  Flux through curved surface $= E(2\pi rl)$. Flux through flat ends $= 0$ (since $\vec{E} \perp d\vec{A}$).
5.  $E(2\pi rl) = \frac{\lambda l}{\epsilon_0} \implies$ **$E = \frac{\lambda}{2\pi\epsilon_0 r}$**.

## 3. Diagram Blueprints & Labeling Checklists

*   **Electric Field Lines of a Dipole**:
    *   **Checklist**:
        *   [ ] Positive charge ($+q$) on left, Negative ($-q$) on right.
        *   [ ] Lines originate at $+q$ and terminate at $-q$.
        *   [ ] Tangents to lines indicate direction.
        *   [ ] Density of lines is higher near the charges.
        *   [ ] Absolutely NO lines crossing each other.
*   **Gaussian Cylinder for Line Charge**:
    *   **Checklist**:
        *   [ ] Draw a straight wire with '+' signs.
        *   [ ] Draw a cylinder around a segment of length $l$.
        *   [ ] Label radius $r$.
        *   [ ] Show area vector $d\vec{A}$ and Field $\vec{E}$ on the curved surface (parallel).
        *   [ ] Show area vector $d\vec{A}$ and Field $\vec{E}$ on the flat caps (perpendicular).

## 4. "Avoid the Trap" & Distinction Tables

*   **TRAP ALERT (Subjective)**: When defining Electric Field intensity, students often forget the limit term $\lim_{q_0 \to 0}$. This is crucial because the test charge itself shouldn't disturb the source configuration!
*   **TRAP ALERT (Objective)**: Torque on a dipole is zero at $\theta = 0^\circ$ (stable equilibrium) and $\theta = 180^\circ$ (unstable equilibrium). Be careful which equilibrium the question asks for.

| Feature | Electric Field ($\vec{E}$) | Electric Force ($\vec{F}$) |
| :--- | :--- | :--- |
| **Dependence** | Independent of test charge | Depends on test charge |
| **Vector Nature** | Direction of force on $+1C$ charge | Given by Coulomb's law including sign |
| **Units** | N/C or V/m | Newtons (N) |

## 5. High-Yield Worked Model Problems

### Problem 1 (ISC Focus - Step-by-Step)
**Q: Using Gauss's theorem, derive an expression for the electric field due to a uniformly charged infinite plane sheet of surface charge density $\sigma$.**
*   **Step 1: Setup**: Consider a thin infinite sheet with uniform surface charge density $\sigma$.
*   **Step 2: Gaussian Surface**: Choose a cylindrical pillbox of cross-sectional area $A$ piercing the sheet, extending length $r$ on both sides.
*   **Step 3: Flux Calculation**: The flux only passes through the two circular caps. $\Phi = \oint \vec{E}\cdot d\vec{A} = EA + EA = 2EA$.
*   **Step 4: Enclosed Charge**: $q_{enclosed} = \sigma A$.
*   **Step 5: Apply Gauss's Law**: $2EA = \frac{\sigma A}{\epsilon_0} \implies$ **$E = \frac{\sigma}{2\epsilon_0}$**.
*   **Conclusion**: Note that $E$ is independent of $r$.

### Problem 2 (NEET/JEE Focus - Speed Method)
**Q: Two point charges $+4e$ and $+e$ are kept at a distance 'a' apart. Where should a third charge $q$ be placed so that the system is in equilibrium?**
*   **Standard Method**: Equate forces: $F_1 = F_2 \implies k(4e)(q)/x^2 = k(e)(q)/(a-x)^2$. Solve quadratic.
*   **Speed Trick**: Distance of null point from smaller charge $Q_1$ is $x = \frac{\sqrt{Q_1}}{\sqrt{Q_2} + \sqrt{Q_1}} \times d$.
*   **Execution**: $x$ (from $+e$) = $\frac{\sqrt{e}}{\sqrt{4e} + \sqrt{e}} \times a = \frac{1}{2+1}a = \frac{a}{3}$. So, $a/3$ from $+e$ (or $2a/3$ from $+4e$).
