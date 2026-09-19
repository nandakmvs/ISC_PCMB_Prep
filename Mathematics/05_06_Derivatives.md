# Chapter 05 & 06: Derivatives (Continuity, Differentiability, and Differentiation)

## 1. Exhaustive Theory & Precise ISC Terminology

### 1.1 Continuity
*   **Continuity at a point**: A function $f(x)$ is **continuous at $x = c$** if the **Left Hand Limit (LHL)**, **Right Hand Limit (RHL)**, and the **value of the function** at $c$ are all equal and finite.
    *   $\lim_{x \to c^-} f(x) = \lim_{x \to c^+} f(x) = f(c)$
*   **Discontinuity**: If a function is not continuous at $c$, it is discontinuous. Types include:
    *   **Removable Discontinuity**: LHL = RHL $\neq f(c)$ (can be redefined to be continuous).
    *   **Discontinuity of the First Kind (Jump)**: LHL $\neq$ RHL.
    *   **Discontinuity of the Second Kind (Essential)**: LHL or RHL does not exist or tends to infinity.

### 1.2 Differentiability
*   **Differentiability at a point**: A function $f(x)$ is **differentiable** (or derivable) at a point $x = c$ in its domain if its **Left Hand Derivative (LHD)** equals its **Right Hand Derivative (RHD)**, and both are finite.
    *   **LHD** at $x = c$: $\lim_{h \to 0^-} \frac{f(c+h) - f(c)}{h}$
    *   **RHD** at $x = c$: $\lim_{h \to 0^+} \frac{f(c+h) - f(c)}{h}$
*   **Crucial Theorem**: **Every differentiable function is continuous, but the converse is not necessarily true.** (e.g., $f(x) = |x|$ is continuous at $x=0$ but not differentiable).

### 1.3 Differentiation Concepts & Terminology
*   **Derivative**: The **instantaneous rate of change** of a function with respect to its variable. Denoted by $f'(x)$, $\frac{dy}{dx}$, $y_1$, or $y'$.
*   **First Principle**: The process of finding the derivative using the fundamental limit definition: $f'(x) = \lim_{h \to 0} \frac{f(x+h) - f(x)}{h}$.
*   **Chain Rule**: The fundamental rule for differentiating **composite functions**. If $y = f(u)$ and $u = g(x)$, then $\frac{dy}{dx} = \frac{dy}{du} \cdot \frac{du}{dx}$.
*   **Implicit Differentiation**: A technique used when $y$ cannot be easily expressed explicitly in terms of $x$ (i.e., $f(x,y) = 0$). We differentiate both sides with respect to $x$ and solve for $\frac{dy}{dx}$.
*   **Parametric Differentiation**: When $x$ and $y$ are expressed in terms of a third variable (parameter) $t$ or $\theta$. $\frac{dy}{dx} = \frac{\frac{dy}{dt}}{\frac{dx}{dt}}$ provided $\frac{dx}{dt} \neq 0$.
*   **Logarithmic Differentiation**: A technique used to differentiate functions of the form $[f(x)]^{g(x)}$ or complex products/quotients. It involves taking the **natural logarithm (ln)** on both sides before differentiating.
*   **Higher Order Derivatives**: The derivative of a first derivative is the **second-order derivative** ($\frac{d^2y}{dx^2}$ or $f''(x)$ or $y_2$). This can be extended to $n$-th order.

### 1.4 Standard Derivative Formulae Checklist (Must Memorize for ISC)
*   $\frac{d}{dx}(x^n) = nx^{n-1}$
*   $\frac{d}{dx}(e^x) = e^x$
*   $\frac{d}{dx}(a^x) = a^x \ln a$
*   $\frac{d}{dx}(\ln x) = \frac{1}{x}$
*   $\frac{d}{dx}(\sin x) = \cos x$ ; $\frac{d}{dx}(\cos x) = -\sin x$
*   $\frac{d}{dx}(\tan x) = \sec^2 x$ ; $\frac{d}{dx}(\cot x) = -\csc^2 x$
*   $\frac{d}{dx}(\sec x) = \sec x \tan x$ ; $\frac{d}{dx}(\csc x) = -\csc x \cot x$
*   $\frac{d}{dx}(\sin^{-1} x) = \frac{1}{\sqrt{1 - x^2}}$ ; $\frac{d}{dx}(\cos^{-1} x) = -\frac{1}{\sqrt{1 - x^2}}$
*   $\frac{d}{dx}(\tan^{-1} x) = \frac{1}{1 + x^2}$ ; $\frac{d}{dx}(\cot^{-1} x) = -\frac{1}{1 + x^2}$
*   $\frac{d}{dx}(\sec^{-1} x) = \frac{1}{|x|\sqrt{x^2 - 1}}$ ; $\frac{d}{dx}(\csc^{-1} x) = -\frac{1}{|x|\sqrt{x^2 - 1}}$
## 2. Step-by-Step Derivations & Mechanisms

