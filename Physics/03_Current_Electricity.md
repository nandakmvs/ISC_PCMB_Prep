# Chapter 3: Current Electricity

## 1. Syllabus & Exhaustive Sub-topic List
- Electric current, flow of electric charges in a metallic conductor, drift velocity, mobility and their relation with electric current
- Ohm's law, electrical resistance, V-I characteristics (linear and non-linear), electrical energy and power
- Electrical resistivity and conductivity, Carbon resistors, colour code for carbon resistors
- Temperature dependence of resistance
- Internal resistance of a cell, potential difference and emf of a cell, combination of cells in series and in parallel
- Kirchhoff's laws and simple applications
- Wheatstone bridge, metre bridge
- Potentiometer - principle and its applications to measure potential difference and for comparing emf of two cells; measurement of internal resistance of a cell

## 2. Theory & Key Derivations (SJBHC Focus)
- **Derivation 1:** Relation between current and drift velocity ($I = n e A v_d$).
- **Derivation 2:** Deduction of Ohm's Law from drift velocity.
- **Derivation 3:** Equivalent EMF and internal resistance for cells in parallel.
- **Derivation 4:** Wheatstone Bridge balance condition using Kirchhoff's rules.
- **Key Concept:** Potentiometer principle and balancing length relations - *crucial for SJBHC 5-mark numericals*.

## 3. Important Formulas & Conceptual Points
- Drift Velocity: $v_d = \frac{eE}{m} \tau$
- Current and Drift Velocity: $I = n e A v_d$
- Mobility: $\mu = \frac{v_d}{E} = \frac{e \tau}{m}$
- Ohm's Law (Microscopic): $\mathbf{J} = \sigma \mathbf{E}$
- Resistivity: $\rho = \frac{m}{n e^2 \tau}$
- Temperature dependence: $R_t = R_0 [1 + \alpha(t - t_0)]$
- EMF and Internal Resistance: $V = E - Ir$ (discharging), $V = E + Ir$ (charging)
- Cells in series: $E_{eq} = E_1 + E_2$, $r_{eq} = r_1 + r_2$
- Cells in parallel: $E_{eq} = \frac{E_1 r_2 + E_2 r_1}{r_1 + r_2}$, $r_{eq} = \frac{r_1 r_2}{r_1 + r_2}$
- Wheatstone Bridge: $\frac{P}{Q} = \frac{R}{S}$
- Potentiometer: $E \propto l \Rightarrow \frac{E_1}{E_2} = \frac{l_1}{l_2}$, $r = R \left( \frac{l_1}{l_2} - 1 \right)$

## 4. SJBHC Specific Numerical Problems
**Type 1: Kirchhoff's Laws**
**Q1.** Two batteries of EMF $4\text{V}$ and $8\text{V}$ with internal resistances $1\Omega$ and $2\Omega$ respectively are connected in a circuit with an external resistance of $9\Omega$. Find the current through the $9\Omega$ resistor using Kirchhoff's rules if the batteries are in opposing parallel configuration.
*Step-by-step Solution:*
1. Draw diagram and assign currents $I_1$ (from 4V) and $I_2$ (from 8V). Current through $9\Omega$ is $I_1 + I_2$.
2. Apply KVL to loop 1: $4 - 1 \cdot I_1 - 9(I_1 + I_2) = 0 \Rightarrow 10I_1 + 9I_2 = 4$.
3. Apply KVL to loop 2: $8 - 2 \cdot I_2 - 9(I_1 + I_2) = 0 \Rightarrow 9I_1 + 11I_2 = 8$.
4. Solve simultaneously: $I_1 = -0.96 \text{ A}$, $I_2 = 1.51 \text{ A}$.
5. Current through $9\Omega$: $I_1 + I_2 = 0.55 \text{ A}$.

**Type 2: Metre Bridge**
**Q2.** In a metre bridge, the null point is found at a distance of $33.7 \text{ cm}$ from $A$. If a resistance of $12\Omega$ is connected in parallel with $S$, the null point occurs at $51.9 \text{ cm}$. Determine the values of $R$ and $S$.
*Solution:*
1. Initially: $\frac{R}{S} = \frac{33.7}{66.3}$.
2. Later, $S'$ is $S$ and 12 in parallel: $S' = \frac{12S}{12+S}$.
3. $\frac{R}{S'} = \frac{51.9}{48.1}$.
4. Divide equations and solve for $S$, then substitute back to get $R$. $S = 13.5\Omega$, $R = 6.86\Omega$.

## 5. Competency Based Education (CBE) - Assertion-Reason & Case-Based
**Directions:** For Assertion (A) and Reason (R), choose the correct option:
a) Both A and R are true and R is the correct explanation of A.
b) Both A and R are true but R is not the correct explanation of A.
c) A is true but R is false.
d) A is false but R is true.

**Q1.**
**Assertion (A):** The drift velocity of electrons in a metallic wire decreases when temperature of the wire increases.
**Reason (R):** On increasing temperature, conductivity of metallic wire decreases due to increased collision frequency (decreased relaxation time).
*Answer:* (a) Both A and R are true and R is the correct explanation.

**Q2.**
**Assertion (A):** Kirchhoff's junction rule is based on the conservation of charge.
**Reason (R):** The algebraic sum of currents meeting at a junction is zero.
*Answer:* (a)

**Case-Based Question:**
*Read the passage and answer:*
A potentiometer is a device used to measure the EMF of a cell precisely. It works on the principle that potential drop across any portion of a uniform wire is directly proportional to its length.
*Q.* Why is a potentiometer preferred over a voltmeter for measuring the EMF of a cell?
*Ans.* Because a potentiometer draws no current from the cell at the null point, measuring the true EMF, whereas a voltmeter draws some current, measuring terminal voltage.

## 6. Past Year Questions & Practice Assignment
**Short Answer (2 Marks):**
1. Define mobility of electron. Write its SI unit.
2. Two wires A and B of the same material have lengths in the ratio 1:2 and radii in the ratio 2:1. What is the ratio of their resistances?
3. State Kirchhoff's loop rule.

**Long Answer (5 Marks):**
1. (a) State the principle of a potentiometer. (b) Draw a circuit diagram to compare the EMFs of two primary cells. (c) Write the formula used.
2. Obtain an expression for the equivalent internal resistance and equivalent EMF of two cells connected in parallel.
3. Using Kirchhoff's rules, find the current flowing through each branch of a given Wheatstone bridge when it is unbalanced.

**SJBHC Practice Assignment:**
- Always state the sign convention clearly when applying Kirchhoff's rules. This is checked meticulously in SJBHC corrections.
- Potentiometer numericals involving internal resistance measurement $r = R(l_1/l_2 - 1)$ are extremely common. Ensure you show the substitution step clearly.
