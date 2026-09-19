# 02. Inverse Trigonometric Functions

## PART 1: Exhaustive Theory & Precise ISC Terminology

### 1.1 Introduction to Inverse Functions
A function $f: A \to B$ has an inverse function $f^{-1}: B \to A$ **if and only if** $f$ is a **bijective** function (i.e., it must be both **one-one** (injective) and **onto** (surjective)). 
Trigonometric functions are inherently periodic and therefore **many-one** over their natural domains. To define their inverses, we must artificially **restrict their domains** to intervals where they become bijective.

**ISC Keyword Focus:** Always state the **Principal Value Branch (PVB)** when defining an inverse trigonometric function.

### 1.2 The Principal Value Branches (Domain and Range)
The standard restricted domain chosen for a trigonometric function to make it bijective corresponds to the **Principal Range** of its inverse function. 
*   **Domain:** The set of valid input values ($x$) for the inverse function.
*   **Range (Principal Value Branch):** The set of valid output angles ($\theta$).

| Function ($y = f(x)$) | Domain ($x$) | Principal Value Branch / Range ($y$) |
| :--- | :--- | :--- |
| **$y = \sin^{-1} x$** | $[-1, 1]$ | $[-\frac{\pi}{2}, \frac{\pi}{2}]$ |
| **$y = \cos^{-1} x$** | $[-1, 1]$ | $[0, \pi]$ |
| **$y = \tan^{-1} x$** | $\mathbb{R}$ (All Reals) | $(-\frac{\pi}{2}, \frac{\pi}{2})$ |
| **$y = \cot^{-1} x$** | $\mathbb{R}$ (All Reals) | $(0, \pi)$ |
| **$y = \sec^{-1} x$** | $\mathbb{R} - (-1, 1)$ or $(-\infty, -1] \cup [1, \infty)$ | $[0, \pi] - \{\frac{\pi}{2}\}$ |
| **$y = \text{cosec}^{-1} x$** | $\mathbb{R} - (-1, 1)$ or $(-\infty, -1] \cup [1, \infty)$ | $[-\frac{\pi}{2}, \frac{\pi}{2}] - \{0\}$ |

**Note on Notation:** 
*   $\sin^{-1} x$ is also written as $\text{arcsin } x$.
*   $\sin^{-1} x \neq (\sin x)^{-1}$. The latter is $\frac{1}{\sin x} = \text{cosec } x$.

### 1.3 Key Concepts for ISC Board
1.  **Principal Value:** The value of an inverse trigonometric function which lies in its principal value branch is called the principal value of that inverse trigonometric function.
2.  **Domain Checking:** Before applying any property, the argument must strictly belong to the domain of the respective inverse trigonometric function. In ISC subjective papers, explicit mention of "for $x \in \dots$" fetches stepwise marks.
## PART 2: Step-by-Step Derivations & Mechanisms

In ISC board exams, direct application of formulas is expected, but derivations of key properties often appear as 2- or 3-mark proofs.

### 2.1 Self-Adjusting Properties
**Property 1:** $f(f^{-1}(x)) = x$
*   $\sin(\sin^{-1} x) = x$ for $x \in [-1, 1]$
*   $\cos(\cos^{-1} x) = x$ for $x \in [-1, 1]$
*   $\tan(\tan^{-1} x) = x$ for $x \in \mathbb{R}$

**Property 2:** $f^{-1}(f(x)) = x$ (Only valid if $x$ is in the principal value branch)
*   $\sin^{-1}(\sin x) = x$ for $x \in [-\frac{\pi}{2}, \frac{\pi}{2}]$
*   $\cos^{-1}(\cos x) = x$ for $x \in [0, \pi]$

### 2.2 Property of Negative Arguments
**Family 1 (Odd-like nature):** $\sin^{-1}$, $\tan^{-1}$, $\text{cosec}^{-1}$
*   $\sin^{-1}(-x) = -\sin^{-1} x$, for $x \in [-1, 1]$
*   $\tan^{-1}(-x) = -\tan^{-1} x$, for $x \in \mathbb{R}$
*   $\text{cosec}^{-1}(-x) = -\text{cosec}^{-1} x$, for $|x| \ge 1$
*Mechanism:* Let $\sin^{-1}(-x) = \theta \implies -x = \sin\theta \implies x = -\sin\theta = \sin(-\theta) \implies \sin^{-1}x = -\theta \implies \theta = -\sin^{-1}x$.

