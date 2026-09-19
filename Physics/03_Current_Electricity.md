# Chapter 03: Current Electricity

## 1. Exhaustive Theory & Precise ISC Terminology

*   **Electric Current ($I$)**: The rate of flow of electric charge through any cross-section of a conductor. $I = \frac{dq}{dt}$.
*   **Drift Velocity ($v_d$)**: The average velocity with which free electrons in a conductor get drifted towards the positive end of the conductor under the influence of an applied electric field.
*   **Mobility ($\mu$)**: The magnitude of drift velocity per unit electric field. $\mu = \frac{|v_d|}{E}$.
*   **Ohm's Law**: Physical conditions (like temperature) remaining constant, the current flowing through a conductor is directly proportional to the potential difference across its ends. $V = IR$.
*   **Electromotive Force (EMF, $\mathcal{E}$)**: The maximum potential difference between the two electrodes of a cell when no current is drawn from the cell (open circuit).
*   **Internal Resistance ($r$)**: The resistance offered by the electrolyte and electrodes of a cell to the flow of current.
*   **Terminal Voltage ($V$)**: The potential difference across the terminals of a cell when current is being drawn from it. $V = \mathcal{E} - Ir$.
*   **Kirchhoff's Current Law (KCL - Junction Rule)**: The algebraic sum of currents meeting at a junction in a closed circuit is zero. $\Sigma I = 0$. (Based on Conservation of Charge).
*   **Kirchhoff's Voltage Law (KVL - Loop Rule)**: The algebraic sum of changes in potential around any closed loop involving resistors and cells in the loop is zero. $\Sigma \Delta V = 0$. (Based on Conservation of Energy).
*   **Wheatstone Bridge**: An arrangement of four resistors used to determine an unknown resistance accurately. Null point condition: $P/Q = R/S$.
*   **Potentiometer**: An instrument used to measure an unknown EMF or potential difference accurately without drawing current from the source.

## 2. Step-by-Step Derivations & Mechanisms

### A. Derivation of Ohm's Law and Resistivity
1.  Let length of conductor be $l$, area $A$, electron density $n$.
2.  Drift velocity $v_d = \frac{e E}{m} \tau$ (where $\tau$ is relaxation time).
3.  Current $I = ne A v_d$.
4.  Substitute $v_d$: $I = ne A \left(\frac{e E}{m} \tau\right) = \frac{ne^2 A \tau}{m} \frac{V}{l}$ (since $E = V/l$).
5.  Rearranging: $V = \left( \frac{m}{ne^2 \tau} \frac{l}{A} \right) I$.
6.  Comparing with $V = IR$, $R = \frac{m}{ne^2 \tau} \frac{l}{A}$.
7.  Since $R = \rho \frac{l}{A}$, Resistivity **$\rho = \frac{m}{ne^2 \tau}$**.

### B. Condition for Balanced Wheatstone Bridge
1.  Consider arms AB (P), BC (Q), AD (R), DC (S). Galvanometer between B and D.
2.  Apply KCL at junctions B and D.
3.  Apply KVL to loop ABDA: $I_1 P + I_g G - I_2 R = 0$.
4.  Apply KVL to loop BCDB: $(I_1 - I_g)Q - (I_2 + I_g)S - I_g G = 0$.
5.  For balanced bridge, $I_g = 0$.
6.  Eq 1 becomes $I_1 P = I_2 R \implies \frac{I_1}{I_2} = \frac{R}{P}$.
7.  Eq 2 becomes $I_1 Q = I_2 S \implies \frac{I_1}{I_2} = \frac{S}{Q}$.
8.  Equating both: $\frac{R}{P} = \frac{S}{Q} \implies$ **$\frac{P}{Q} = \frac{R}{S}$**.

## 3. Diagram Blueprints & Labeling Checklists

*   **Potentiometer Circuit for Comparing EMFs**:
    *   **Checklist**:
        *   [ ] Primary circuit: Driver battery ($E_p$), Key ($K_1$), Rheostat ($Rh$) connected across wire AB.
        *   [ ] Secondary circuit: Cells $E_1, E_2$ connected to a two-way key, then to Galvanometer ($G$) and Jockey ($J$).
        *   [ ] Critical: Positive terminals of ALL batteries ($E_p, E_1, E_2$) MUST be connected to the SAME point (A).
        *   [ ] Label balancing lengths $l_1, l_2$.

## 4. "Avoid the Trap" & Distinction Tables

*   **TRAP ALERT (Subjective)**: When applying KVL, explicitly state your loop direction (clockwise or counter-clockwise) and stick strictly to the sign convention. Current flow causes a drop ($-IR$), opposing current causes a gain ($+IR$).
*   **TRAP ALERT (Objective)**: A voltmeter measures terminal voltage, NOT EMF. A potentiometer measures true EMF because it draws zero current ($I=0$).

| Device | Voltmeter | Potentiometer |
| :--- | :--- | :--- |
| **Current drawn** | Draws small current | Draws ZERO current at null point |
| **Accuracy** | Approximate reading | Exact measurement of EMF |
| **Resistance** | High but finite | Infinite (effectively, at null) |

## 5. High-Yield Worked Model Problems

### Problem 1 (ISC Focus - Step-by-Step)
**Q: A cell of EMF $E$ and internal resistance $r$ is connected across a variable resistor $R$. Plot a graph showing variation of terminal voltage $V$ with $R$.**
*   **Step 1: Formula Setup**: Current $I = \frac{E}{R+r}$. Terminal Voltage $V = IR = \frac{E R}{R+r}$.
*   **Step 2: Rearrange for limits**: $V = \frac{E}{1 + r/R}$.
*   **Step 3: Analyze Limits**:
    *   When $R \to 0$ (short circuit), $V = 0$.
    *   When $R = r$, $V = E/2$.
    *   When $R \to \infty$ (open circuit), $V = E$.
*   **Step 4: Draw Graph**: Curve starting from origin (0,0), asymptotically approaching the horizontal line $V = E$.

### Problem 2 (NEET/JEE Focus - Speed Method)
**Q: Find the equivalent resistance of a cube of wires (each of resistance $r$) across its main body diagonal.**
*   **Speed Trick / Memorization**:
    *   Body Diagonal: $\frac{5}{6}r$
    *   Face Diagonal: $\frac{3}{4}r$
    *   Edge: $\frac{7}{12}r$
*   **Execution**: Simply state the standard result $\frac{5}{6}r$ saving 5 minutes of KVL nodal analysis.
