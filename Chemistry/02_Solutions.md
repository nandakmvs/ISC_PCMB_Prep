# Chapter 2: Solutions

## 2.1 Introduction & Types of Solutions
A solution is a homogeneous mixture of two or more chemically non-reacting substances. The component present in a larger amount is the solvent, and the one in a smaller amount is the solute. In ISC Class 12, the focus is on binary solutions (one solvent, one solute).

## 2.2 Expressing Concentration
Understanding concentration terms is crucial for Colligative Properties numericals.
*   **Molarity ($M$)**: Moles of solute per litre of solution. (Temperature dependent)
*   **Molality ($m$)**: Moles of solute per kg of solvent. (Temperature independent - preferred for Colligative Properties)
*   **Mole Fraction ($x$)**: Ratio of moles of one component to total moles. $x_A + x_B = 1$.

**SJBHC Pro-Tip (Numericals)**: Be comfortable converting Molarity to Molality using the density of the solution ($d = M(\frac{1}{m} + \frac{M_2}{1000})$).

## 2.3 Solubility & Henry's Law
*Solubility* is the maximum amount of solute that dissolves in a specified amount of solvent at a specific temperature.
**Henry's Law**: The partial pressure of the gas in vapour phase ($p$) is proportional to the mole fraction of the gas ($x$) in the solution.
$$ p = K_H \cdot x $$
Where $K_H$ is Henry's law constant. Higher $K_H$ means lower solubility.

**Assertion-Reason (SJBHC Style)**:
*Assertion (A)*: Aquatic species are more comfortable in cold water rather than in warm water.
*Reason (R)*: $K_H$ values for both $N_2$ and $O_2$ increase with an increase in temperature, implying solubility decreases with rising temperature.
*Conclusion*: Both A and R are true, and R is the correct explanation of A.

## 2.4 Raoult's Law & Liquid-Liquid Solutions
For a solution of volatile liquids, the partial vapour pressure of each component is directly proportional to its mole fraction in the solution.
$$ p_1 = p_1^0 \cdot x_1 $$
$$ p_2 = p_2^0 \cdot x_2 $$
$$ P_{total} = p_1 + p_2 = p_1^0 x_1 + p_2^0 x_2 $$

## 2.5 Ideal and Non-Ideal Solutions
**Ideal Solutions**: Obey Raoult's law exactly over the entire range of concentration. $\Delta H_{mix} = 0$, $\Delta V_{mix} = 0$. (e.g., Benzene + Toluene). A-B interactions are similar to A-A and B-B interactions.

**Non-Ideal Solutions**:
1.  **Positive Deviation**: Vapour pressure is higher than expected. A-B interactions are weaker. $\Delta H_{mix} > 0, \Delta V_{mix} > 0$. (e.g., Ethanol + Acetone). Forms **minimum boiling azeotropes**.
2.  **Negative Deviation**: Vapour pressure is lower than expected. A-B interactions are stronger. $\Delta H_{mix} < 0, \Delta V_{mix} < 0$. (e.g., Chloroform + Acetone, due to H-bonding). Forms **maximum boiling azeotropes**.

**Competency Focus**:
Identify the type of deviation based on molecular structure and hydrogen bonding. For instance, mixing phenol and aniline results in a negative deviation due to intermolecular H-bonding.

## 2.6 Colligative Properties (Part 1)
Properties that depend only on the *number* of solute particles and not on their nature.

**1. Relative Lowering of Vapour Pressure (RLVP)**:
$$ \frac{p_1^0 - p_1}{p_1^0} = x_2 = \frac{n_2}{n_1 + n_2} $$
For dilute solutions, $n_2 << n_1$, so $x_2 \approx \frac{n_2}{n_1}$. Use this approximation carefully; if the difference is small, use exact calculation.

**2. Elevation of Boiling Point ($\Delta T_b$)**:
Boiling point is reached when vapour pressure equals atmospheric pressure. Addition of non-volatile solute lowers vapour pressure, thus increasing boiling point.
$$ \Delta T_b = K_b \cdot m $$
Where $K_b$ is the ebullioscopic constant or molal elevation constant.
$M_2 = \frac{K_b \cdot W_2 \cdot 1000}{\Delta T_b \cdot W_1}$

