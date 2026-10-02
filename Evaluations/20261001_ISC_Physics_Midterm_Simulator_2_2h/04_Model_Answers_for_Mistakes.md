# Model Answers & Corrections: Physics Midterm Simulator 02

### 1. Stretching a Wire (Resistance)
**Mistake:** Assuming $R \propto l$ without accounting for area change.
**Correction:** 
When a wire is *stretched*, its volume ($V = A \cdot l$) remains constant.
If length becomes $nl$, area MUST become $A/n$.
$R_{new} = \rho \frac{nl}{A/n} = n^2 \left(\rho \frac{l}{A}\right) = n^2 R_{old}$
Since it was stretched to twice its length ($n=2$), $R_{new} = 4R$.

### 2. Capacitor Combinations
**Mistake:** Reversing the parallel/series logic for capacitors.
**Correction:** 
- Capacitors in Series: $\frac{1}{C_{eq}} = \frac{1}{C_1} + \frac{1}{C_2} \implies$ Decreases capacitance.
- Capacitors in Parallel: $C_{eq} = C_1 + C_2 \implies$ Increases capacitance.
To get $2C/3$ (which is less than $C$), we need a series component.
Let's try two in parallel: $C_p = C + C = 2C$.
Now put this $2C$ in series with the remaining $C$:
$C_{eq} = \frac{(2C)(C)}{2C + C} = \frac{2C^2}{3C} = \frac{2C}{3}$.
So the correct arrangement is **Two in parallel, and that combination in series with the third**.

### 3. Telescope Separation Length
**Mistake:** Subtracting focal lengths instead of adding them.
**Correction:**
In an astronomical telescope in normal adjustment (image at infinity), the focal point of the objective lens exactly coincides with the focal point of the eyepiece.
Therefore, the physical distance (separation) between the two lenses is simply the sum of their focal lengths:
$L = f_o + f_e$
$L = 144 + 6 = 150 \text{ cm}$.