**Family 2 (Supplementary nature):** $\cos^{-1}$, $\cot^{-1}$, $\sec^{-1}$
*   $\cos^{-1}(-x) = \pi - \cos^{-1} x$, for $x \in [-1, 1]$
*   $\cot^{-1}(-x) = \pi - \cot^{-1} x$, for $x \in \mathbb{R}$
*   $\sec^{-1}(-x) = \pi - \sec^{-1} x$, for $|x| \ge 1$
*Mechanism (ISC Step-by-step):* 
1. Let $\cos^{-1}(-x) = \theta$. (where $\theta \in [0, \pi]$)
2. $-x = \cos \theta \implies x = -\cos \theta$
3. $x = \cos(\pi - \theta)$ (Since $\cos(\pi-\theta) = -\cos\theta$ and $\pi-\theta \in [0, \pi]$)
4. $\cos^{-1} x = \pi - \theta \implies \theta = \pi - \cos^{-1} x$.

### 2.3 Reciprocal Properties
*   $\sin^{-1}(\frac{1}{x}) = \text{cosec}^{-1} x$, for $|x| \ge 1$
*   $\cos^{-1}(\frac{1}{x}) = \sec^{-1} x$, for $|x| \ge 1$
*   $\tan^{-1}(\frac{1}{x}) = \cot^{-1} x$ for $x > 0$  **(Note: If $x < 0$, $\tan^{-1}(\frac{1}{x}) = -\pi + \cot^{-1} x$)**

### 2.4 Complementary Angle Properties
*   $\sin^{-1} x + \cos^{-1} x = \frac{\pi}{2}$, for $x \in [-1, 1]$
*   $\tan^{-1} x + \cot^{-1} x = \frac{\pi}{2}$, for $x \in \mathbb{R}$
*   $\sec^{-1} x + \text{cosec}^{-1} x = \frac{\pi}{2}$, for $|x| \ge 1$
*Derivation:* Let $\sin^{-1} x = \theta \implies x = \sin\theta = \cos(\frac{\pi}{2} - \theta)$. Therefore, $\cos^{-1} x = \frac{\pi}{2} - \theta = \frac{\pi}{2} - \sin^{-1} x$.

### 2.5 Sum and Difference Properties
**Formula 1 (Addition):**
$\tan^{-1} x + \tan^{-1} y = \tan^{-1}\left(\frac{x+y}{1-xy}\right)$, if $xy < 1$
*(If $xy > 1$ and $x>0, y>0$, then $\tan^{-1} x + \tan^{-1} y = \pi + \tan^{-1}\left(\frac{x+y}{1-xy}\right)$)*

**Formula 2 (Subtraction):**
$\tan^{-1} x - \tan^{-1} y = \tan^{-1}\left(\frac{x-y}{1+xy}\right)$, if $xy > -1$

**Multiple Angles (Crucial for Substitution):**
*   $2\tan^{-1} x = \sin^{-1}\left(\frac{2x}{1+x^2}\right)$, for $|x| \le 1$
*   $2\tan^{-1} x = \cos^{-1}\left(\frac{1-x^2}{1+x^2}\right)$, for $x \ge 0$
*   $2\tan^{-1} x = \tan^{-1}\left(\frac{2x}{1-x^2}\right)$, for $-1 < x < 1$
## PART 3: Diagram Blueprints & Labeling Checklists

For ISC examination, if asked to draw graphs of inverse trigonometric functions, strict adherence to the principal value branches is mandatory. Missing labels often lead to point deductions.

### Blueprint 1: Graph of $y = \sin^{-1} x$
*   **Shape:** An inverted "S" shape curve confined within a bounding box.
*   **X-axis bounds:** $[-1, 1]$. Label $x = -1$, $x = 0$ (origin), $x = 1$.
*   **Y-axis bounds:** $[-\frac{\pi}{2}, \frac{\pi}{2}]$. Label $y = -\frac{\pi}{2}$, $y = \frac{\pi}{2}$.
*   **Origin:** Passes exactly through $(0,0)$.
*   **Endpoints Checklist:** Mark solid dots at $(-1, -\frac{\pi}{2})$ and $(1, \frac{\pi}{2})$.

### Blueprint 2: Graph of $y = \cos^{-1} x$
*   **Shape:** A smooth decreasing curve passing through the y-axis.
*   **X-axis bounds:** $[-1, 1]$. Label $x = -1$, $x = 0$, $x = 1$.
*   **Y-axis bounds:** $[0, \pi]$. Label $y = 0$, $y = \frac{\pi}{2}$, $y = \pi$.
*   **Y-intercept:** Passes through $(0, \frac{\pi}{2})$.
*   **Endpoints Checklist:** Mark solid dots at $(-1, \pi)$ and $(1, 0)$.

