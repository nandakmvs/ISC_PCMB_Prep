# Chapter 09: Ray Optics and Optical Instruments

## 1. Exhaustive Theory & Precise ISC Terminology

*   **Laws of Reflection**: (i) Incident ray, reflected ray, and normal lie in the same plane. (ii) Angle of incidence = Angle of reflection ($\angle i = \angle r$).
*   **Spherical Mirrors**: Paraxial rays (close to axis) and Marginal rays.
*   **Mirror Formula**: $\frac{1}{v} + \frac{1}{u} = \frac{1}{f}$.
*   **Refraction**: Bending of light when passing from one medium to another.
*   **Snell's Law**: The ratio of the sine of the angle of incidence to the sine of the angle of refraction is a constant for a given pair of media. $\frac{\sin i}{\sin r} = _{1}\mu_{2} = \frac{\mu_2}{\mu_1}$.
*   **Total Internal Reflection (TIR)**: The phenomenon where light traveling from a denser to a rarer medium is completely reflected back into the denser medium if the angle of incidence exceeds the critical angle.
*   **Critical Angle ($i_c$)**: The angle of incidence in the denser medium for which the angle of refraction is $90^\circ$. $\sin i_c = \frac{1}{\mu}$.
*   **Lens Maker's Formula**: Relates focal length to radii of curvature and refractive index.
*   **Thin Lens Formula**: $\frac{1}{v} - \frac{1}{u} = \frac{1}{f}$.
*   **Power of a Lens ($P$)**: The measure of convergence or divergence. $P = \frac{1}{f \text{ (in meters)}}$. Unit: Diopter (D).
*   **Dispersion**: Splitting of white light into constituent colors through a prism.
*   **Magnifying Power**: The ratio of the angle subtended at the eye by the image to the angle subtended by the object (when placed at least distance of distinct vision).

## 2. Step-by-Step Derivations & Mechanisms

### A. Lens Maker's Formula
1.  Consider a convex lens of refractive index $\mu_2$ in a medium of $\mu_1$. Let surfaces have radii $R_1, R_2$.
2.  Refraction at surface 1: Forms image $I_1$ at distance $v_1$.
    $\frac{\mu_2}{v_1} - \frac{\mu_1}{u} = \frac{\mu_2 - \mu_1}{R_1}$ (Eq. 1)
3.  Refraction at surface 2: $I_1$ acts as a virtual object for surface 2, forming final image at $v$.
    $\frac{\mu_1}{v} - \frac{\mu_2}{v_1} = \frac{\mu_1 - \mu_2}{R_2} = - \frac{\mu_2 - \mu_1}{R_2}$ (Eq. 2)
4.  Add Eq 1 and Eq 2:
    $\frac{\mu_1}{v} - \frac{\mu_1}{u} = (\mu_2 - \mu_1) \left( \frac{1}{R_1} - \frac{1}{R_2} \right)$
5.  Divide by $\mu_1$: $\frac{1}{v} - \frac{1}{u} = \left( \frac{\mu_2}{\mu_1} - 1 \right) \left( \frac{1}{R_1} - \frac{1}{R_2} \right)$
6.  If object is at infinity ($u = -\infty$), image is at focus ($v = f$).
7.  **$\frac{1}{f} = (\mu_{rel} - 1) \left( \frac{1}{R_1} - \frac{1}{R_2} \right)$**.

### B. Prism Formula
1.  At minimum deviation ($D_m$), the ray passes symmetrically.
2.  $i = e$ and $r_1 = r_2 = r$.
3.  Prism angle $A = r_1 + r_2 \implies A = 2r \implies r = A/2$.
4.  Deviation $\delta = i + e - A \implies D_m = 2i - A \implies i = \frac{A + D_m}{2}$.
5.  By Snell's law: **$\mu = \frac{\sin i}{\sin r} = \frac{\sin(\frac{A + D_m}{2})}{\sin(\frac{A}{2})}$**.

## 3. Diagram Blueprints & Labeling Checklists

*   **Compound Microscope Ray Diagram**:
    *   **Checklist**:
        *   [ ] Objective lens (small), Eyepiece lens (large).
        *   [ ] Object $AB$ placed just outside $f_o$.
        *   [ ] Real, inverted, magnified intermediate image $A'B'$ formed between $f_e$ and optical center of eyepiece.
        *   [ ] Final virtual, highly magnified image $A''B''$ formed at $D$ or infinity.
        *   [ ] Arrows on all rays. Include eye on the right.
        *   [ ] Label focal points, $u_o, v_o, u_e, v_e$.

## 4. "Avoid the Trap" & Distinction Tables

*   **TRAP ALERT (Subjective)**: 90% of numerical errors in Optics occur due to violating the **Cartesian Sign Convention**.
    *   Direction of incident light is POSITIVE.
    *   Distances measured opposite to incident light are NEGATIVE.
    *   Convex Focus = Positive, Concave Focus = Negative.
*   **Distinction**:
  | Reflecting Telescope | Refracting Telescope |
  | :--- | :--- |
  | Uses parabolic mirror as objective | Uses convex lens as objective |
  | No chromatic aberration | Suffers from chromatic aberration |
  | Lighter and easier to support | Heavy, difficult to support large lenses |

## 5. High-Yield Worked Model Problems

### Problem 1 (ISC Focus - Step-by-Step)
**Q: An equiconvex lens of focal length 20 cm ($\mu = 1.5$) is sliced completely into two halves along its principal axis. What is the focal length of each half? What if it's sliced perpendicular to the principal axis?**
*   **Step 1**: Use Lens Maker's: $\frac{1}{f} = (\mu - 1) (\frac{1}{R} - (-\frac{1}{R})) = \frac{2(\mu - 1)}{R}$.
*   **Step 2**: Sliced along principal axis: Radii $R$ and $-R$ remain unchanged. Therefore, focal length remains **20 cm**. Intensity of image decreases (aperture halved).
*   **Step 3**: Sliced perpendicular: One surface becomes plane ($R_2 = \infty$).
*   **Step 4**: New focal length: $\frac{1}{f'} = (\mu - 1)(\frac{1}{R} - 0) = \frac{\mu - 1}{R}$.
*   **Conclusion**: $f' = 2f$. The new focal length is **40 cm**.

### Problem 2 (NEET/JEE Focus - Speed Method)
**Q: A combination of two thin lenses in contact produces a real image magnified 2 times of an object placed 15 cm from it. If the power of one lens is +5 D, find the focal length of the other.**
*   **Speed Trick / Direct Formula**:
    *   $m = -2$ (real). $v = -mu = -(-2)(-15) = +30$ cm.
    *   $1/F_{eq} = 1/v - 1/u = 1/30 - 1/(-15) = 1/30 + 2/30 = 3/30 = 1/10$ cm$^{-1}$. So $F_{eq} = +10$ cm.
    *   $P_{eq} = 100/F_{eq} = +10$ D.
    *   $P_{eq} = P_1 + P_2 \implies 10 = 5 + P_2 \implies P_2 = +5$ D.
    *   $F_2 = 100/P_2 =$ **+20 cm**.
