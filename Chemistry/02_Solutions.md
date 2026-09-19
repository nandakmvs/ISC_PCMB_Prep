# Chapter 2: Solutions

## 1. Exhaustive Theory & Precise ISC Terminology

A **solution** is a **homogeneous mixture** of two or more substances whose composition can be varied within certain limits.
- **Solvent**: The component present in the largest quantity, which determines the physical state of the solution.
- **Solute**: The component present in a lesser quantity.

### Concentration Terms
- **Molarity (M)**: Moles of solute per **liter of solution**. (Temperature dependent).
- **Molality (m)**: Moles of solute per **kilogram of solvent**. (Temperature independent - **highly preferred for ISC explanations**).
- **Mole Fraction (x)**: Ratio of moles of one component to total moles in solution.

### Solubility and Henry's Law
- **Solubility**: Maximum amount of solute that can be dissolved in a specified amount of solvent at a constant temperature.
- **Henry's Law**: The **partial pressure** of a gas in vapor phase ($p$) is proportional to the **mole fraction** of the gas ($x$) in the solution.
  $$ p = K_H \cdot x $$
  *ISC Keyword Emphasis*: $K_H$ is the **Henry's Law constant**. Higher $K_H$ means lower solubility at a given pressure.

### Raoult's Law
For a solution of volatile liquids, the partial vapor pressure of each component is directly proportional to its mole fraction in the solution.
$$ p_1 = p_1^0 x_1 $$
- **Ideal Solutions**: Obey Raoult's law exactly across all concentrations. (e.g., n-hexane and n-heptane). Have $\Delta H_{mix} = 0$ and $\Delta V_{mix} = 0$.
- **Non-Ideal Solutions**: Do not obey Raoult's law.
  - *Positive Deviation*: A-B interactions are **weaker** than A-A or B-B interactions. (e.g., Ethanol + Acetone). Forms **Minimum boiling azeotrope**.
  - *Negative Deviation*: A-B interactions are **stronger** than A-A or B-B. (e.g., Chloroform + Acetone due to H-bonding). Forms **Maximum boiling azeotrope**.

### Colligative Properties
Properties that depend **only on the number of solute particles** and not on their nature.
1. **Relative Lowering of Vapor Pressure**: $\frac{p_1^0 - p_1}{p_1^0} = x_2$
2. **Elevation of Boiling Point (Ebullioscopy)**: $\Delta T_b = K_b \cdot m$
3. **Depression of Freezing Point (Cryoscopy)**: $\Delta T_f = K_f \cdot m$
4. **Osmotic Pressure**: $\pi = C R T$

### van't Hoff Factor ($i$)
Accounts for **association** or **dissociation** of solute particles.
$$ i = \frac{\text{Normal molar mass}}{\text{Abnormal molar mass}} = \frac{\text{Observed colligative property}}{\text{Calculated colligative property}} $$
- For dissociation (e.g., NaCl): $i > 1$. Degree of dissociation $\alpha = \frac{i-1}{n-1}$.
- For association (e.g., Acetic acid in benzene): $i < 1$. Degree of association $\alpha = \frac{1-i}{1-1/n}$.

---

## 2. Step-by-Step Derivations & Mechanisms

### Derivation of Relative Lowering of Vapor Pressure
1. From Raoult's Law: $p_1 = p_1^0 x_1$
2. For a binary solution: $x_1 + x_2 = 1 \implies x_1 = 1 - x_2$
3. Substitute: $p_1 = p_1^0(1 - x_2) = p_1^0 - p_1^0 x_2$
4. Rearrange: $p_1^0 x_2 = p_1^0 - p_1$
5. Final Equation: $\frac{p_1^0 - p_1}{p_1^0} = x_2 = \frac{n_2}{n_1 + n_2}$
*ISC Note*: For dilute solutions, $n_2 \ll n_1$, so $x_2 \approx \frac{n_2}{n_1} = \frac{W_2 / M_2}{W_1 / M_1}$.

---

## 3. Diagram Blueprints & Labeling Checklists

### 1. Vapor Pressure vs Mole Fraction Graph (Ideal Solution)
- **Axes**: Y-axis: Vapor Pressure, X-axis: Mole fraction ($x_1 = 1 \to 0$, $x_2 = 0 \to 1$).
- **Lines**: Straight lines for $p_1$ and $p_2$.
- **Total Pressure**: Straight line connecting $p_1^0$ and $p_2^0$, $P_{total} = p_1 + p_2$.
- **Checklist**: Label $p_1^0$, $p_2^0$, solid line for $P_{total}$, dashed lines for partial pressures.

### 2. Elevation of Boiling Point Graph
- **Axes**: Y-axis: Vapor Pressure, X-axis: Temperature (K).
- **Curves**: Solvent curve (higher VP), Solution curve (lower VP).
- **Intersection**: Draw a horizontal line at 1 atm (atmospheric pressure).
- **Checklist**: Mark $T_b^0$ (Solvent boiling point), $T_b$ (Solution boiling point), $\Delta T_b$ gap.