### Blueprint 3: Graph of $y = \tan^{-1} x$
*   **Shape:** A smooth "S" curve passing through origin, stretching horizontally to infinity.
*   **Asymptotes (CRITICAL):** Draw dashed horizontal lines at $y = \frac{\pi}{2}$ and $y = -\frac{\pi}{2}$.
*   **Origin:** Passes through $(0,0)$.
*   **ISC Labeling Checklist:** Mention "Horizontal Asymptote $y = \pm\pi/2$". The curve must *approach* but *never touch* these lines.

### Blueprint 4: Graph of $y = \sec^{-1} x$
*   **Shape:** Two disconnected branches.
*   **Asymptote:** Draw a dashed horizontal line at $y = \frac{\pi}{2}$.
*   **X-axis:** The region $(-1, 1)$ must remain completely EMPTY (no curve).
*   **Branches:** 
    *   Right branch starts from a solid dot at $(1, 0)$ and curves up, asymptotically approaching $y = \frac{\pi}{2}$ as $x \to \infty$.
    *   Left branch starts from a solid dot at $(-1, \pi)$ and curves down, asymptotically approaching $y = \frac{\pi}{2}$ as $x \to -\infty$.

### ISC Master Diagram Checklist:
1.  Are arrows present on the $X$ and $Y$ axes?
2.  Is the origin labeled 'O' or $(0,0)$?
3.  Are asymptotes marked as dashed lines and their equations written?
4.  Are domain limits strictly respected (no extension of curve beyond $[-1,1]$ for sin⁻¹ and cos⁻¹)?
## PART 4: "Avoid the Trap" & Distinction Tables

