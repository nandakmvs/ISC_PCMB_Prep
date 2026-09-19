# Chapter 02: Electrostatic Potential and Capacitors

## 1. Exhaustive Theory & Precise ISC Terminology

*   **Electrostatic Potential ($V$)**: The amount of work done by an external force in moving a unit positive charge from infinity to a point in the electric field, without acceleration. $V = \frac{W}{q_0}$. Unit: Volt (V).
*   **Potential Difference ($\Delta V$)**: The work done in moving a unit positive charge from one point to another. $V_B - V_A = \frac{W_{AB}}{q_0}$.
*   **Equipotential Surface**: A surface with a constant value of potential at all points on the surface. Work done in moving a charge on this surface is always zero.
*   **Potential Energy ($U$)**: The work done in assembling a system of charges by bringing them from infinity to their present locations. $U = \frac{1}{4\pi\epsilon_0}\frac{q_1 q_2}{r}$.
*   **Dielectrics**: Non-conducting substances that have no charge carriers but undergo electrical polarization in an external electric field.
*   **Polarization ($\vec{P}$)**: Dipole moment per unit volume.
*   **Dielectric Constant ($K$)**: The ratio of the permittivity of the medium to the permittivity of free space ($K = \frac{\epsilon}{\epsilon_0}$).
*   **Capacitance ($C$)**: The ability of a conductor to store electric charge and energy. $C = \frac{Q}{V}$. Unit: Farad (F).
*   **Parallel Plate Capacitor**: Two large plane parallel conducting plates separated by a small distance. $C = \frac{\epsilon_0 A}{d}$.

## 2. Step-by-Step Derivations & Mechanisms

### A. Electric Potential due to a Point Charge
1.  Consider a point charge $+q$ at the origin $O$. We need to find potential at point $P$ at distance $r$.
2.  Imagine a test charge $+q_0$ at distance $x$. Repulsive force $F = \frac{1}{4\pi\epsilon_0} \frac{q q_0}{x^2}$.
3.  Small work done $dW$ in moving $q_0$ by $dx$ towards $O$: $dW = \vec{F} \cdot d\vec{x} = -F dx$.
4.  Total work $W = \int_{\infty}^{r} - \frac{1}{4\pi\epsilon_0} \frac{q q_0}{x^2} dx = -\frac{q q_0}{4\pi\epsilon_0} \left[ -\frac{1}{x} \right]_{\infty}^{r} = \frac{1}{4\pi\epsilon_0} \frac{q q_0}{r}$.
5.  Potential $V = \frac{W}{q_0} =$ **$\frac{1}{4\pi\epsilon_0} \frac{q}{r}$**.

### B. Capacitance of a Parallel Plate Capacitor with Dielectric Slab
1.  Plates have area $A$, separation $d$, and charges $+Q, -Q$.
2.  A dielectric slab of thickness $t < d$ and constant $K$ is introduced.
3.  Electric field in air gap: $E_0 = \frac{\sigma}{\epsilon_0}$.
4.  Electric field in dielectric: $E = \frac{E_0}{K}$.
5.  Potential difference $V = E_0(d-t) + E(t) = E_0(d-t) + \frac{E_0}{K}t = \frac{Q}{A\epsilon_0} \left( d - t + \frac{t}{K} \right)$.
6.  Capacitance $C = \frac{Q}{V} = \frac{\epsilon_0 A}{d - t + \frac{t}{K}}$.

## 3. Diagram Blueprints & Labeling Checklists

*   **Equipotential Surfaces**:
    *   **Checklist**:
        *   [ ] Point charge: Concentric circles (2D) / spheres (3D) getting farther apart as $r$ increases.
        *   [ ] Uniform field: Parallel, equally spaced planes.
        *   [ ] Dipole: Peanut shapes, compressed between charges, expanded outside.
        *   [ ] MUST show electric field lines intersecting surfaces at exactly $90^\circ$.
*   **Capacitors in Series and Parallel**:
    *   **Checklist**:
        *   [ ] Series: End-to-end connection, label same $Q$ on each, separate $V_1, V_2, V_3$.
        *   [ ] Parallel: Common junction points, label same $V$ across each, separate $Q_1, Q_2, Q_3$.

## 4. "Avoid the Trap" & Distinction Tables

*   **TRAP ALERT (Subjective)**: Don't confuse Electric Potential ($V$) with Potential Energy ($U$). Potential is per unit charge ($J/C$), while energy is just in Joules ($J$).
*   **TRAP ALERT (Objective)**: When a battery is disconnected, $Q$ remains constant when inserting a dielectric. When a battery remains connected, $V$ remains constant.

| Parameter | Battery Disconnected (Dielectric inserted) | Battery Connected (Dielectric inserted) |
| :--- | :--- | :--- |
| **Charge ($Q$)** | Constant | Increases to $KQ_0$ |
| **Potential ($V$)**| Decreases to $V_0/K$ | Constant |
| **Field ($E$)** | Decreases to $E_0/K$ | Constant |
| **Energy ($U$)** | Decreases to $U_0/K$ | Increases to $KU_0$ |

## 5. High-Yield Worked Model Problems

### Problem 1 (ISC Focus - Step-by-Step)
**Q: Derive an expression for the equivalent capacitance when three capacitors $C_1, C_2, C_3$ are connected in series.**
*   **Step 1**: Draw circuit diagram with $C_1, C_2, C_3$ in series across a voltage source $V$.
*   **Step 2**: State the principle: In series, charge $Q$ on each capacitor is the same. The total potential difference is the sum of individual potential differences.
*   **Step 3**: Equation: $V = V_1 + V_2 + V_3$.
*   **Step 4**: Substitute $V_i = Q/C_i$: $V = \frac{Q}{C_1} + \frac{Q}{C_2} + \frac{Q}{C_3} = Q \left( \frac{1}{C_1} + \frac{1}{C_2} + \frac{1}{C_3} \right)$.
*   **Step 5**: For equivalent capacitor $C_{eq}$, $V = \frac{Q}{C_{eq}}$.
*   **Conclusion**: Equating both, **$\frac{1}{C_{eq}} = \frac{1}{C_1} + \frac{1}{C_2} + \frac{1}{C_3}$**.

### Problem 2 (NEET/JEE Focus - Speed Method)
**Q: 27 identical liquid drops, each charged to 10V, combine to form a single large drop. What is the potential of the large drop?**
*   **Standard Method**: Find new radius $R = (27)^{1/3}r = 3r$. Total charge $Q_{tot} = 27q$. $V_{new} = k(27q)/(3r) = 9 (kq/r) = 9 \times 10 = 90V$.
*   **Speed Trick**: $V_{big} = n^{2/3} V_{small}$.
*   **Execution**: $V_{big} = (27)^{2/3} \times 10 = (3)^{2} \times 10 = 9 \times 10 = 90V$.