### 2.1 Mechanism: Logarithmic Differentiation
Used when $y = u(x)^{v(x)}$ or when dealing with a product/quotient of multiple functions.
**Step 1:** Let $y = u(x)^{v(x)}$.
**Step 2:** Take **natural log** ($\ln$ or $\log_e$) on both sides: $\ln y = v(x) \cdot \ln(u(x))$.
**Step 3:** Differentiate implicitly with respect to $x$:
$\frac{1}{y} \frac{dy}{dx} = v(x) \cdot \frac{d}{dx}[\ln(u(x))] + \ln(u(x)) \cdot \frac{d}{dx}[v(x)]$ (Using Product Rule)
**Step 4:** Substitute $y$ back into the equation:
$\frac{dy}{dx} = u(x)^{v(x)} \left[ v(x) \cdot \frac{u'(x)}{u(x)} + v'(x) \ln(u(x)) \right]$
*ISC Presentation Tip:* Always write "Taking logarithm on both sides" and "Differentiating w.r.t $x$".

### 2.2 Mechanism: Parametric Differentiation & Second Derivative
Given $x = f(t)$ and $y = g(t)$.
**First Derivative:**
1. Differentiate $x$ w.r.t $t$: $\frac{dx}{dt} = f'(t)$
2. Differentiate $y$ w.r.t $t$: $\frac{dy}{dt} = g'(t)$
3. Use formula: $\frac{dy}{dx} = \frac{dy/dt}{dx/dt} = \frac{g'(t)}{f'(t)}$

**Second Derivative (HIGH PROBABILITY ISC EXAM TRAP):**
To find $\frac{d^2y}{dx^2}$, you must differentiate $\frac{dy}{dx}$ with respect to **$x$**, not $t$.
$\frac{d^2y}{dx^2} = \frac{d}{dx} \left( \frac{dy}{dx} \right) = \frac{d}{dt} \left( \frac{dy}{dx} \right) \cdot \frac{dt}{dx}$
**Critical Step:** Multiply the derivative of $\frac{dy}{dx}$ (w.r.t $t$) by $\frac{dt}{dx}$ (which is the reciprocal of $\frac{dx}{dt}$).

### 2.3 Mechanism: Derivative of Inverse Trigonometric Functions using Substitution
Instead of direct chain rule (which gets messy), use trig substitutions to simplify before differentiating.
*   **Expression**: $\sqrt{a^2 - x^2}$ $\rightarrow$ **Substitute**: $x = a\sin\theta$ or $a\cos\theta$
*   **Expression**: $\sqrt{a^2 + x^2}$ $\rightarrow$ **Substitute**: $x = a\tan\theta$ or $a\cot\theta$
*   **Expression**: $\sqrt{x^2 - a^2}$ $\rightarrow$ **Substitute**: $x = a\sec\theta$ or $a\csc\theta$
*   **Expression**: $\sqrt{\frac{a-x}{a+x}}$ $\rightarrow$ **Substitute**: $x = a\cos(2\theta)$

**ISC Step-by-step example for $y = \tan^{-1}\left(\frac{2x}{1-x^2}\right)$:**
1. Let $x = \tan\theta \implies \theta = \tan^{-1}x$.
2. $y = \tan^{-1}\left(\frac{2\tan\theta}{1-\tan^2\theta}\right)$
3. $y = \tan^{-1}(\tan 2\theta)$
4. $y = 2\theta = 2\tan^{-1}x$ (Crucial: ensure domain constraints are met, though ISC usually assumes principal branch).
5. Differentiate: $\frac{dy}{dx} = 2 \cdot \frac{1}{1+x^2} = \frac{2}{1+x^2}$.

### 2.4 Derivation: Product Rule via First Principle
Let $f(x) = u(x)v(x)$.
$f'(x) = \lim_{h \to 0} \frac{u(x+h)v(x+h) - u(x)v(x)}{h}$
Add and subtract $u(x+h)v(x)$ in the numerator:
$= \lim_{h \to 0} \frac{u(x+h)v(x+h) - u(x+h)v(x) + u(x+h)v(x) - u(x)v(x)}{h}$
$= \lim_{h \to 0} \left[ u(x+h)\frac{v(x+h)-v(x)}{h} + v(x)\frac{u(x+h)-u(x)}{h} \right]$
Applying limit $h \to 0$:
$= u(x)v'(x) + v(x)u'(x)$.
## 3. Diagram Blueprints & Labeling Checklists

While pure differentiation lacks biological diagrams, the **geometrical meaning** of a derivative is highly visual and often tested conceptually in JEE and implicitly in ISC application questions.

### 3.1 Geometrical Blueprint: The Derivative as a Slope of Tangent
**Visualizing Differentiability:**
*   **Diagram:** A smooth curve $y = f(x)$. Two points on the curve: $P(c, f(c))$ and a nearby point $Q(c+h, f(c+h))$.
*   **Secant Line:** A line passing through $P$ and $Q$.
    *   *Label:* Slope of Secant $PQ = \frac{f(c+h) - f(c)}{h}$
*   **Tangent Line:** As $h \to 0$, point $Q$ slides along the curve towards $P$. The secant line becomes the tangent line at $P$.
    *   *Label:* Tangent at $P$. Slope $m = \lim_{h \to 0} \frac{f(c+h) - f(c)}{h} = f'(c)$.

### 3.2 Visual Non-Differentiability (Sharp Corners vs. Discontinuities)
**Diagram 1: The "Corner" (e.g., $y = |x|$ at $x=0$)**
*   *Feature:* A sharp point or "cusp".
*   *Analysis:* The slope of the tangent coming from the left (LHD = -1) is fundamentally different from the slope coming from the right (RHD = +1).
*   *Labeling Checklist:* Point $O(0,0)$ labeled as **"Continuous but Non-Differentiable"**.

**Diagram 2: Vertical Tangent (e.g., $y = \sqrt[3]{x}$ at $x=0$)**
*   *Feature:* Curve becomes completely vertical for an instant.
*   *Analysis:* The derivative $\to \infty$. Since the limit is not finite, it is non-differentiable.
*   *Labeling Checklist:* Tangent line coincides with Y-axis. $\frac{dy}{dx} \to \infty$.

**Conceptual Link (JEE speed):**
Whenever you see a modulus function $|g(x)|$, suspect non-differentiability at points where $g(x) = 0$.
## 4. "Avoid the Trap" & Distinction Tables (Objective vs Subjective traps)

### 4.1 Distinction: Continuity vs. Differentiability

| Feature | Continuity | Differentiability |
| :--- | :--- | :--- |
| **Meaning** | No breaks, jumps, or holes in the curve. | Smooth curve, no sharp corners, no vertical tangents. |
| **Mathematical Condition** | LHL = RHL = $f(c)$ | LHD = RHD (both finite) |
| **Relationship** | Differentiability implies Continuity. | Continuity DOES NOT imply Differentiability. |
| **Common Traps** | Assuming $y = \frac{1}{x}$ is continuous everywhere. (It is discontinuous at $x=0$). | Assuming $|x|$ is differentiable at $x=0$. It forms a sharp 'V' corner. |

### 4.2 ISC Subjective Formatting Traps (How to lose marks)
*   **The Second Derivative Parametric Trap:** As shown in Section 2, calculating $\frac{d^2y}{dx^2}$ for parametric equations by simply dividing $\frac{d^2y}{dt^2}$ by $\frac{d^2x}{dt^2}$ is a **FATAL ERROR**. You must multiply by $\frac{dt}{dx}$.
*   **Missing Chain Rule Links:** In $y = \sin^3(4x)$, students often write $3\sin^2(4x)$ and stop.
    *   *Correction:* Differentiate outside-in: Power $\to$ Trig $\to$ Algebraic. $3\sin^2(4x) \cdot \cos(4x) \cdot 4$.
*   **Logarithmic Differentiation Presentation:** Forgetting to write "taking logarithm on both sides" will lose step marks in ISC. Also, if $y = x^x + (\sin x)^x$, you **CANNOT** write $\ln y = x\ln x + x\ln(\sin x)$. Logarithm over addition ($\ln(A+B)$) does not distribute!
    *   *ISC Solution:* Let $u = x^x$ and $v = (\sin x)^x$. Solve $\frac{du}{dx}$ and $\frac{dv}{dx}$ separately, then sum them up: $\frac{dy}{dx} = \frac{du}{dx} + \frac{dv}{dx}$.

### 4.3 NEET/JEE Objective Speed Traps
*   **The Inverse Trig Domain Trap:** When simplifying $y = \sin^{-1}(\sin 2x)$, the answer is $2x$ ONLY IF $2x \in [-\frac{\pi}{2}, \frac{\pi}{2}]$. If $2x$ is outside this principal domain, you must use allied angle formulas to bring it inside before differentiating.
*   **L'Hôpital's Rule Overuse:** In limits related to derivatives, students apply L'Hôpital without checking if it's a $0/0$ or $\infty/\infty$ indeterminate form, leading to wrong answers instantly. Always plug in the limit value first.
## 5. High-Yield Worked Model Problems

### Problem 1: Complex Logarithmic Differentiation (ISC Long Answer Model)
**Question:** If $x^y = e^{x-y}$, prove that $\frac{dy}{dx} = \frac{\log x}{(1 + \log x)^2}$
*Note: In Calculus, $\log$ implies natural log ($\ln$) unless specified otherwise.*

**ISC Subjective Step-by-Step:**
1.  **Given equation:** $x^y = e^{x-y}$
2.  **Take logarithm on both sides:**
    $\log(x^y) = \log(e^{x-y})$
    $y \log x = (x-y) \log e$
3.  **Use property $\log e = 1$:**
    $y \log x = x - y$
4.  **Isolate $y$:** This is a crucial simplification step before differentiating!
    $y \log x + y = x$
    $y(1 + \log x) = x \implies y = \frac{x}{1 + \log x}$
5.  **Differentiate w.r.t $x$ using Quotient Rule:**
    $\frac{dy}{dx} = \frac{(1 + \log x) \cdot \frac{d}{dx}(x) - x \cdot \frac{d}{dx}(1 + \log x)}{(1 + \log x)^2}$
    $\frac{dy}{dx} = \frac{(1 + \log x)(1) - x(0 + \frac{1}{x})}{(1 + \log x)^2}$
    $\frac{dy}{dx} = \frac{1 + \log x - 1}{(1 + \log x)^2}$
    **$\frac{dy}{dx} = \frac{\log x}{(1 + \log x)^2}$ (Hence Proved)**

**JEE Speed Hack:** Always try to explicitly express $y$ in terms of $x$ (or $x$ in terms of $y$) before using implicit differentiation if it simplifies the expression algebraically. It avoids messy $\frac{dy}{dx}$ terms scattered everywhere.

### Problem 2: The Parametric Second Derivative Trap
**Question:** If $x = a(\cos t + t\sin t)$ and $y = a(\sin t - t\cos t)$, find $\frac{d^2y}{dx^2}$ at $t = \frac{\pi}{4}$.

**ISC Subjective Step-by-Step:**
1.  **Find $\frac{dx}{dt}$:**
    $\frac{dx}{dt} = a[-\sin t + (\sin t + t\cos t)]$ (Product rule on $t\sin t$)
    $\frac{dx}{dt} = at\cos t$
2.  **Find $\frac{dy}{dt}$:**
    $\frac{dy}{dt} = a[\cos t - (\cos t - t\sin t)]$ (Product rule on $t\cos t$)
    $\frac{dy}{dt} = at\sin t$
3.  **Find $\frac{dy}{dx}$:**
    $\frac{dy}{dx} = \frac{dy/dt}{dx/dt} = \frac{at\sin t}{at\cos t} = \tan t$
4.  **Find $\frac{d^2y}{dx^2}$ (CRITICAL STEP):**
    $\frac{d^2y}{dx^2} = \frac{d}{dx}(\tan t) = \sec^2 t \cdot \mathbf{\frac{dt}{dx}}$
    Substitute $\frac{dt}{dx} = \frac{1}{at\cos t}$:
    $\frac{d^2y}{dx^2} = \sec^2 t \cdot \frac{1}{at\cos t} = \frac{\sec^3 t}{at}$
5.  **Evaluate at $t = \frac{\pi}{4}$:**
    $\frac{d^2y}{dx^2} \Big|_{t=\pi/4} = \frac{(\sqrt{2})^3}{a(\pi/4)} = \frac{2\sqrt{2}}{\frac{a\pi}{4}} = \frac{8\sqrt{2}}{a\pi}$

### Problem 3: Implicit Higher Order Derivative (Proving Type)
**Question:** If $y = A\sin x + B\cos x$, prove that $\frac{d^2y}{dx^2} + y = 0$.

**Step-by-Step (ISC & Speed Method are identical here):**
1.  **Differentiate w.r.t $x$:**
    $y_1 = \frac{dy}{dx} = A\cos x - B\sin x$
2.  **Differentiate again w.r.t $x$:**
    $y_2 = \frac{d^2y}{dx^2} = -A\sin x - B\cos x$
3.  **Factor out the negative sign:**
    $y_2 = -(A\sin x + B\cos x)$
4.  **Substitute original $y$:**
    $y_2 = -y \implies \frac{d^2y}{dx^2} + y = 0$ (Proved)