**3. Depression of Freezing Point ($\Delta T_f$)**:
Addition of non-volatile solute lowers the freezing point.
$$ \Delta T_f = K_f \cdot m $$
Where $K_f$ is the cryoscopic constant.
$M_2 = \frac{K_f \cdot W_2 \cdot 1000}{\Delta T_f \cdot W_1}$

*Numerical Alert*: Always check if the solute undergoes association or dissociation. If it's a strong electrolyte like $NaCl$, you must incorporate the van't Hoff factor (covered in section 2.8).

## 2.7 Osmosis and Osmotic Pressure
**Osmosis**: The net spontaneous flow of solvent molecules from a solvent (or less concentrated solution) to a more concentrated solution through a semi-permeable membrane.
**Osmotic Pressure ($\pi$)**: The excess pressure that must be applied to a solution to prevent osmosis.
$$ \pi = C R T $$
Where $C$ is molarity, $R$ is gas constant ($0.0821 \text{ L atm K}^{-1} \text{mol}^{-1}$ or $0.083 \text{ L bar K}^{-1} \text{mol}^{-1}$).

*Reverse Osmosis*: If a pressure larger than the osmotic pressure is applied to the solution side, the pure solvent flows out of the solution through the SPM. Used in desalination.

## 2.8 Abnormal Molar Mass and van't Hoff Factor ($i$)
When solutes undergo association (e.g., acetic acid in benzene) or dissociation (e.g., $KCl$ in water), the number of particles changes, causing abnormal colligative properties.
$$ i = \frac{\text{Normal molar mass}}{\text{Abnormal molar mass}} = \frac{\text{Observed colligative property}}{\text{Calculated colligative property}} $$
*   For dissociation: $i > 1$. Degree of dissociation $\alpha = \frac{i - 1}{n - 1}$
*   For association: $i < 1$. Degree of association $\alpha = \frac{1 - i}{1 - 1/n}$
*   For non-electrolytes: $i = 1$.

**Modified Colligative Equations**:
1.  $\frac{p_1^0 - p_1}{p_1^0} = i \cdot x_2$
2.  $\Delta T_b = i \cdot K_b \cdot m$
3.  $\Delta T_f = i \cdot K_f \cdot m$
4.  $\pi = i \cdot C \cdot R \cdot T$

## 2.9 Competency-Based & Assertion-Reason Drill

**Assertion-Reason Pattern**:
**Question 1:**
*Assertion (A)*: The boiling point of $0.1 \text{ M}$ urea solution is less than that of $0.1 \text{ M}$ $KCl$ solution.
*Reason (R)*: Elevation of boiling point is directly proportional to the number of species present in the solution.
*Answer*: Both A and R are true, and R is the correct explanation of A. (Urea is a non-electrolyte, $i=1$; $KCl$ dissociates into 2 ions, $i=2$).

**Question 2:**
*Assertion (A)*: $0.1 \text{ M}$ solution of $NaCl$ has a higher osmotic pressure than $0.1 \text{ M}$ solution of Glucose.
*Reason (R)*: $NaCl$ undergoes dissociation yielding more particles, while glucose does not.
*Answer*: Both A and R are true, and R is the correct explanation of A.

**Case-Based Example**:
Consider two solutions separated by a semi-permeable membrane. Solution A is $0.5 \text{ M} \text{ BaCl}_2$ and Solution B is $0.5 \text{ M} \text{ NaCl}$.
1.  *Which solution will show higher osmotic pressure?* Solution A, because $BaCl_2$ yields 3 ions ($i=3$) compared to $NaCl$ yielding 2 ions ($i=2$).
2.  *What will be the direction of solvent flow?* From Solution B (lower effective concentration/osmotic pressure) to Solution A (higher effective concentration).

**SJBHC Final Check**:
- Are you calculating $i$ properly for weak electrolytes given $\alpha$?
- Did you use $K_b$ and $K_f$ with the correct molality? Remember, Molarity $\neq$ Molality unless explicitly approximated in very dilute aqueous solutions!