---

## 4. "Avoid the Trap" & Distinction Tables

| Ideal Solution | Non-Ideal (Positive Deviation) | Non-Ideal (Negative Deviation) |
| :--- | :--- | :--- |
| $\Delta H_{mix} = 0$ | $\Delta H_{mix} > 0$ (Endothermic) | $\Delta H_{mix} < 0$ (Exothermic) |
| $\Delta V_{mix} = 0$ | $\Delta V_{mix} > 0$ (Expansion) | $\Delta V_{mix} < 0$ (Contraction) |
| Raoult's Law obeyed | $p_1 > p_1^0 x_1$ | $p_1 < p_1^0 x_1$ |
| Eg: Benzene+Toluene | Eg: Ethanol+Water | Eg: Phenol+Aniline |

### ⚠️ ISC Traps & Subjective Pitfalls
- **Trap**: Using Molarity instead of Molality for colligative properties.
  - *Correction*: $\Delta T_b$ uses **molality ($m$)** because mass does not change with temperature, whereas volume (in molarity) does.
- **Trap**: Forgetting the van't Hoff factor for electrolytes.
  - *Correction*: Always write $\Delta T_f = i \cdot K_f \cdot m$. If it's glucose/urea, $i=1$. If it's $K_2SO_4$, $i=3$ (assuming 100% dissociation).
- **Trap**: Defining Osmosis poorly.
  - *Correction*: ISC requires the phrase: "**Flow of solvent molecules** from a region of **lower concentration (of solute)** to **higher concentration** across a **semi-permeable membrane**."

---

## 5. High-Yield Worked Model Problems

### Q1. ISC Step-by-Step Problem: Osmotic Pressure
**Calculate the osmotic pressure of a $0.05 \text{ M}$ solution of $NaCl$ at $300 \text{ K}$, assuming complete dissociation. ($R = 0.0821 \text{ L atm K}^{-1} \text{mol}^{-1}$)**

**ISC Method (For Board Exams - Show all steps):**
1. **Identify Given Data**: $C = 0.05 \text{ M}$, $T = 300 \text{ K}$, $R = 0.0821 \text{ L atm K}^{-1} \text{mol}^{-1}$.
2. **Identify Solute Type**: NaCl is a strong electrolyte. It dissociates into $Na^+$ and $Cl^-$.
   Number of ions ($n$) = 2. Since dissociation is complete ($\alpha = 1$), van't Hoff factor $i = 2$.
3. **Write Formula**: $\pi = i C R T$
4. **Substitute & Calculate**:
   $\pi = 2 \times 0.05 \times 0.0821 \times 300$
   $\pi = 0.1 \times 24.63 = 2.463 \text{ atm}$
5. **Final Answer Statement**: The osmotic pressure of the NaCl solution is **2.463 atm**.

**NEET/JEE Speed Method:**
Recognize $NaCl \implies i=2$. $RT$ at 300K is $\approx 24.6$. $\pi = 2 \times 0.05 \times 24.6 = 0.1 \times 24.6 = 2.46 \text{ atm}$.

### Q2. ISC Step-by-Step Problem: Degree of Association
**2g of benzoic acid ($C_6H_5COOH$) dissolved in 25g of benzene shows a depression in freezing point equal to 1.62 K. Molal depression constant for benzene is 4.9 K kg mol$^{-1}$. What is the percentage association of acid if it forms a dimer in solution?**

**ISC Method:**
1. **Given**: $W_2 = 2 \text{ g}$, $W_1 = 25 \text{ g}$, $\Delta T_f = 1.62 \text{ K}$, $K_f = 4.9 \text{ K kg mol}^{-1}$.
2. **Find Observed Molar Mass ($M_{obs}$)**:
   $\Delta T_f = \frac{K_f \times W_2 \times 1000}{M_{obs} \times W_1}$
   $1.62 = \frac{4.9 \times 2 \times 1000}{M_{obs} \times 25}$
   $M_{obs} = \frac{4.9 \times 2 \times 40}{1.62} = 241.98 \text{ g/mol}$
3. **Normal Molar Mass ($M_{calc}$)** for Benzoic acid = $122 \text{ g/mol}$.
4. **van't Hoff Factor ($i$)**: $i = \frac{M_{calc}}{M_{obs}} = \frac{122}{241.98} \approx 0.504$.
5. **Degree of Association ($\alpha$)**:
   Formula for dimerization ($n=2$): $\alpha = \frac{1-i}{1-1/n}$
   $\alpha = \frac{1 - 0.504}{1 - 1/2} = \frac{0.496}{0.5} = 0.992$
6. **Percentage Association**: $0.992 \times 100 = \mathbf{99.2\%}$.