### TRAP 1: The Domain Overshoot (Most Common ISC Error)
**Scenario:** Evaluate $\sin^{-1}(\sin \frac{2\pi}{3})$.
*   **The Trap (Student's immediate instinct):** Apply $\sin^{-1}(\sin x) = x$ and write answer = $\frac{2\pi}{3}$.
*   **Why it's wrong:** The principal range of $\sin^{-1} x$ is $[-\frac{\pi}{2}, \frac{\pi}{2}]$. The angle $\frac{2\pi}{3} (120^\circ)$ falls outside this range.
*   **The ISC Subjective Correction:**
    *   $\sin^{-1}(\sin \frac{2\pi}{3}) = \sin^{-1}(\sin(\pi - \frac{\pi}{3}))$
    *   $= \sin^{-1}(\sin \frac{\pi}{3})$ 
    *   $= \frac{\pi}{3}$. (Since $\frac{\pi}{3} \in [-\frac{\pi}{2}, \frac{\pi}{2}]$)

### TRAP 2: The Negative Argument Blunder
**Scenario:** Evaluate $\cos^{-1}(-\frac{1}{2})$.
*   **The Trap:** Treating it like sine: $\cos^{-1}(-\frac{1}{2}) \rightarrow -\cos^{-1}(\frac{1}{2}) = -\frac{\pi}{3}$.
*   **Why it's wrong:** $\cos^{-1}(-x) = \pi - \cos^{-1} x$.
*   **The Correct Path:** $\cos^{-1}(-\frac{1}{2}) = \pi - \cos^{-1}(\frac{1}{2}) = \pi - \frac{\pi}{3} = \frac{2\pi}{3}$.

### DISTINCTION TABLE: General vs. Principal Solutions
| Context | Expression | Correct Interpretation / Action |
| :--- | :--- | :--- |
| **Solving Trigonometric Equations** | $\sin x = \frac{1}{2}$ | Finding $x$. Requires general solution: $x = n\pi + (-1)^n \frac{\pi}{6}$ |
| **Evaluating Inverse Functions** | $x = \sin^{-1}(\frac{1}{2})$ | Finding a specific value. Requires principal value: $x = \frac{\pi}{6}$ strictly. |
| **Algebraic Notation** | $\sin^{-1} x$ | Refers to the INVERSE function. Evaluates to an angle. |
| **Algebraic Notation** | $(\sin x)^{-1}$ | Refers to the RECIPROCAL $\frac{1}{\sin x} = \text{cosec } x$. Evaluates to a ratio. |

### TRAP 3: $\tan^{-1} x + \tan^{-1} y$ Condition Ignorance
When applying $\tan^{-1} x + \tan^{-1} y = \tan^{-1}\frac{x+y}{1-xy}$, students frequently ignore the $xy < 1$ condition.
*   **Example:** $\tan^{-1}(2) + \tan^{-1}(3)$.
*   Here $x=2, y=3 \implies xy = 6 > 1$.
*   *Trap:* $\tan^{-1}(\frac{2+3}{1-6}) = \tan^{-1}(-1) = -\frac{\pi}{4}$.
*   *Correct approach (NEET/JEE & ISC):* Since $xy > 1$, add $\pi$. Answer = $\pi + \tan^{-1}(-1) = \pi - \frac{\pi}{4} = \frac{3\pi}{4}$.
## PART 5: High-Yield Worked Model Problems

### Model 1: Simplification using Trigonometric Substitution (ISC Staple)
**Problem:** Write $\tan^{-1}\left(\frac{\sqrt{1+x^2} - 1}{x}\right)$, $x \neq 0$ in the simplest form.
**ISC Step-by-Step Solution:**
1.  **Substitution:** Let $x = \tan \theta$, which implies $\theta = \tan^{-1} x$.
2.  **Substitute into expression:** 
    $\tan^{-1}\left(\frac{\sqrt{1+\tan^2\theta} - 1}{\tan\theta}\right)$
3.  **Use trig identities:** $1+\tan^2\theta = \sec^2\theta$.
    $\tan^{-1}\left(\frac{\sec\theta - 1}{\tan\theta}\right)$
4.  **Convert to sin/cos:**
    $\tan^{-1}\left(\frac{\frac{1}{\cos\theta} - 1}{\frac{\sin\theta}{\cos\theta}}\right) = \tan^{-1}\left(\frac{1 - \cos\theta}{\sin\theta}\right)$
5.  **Use half-angle formulas (Crucial ISC step):**
    $1 - \cos\theta = 2\sin^2(\frac{\theta}{2})$ and $\sin\theta = 2\sin(\frac{\theta}{2})\cos(\frac{\theta}{2})$
6.  **Simplify:**
    $\tan^{-1}\left(\frac{2\sin^2(\frac{\theta}{2})}{2\sin(\frac{\theta}{2})\cos(\frac{\theta}{2})}\right) = \tan^{-1}(\tan \frac{\theta}{2})$
7.  **Final Evaluation:**
    $= \frac{\theta}{2} = \frac{1}{2} \tan^{-1} x$.

### Model 2: Equation Solving
**Problem:** Solve for $x$: $\tan^{-1} 2x + \tan^{-1} 3x = \frac{\pi}{4}$.
**ISC Step-by-Step Solution:**
1.  **Apply Formula:** Assuming $2x \cdot 3x < 1$.
    $\tan^{-1}\left(\frac{2x + 3x}{1 - (2x)(3x)}\right) = \frac{\pi}{4}$
2.  **Shift function:**
    $\frac{5x}{1 - 6x^2} = \tan(\frac{\pi}{4}) = 1$
3.  **Form Quadratic Equation:**
    $5x = 1 - 6x^2 \implies 6x^2 + 5x - 1 = 0$
4.  **Factorize:**
    $6x^2 + 6x - x - 1 = 0 \implies 6x(x+1) - 1(x+1) = 0$
    $(6x - 1)(x + 1) = 0$
    $x = \frac{1}{6}$ or $x = -1$.
5.  **Check Roots (MANDATORY IN ISC):**
    *   If $x = -1$, LHS $= \tan^{-1}(-2) + \tan^{-1}(-3)$ (Negative sum, but RHS is positive $\pi/4$. Rejected).
    *   If $x = \frac{1}{6}$, $2x \cdot 3x = 6(\frac{1}{36}) = \frac{1}{6} < 1$. Condition satisfied.
    *   **Answer:** $x = \frac{1}{6}$.

### Model 3: Inter-conversion of Inverse Functions (NEET/JEE Speed Method vs ISC Method)
**Problem:** Evaluate $\sin(\cot^{-1} x)$.

**ISC Subjective Method:**
1. Let $\cot^{-1} x = \theta \implies \cot \theta = x$.
2. We need to find $\sin \theta$.
3. We know $\text{cosec}^2\theta = 1 + \cot^2\theta = 1 + x^2$.
4. $\text{cosec} \theta = \sqrt{1+x^2}$ (taking positive root for principal branch).
5. Therefore, $\sin \theta = \frac{1}{\text{cosec}\theta} = \frac{1}{\sqrt{1+x^2}}$.
6. Final answer: $\frac{1}{\sqrt{1+x^2}}$.

**NEET/JEE Speed Method (Right Triangle Approach):**
1. $\cot = \frac{\text{Adjacent}}{\text{Opposite}} = \frac{x}{1}$.
2. Draw a right triangle: Base $= x$, Perpendicular $= 1$.
3. Hypotenuse $= \sqrt{x^2 + 1}$.
4. The outer function is $\sin$, so we need $\sin = \frac{\text{Opposite}}{\text{Hypotenuse}}$.
5. Directly read from triangle: $\sin = \frac{1}{\sqrt{x^2+1}}$. (Done in 5 seconds).
