# Chapter 10: Wave Optics

## 1. Exhaustive Theory & Precise ISC Terminology

*   **Wavefront**: The continuous locus of all particles of a medium which are vibrating in the same phase. (Spherical, Cylindrical, Plane).
*   **Huygens' Principle**: Every point on a given wavefront acts as a fresh source of new disturbance, called secondary wavelets, which travel in all directions with the velocity of light in the medium. The forward envelope of these wavelets gives the new wavefront.
*   **Interference of Light**: The phenomenon of redistribution of light energy due to the superposition of light waves from two coherent sources.
*   **Coherent Sources**: Sources that emit continuous light waves of the same frequency and a zero or constant phase difference.
*   **Constructive Interference**: Points where crest meets crest; maximum intensity. Path difference $\Delta x = n\lambda$.
*   **Destructive Interference**: Points where crest meets trough; minimum intensity. Path difference $\Delta x = (n + \frac{1}{2})\lambda$.
*   **Fringe Width ($\beta$)**: The distance between two consecutive bright or dark fringes. $\beta = \frac{\lambda D}{d}$.
*   **Diffraction**: The phenomenon of bending of light around the corners of an obstacle or aperture and its encroachment into the region of geometrical shadow.
*   **Polarisation**: The restriction of the vibrations of light waves to a single plane perpendicular to the direction of propagation. (Transverse nature of light).
*   **Brewster's Law**: $\mu = \tan i_p$.
*   **Malus's Law**: $I = I_0 \cos^2 \theta$.

## 2. Step-by-Step Derivations & Mechanisms

### A. Laws of Refraction on the basis of Huygens' Principle
1.  Consider a plane wavefront $AB$ incident on a surface $XY$ separating media of velocities $v_1$ and $v_2$. Let angle of incidence be $i$.
2.  By the time wavelet from $B$ reaches $C$ in time $\tau$ ($BC = v_1 \tau$), wavelet from $A$ travels a distance $AD = v_2 \tau$ in the second medium.
3.  Draw a tangent $CD$ to the wavelet from $A$. $CD$ is the refracted wavefront. Angle of refraction is $r$.
4.  In $\triangle ABC$: $\sin i = \frac{BC}{AC} = \frac{v_1 \tau}{AC}$.
5.  In $\triangle ADC$: $\sin r = \frac{AD}{AC} = \frac{v_2 \tau}{AC}$.
6.  Ratio: $\frac{\sin i}{\sin r} = \frac{v_1 \tau / AC}{v_2 \tau / AC} = \frac{v_1}{v_2} = _{1}\mu_{2}$. (Snell's Law Proved).

### B. Fringe Width in YDSE
1.  Path difference between waves from $S_1$ and $S_2$ to point $P$ is $\Delta x = S_2P - S_1P$.
2.  From geometry (assuming $D \gg d$), $\Delta x \approx d \sin \theta \approx d \tan \theta = d (\frac{y}{D})$.
3.  For $n$-th bright fringe: $\Delta x = n\lambda \implies \frac{yd}{D} = n\lambda \implies y_n = \frac{n\lambda D}{d}$.
4.  Fringe width $\beta = y_{n+1} - y_n = \frac{(n+1)\lambda D}{d} - \frac{n\lambda D}{d} =$ **$\frac{\lambda D}{d}$**.

## 3. Diagram Blueprints & Labeling Checklists

*   **Young's Double Slit Experiment (YDSE)**:
    *   **Checklist**:
        *   [ ] Primary source $S$, secondary coherent slits $S_1, S_2$.
        *   [ ] Screen at distance $D$.
        *   [ ] Slit separation $d$.
        *   [ ] Point $P$ on screen at distance $y$ from central maximum $O$.
        *   [ ] Show rays $S_1P$ and $S_2P$. Draw perpendicular $S_1N$ onto $S_2P$ to show path difference $\Delta x = S_2N$.

*   **Single Slit Diffraction**:
    *   **Checklist**:
        *   [ ] Single slit of width $a$.
        *   [ ] Incident plane wavefront.
        *   [ ] Lens to focus rays on screen.
        *   [ ] Intensity graph: High wide central peak, rapidly diminishing secondary peaks.

## 4. "Avoid the Trap" & Distinction Tables

*   **TRAP ALERT (Subjective)**: Don't confuse the formulas for the width of the central maximum in diffraction. The angular width is $\frac{2\lambda}{a}$, and the linear width is $\frac{2\lambda D}{a}$. It is TWICE the width of secondary maxima.
*   **TRAP ALERT (Objective)**: If the whole YDSE apparatus is immersed in a liquid of refractive index $\mu$, the wavelength becomes $\lambda' = \lambda/\mu$. Thus, fringe width $\beta$ decreases by a factor of $\mu$.

| Feature | Interference | Diffraction |
| :--- | :--- | :--- |
| **Origin** | Superposition of waves from two distinct coherent sources | Superposition of secondary wavelets from different parts of the same wavefront |
| **Fringe Width** | Generally uniform | Never uniform (Central max is double width) |
| **Intensity** | All bright fringes have same intensity | Intensity of bright fringes decreases rapidly |
| **Dark Fringes** | Perfectly dark (if amplitudes are equal) | Not perfectly dark |

## 5. High-Yield Worked Model Problems

### Problem 1 (ISC Focus - Step-by-Step)
**Q: Two coherent light waves of intensities $I$ and $4I$ are superposed. Find the maximum and minimum possible intensities in the resulting beam.**
*   **Step 1: Formula Setup**: $I_{max} = (\sqrt{I_1} + \sqrt{I_2})^2$ and $I_{min} = (\sqrt{I_1} - \sqrt{I_2})^2$.
*   **Step 2: Substitution**: $I_1 = I$, $I_2 = 4I$.
*   **Step 3: Max Intensity**: $I_{max} = (\sqrt{I} + \sqrt{4I})^2 = (\sqrt{I} + 2\sqrt{I})^2 = (3\sqrt{I})^2 =$ **$9I$**.
*   **Step 4: Min Intensity**: $I_{min} = (\sqrt{I} - \sqrt{4I})^2 = (\sqrt{I} - 2\sqrt{I})^2 = (-\sqrt{I})^2 =$ **$I$**.
*   **Conclusion**: The ratio $I_{max}:I_{min}$ is 9:1.

### Problem 2 (NEET/JEE Focus - Speed Method)
**Q: Unpolarised light of intensity $I_0$ passes through two polaroids with their transmission axes at an angle of $45^\circ$. What is the intensity of the transmitted light?**
*   **Speed Trick**: First polaroid cuts unpolarised light exactly in half. Second applies Malus's Law.
*   **Execution**:
    *   After 1st Polaroid: $I_1 = I_0 / 2$.
    *   After 2nd Polaroid: $I_2 = I_1 \cos^2(45^\circ) = (I_0/2) \times (1/\sqrt{2})^2 = (I_0/2) \times (1/2) =$ **$I_0/4$**.
