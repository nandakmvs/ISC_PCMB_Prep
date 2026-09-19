# Chapter 2: Inverse Trigonometric Functions

## 1. Exhaustive Theory & Precise ISC Terminology

**Inverse Trigonometric Functions** are the inverse functions of the trigonometric functions, with appropriately restricted domains to make them bijective.

**Principal Value Branches (PVB):**
1. $y = \sin^{-1}x$: Domain $[-1, 1]$, Range (PVB) $[-\frac{\pi}{2}, \frac{\pi}{2}]$
2. $y = \cos^{-1}x$: Domain $[-1, 1]$, Range (PVB) $[0, \pi]$
3. $y = \tan^{-1}x$: Domain $R$, Range (PVB) $(-\frac{\pi}{2}, \frac{\pi}{2})$
4. $y = \cot^{-1}x$: Domain $R$, Range (PVB) $(0, \pi)$
5. $y = \sec^{-1}x$: Domain $R - (-1, 1)$, Range (PVB) $[0, \pi] - \{\frac{\pi}{2}\}$
6. $y = \text{cosec}^{-1}x$: Domain $R - (-1, 1)$, Range (PVB) $[-\frac{\pi}{2}, \frac{\pi}{2}] - \{0\}$

**Properties of Inverse Trigonometric Functions:**
- **Self-cancelling**: $\sin(\sin^{-1}x) = x$ for $x \in [-1, 1]$; $\sin^{-1}(\sin x) = x$ for $x \in [-\frac{\pi}{2}, \frac{\pi}{2}]$
- **Reciprocal**: $\sin^{-1}(\frac{1}{x}) = \text{cosec}^{-1}x$ for $x \ge 1$ or $x \le -1$. Similar for $\cos$ and $\tan$.
- **Negative Arguments**: 
  - $\sin^{-1}(-x) = -\sin^{-1}x$, $\tan^{-1}(-x) = -\tan^{-1}x$, $\text{cosec}^{-1}(-x) = -\text{cosec}^{-1}x$
  - $\cos^{-1}(-x) = \pi - \cos^{-1}x$, $\cot^{-1}(-x) = \pi - \cot^{-1}x$, $\sec^{-1}(-x) = \pi - \sec^{-1}x$
- **Complementary**: 
  - $\sin^{-1}x + \cos^{-1}x = \frac{\pi}{2}$, $x \in [-1, 1]$
  - $\tan^{-1}x + \cot^{-1}x = \frac{\pi}{2}$, $x \in R$
  - $\text{cosec}^{-1}x + \sec^{-1}x = \frac{\pi}{2}$, $|x| \ge 1$

## 2. Step-by-Step Derivations & Mechanisms

**Derivation of $\cos^{-1}(-x) = \pi - \cos^{-1}x$:**
Let $y = \cos^{-1}(-x)$. Then $\cos y = -x$, where $y \in [0, \pi]$.
$x = -\cos y = \cos(\pi - y)$.
Since $y \in [0, \pi]$, we have $\pi - y \in [0, \pi]$.
Therefore, we can take $\cos^{-1}$ on both sides: $\cos^{-1}x = \pi - y$.
Substitute back $y$: $\cos^{-1}x = \pi - \cos^{-1}(-x)$.
Rearranging: $\cos^{-1}(-x) = \pi - \cos^{-1}x$.

**Mechanism for Simplification Using Substitutions:**
- For $\sqrt{a^2 - x^2}$, substitute $x = a \sin \theta$ or $a \cos \theta$.
- For $\sqrt{a^2 + x^2}$, substitute $x = a \tan \theta$ or $a \cot \theta$.
- For $\sqrt{x^2 - a^2}$, substitute $x = a \sec \theta$ or $a \text{cosec} \theta$.
- For $\sqrt{\frac{a-x}{a+x}}$, substitute $x = a \cos 2\theta$.

## 3. Diagram Blueprints & Labeling Checklists

- **Graphs**:
  - $\sin^{-1}x$: An S-curve restricted between $x = -1$ and $x = 1$, bounded by $y = -\pi/2$ and $y = \pi/2$.
  - $\cos^{-1}x$: A descending curve from $(-1, \pi)$ through $(0, \pi/2)$ ending at $(1, 0)$.
  - **Label Checklist**: Always label domain limits on X-axis and PVB limits on Y-axis. Identify intercepts clearly.

## 4. "Avoid the Trap" & Distinction Tables

| Trap / Common Mistake | Strategy / Fact to Remember |
| :--- | :--- |
| Writing $\sin^{-1}(\sin \frac{2\pi}{3}) = \frac{2\pi}{3}$ | The angle $\frac{2\pi}{3}$ is NOT in the PVB $[-\frac{\pi}{2}, \frac{\pi}{2}]$. Convert it first: $\sin(\pi - \frac{\pi}{3}) = \sin(\frac{\pi}{3})$. Hence, answer is $\frac{\pi}{3}$. |
| Misapplying properties outside domain | $\tan^{-1}x + \tan^{-1}y = \tan^{-1}(\frac{x+y}{1-xy})$ is only valid if $xy < 1$. If $xy > 1, x>0, y>0$, add $\pi$. |
| Notation confusion | $\sin^{-1}x$ is NOT $(\sin x)^{-1}$. The latter is $\frac{1}{\sin x} = \text{cosec} x$. |

## 5. High-Yield Worked Model Problems

**Problem (ISC Step-by-Step)**: Prove that $2 \tan^{-1}(\frac{1}{2}) + \tan^{-1}(\frac{1}{7}) = \tan^{-1}(\frac{31}{17})$.
**Solution**:
1. First, apply $2\tan^{-1}x = \tan^{-1}\left(\frac{2x}{1-x^2}\right)$ for $|x| < 1$.
   $2\tan^{-1}(\frac{1}{2}) = \tan^{-1}\left(\frac{2(1/2)}{1 - (1/2)^2}\right) = \tan^{-1}\left(\frac{1}{1 - 1/4}\right) = \tan^{-1}(\frac{4}{3})$.
2. Now substitute back into the LHS: $\tan^{-1}(\frac{4}{3}) + \tan^{-1}(\frac{1}{7})$.
3. Apply $\tan^{-1}x + \tan^{-1}y = \tan^{-1}(\frac{x+y}{1-xy})$ since $x \cdot y = \frac{4}{3} \times \frac{1}{7} = \frac{4}{21} < 1$.
   $= \tan^{-1}\left(\frac{4/3 + 1/7}{1 - (4/3)(1/7)}\right) = \tan^{-1}\left(\frac{28+3}{21 - 4}\right) = \tan^{-1}(\frac{31}{17})$.
4. LHS = RHS. Hence proved.

**Problem (NEET/JEE Speed Method)**: Find the value of $\cos^{-1}(\cos(\frac{13\pi}{6}))$.
**Solution**:
$\frac{13\pi}{6} = 2\pi + \frac{\pi}{6}$.
$\cos(2\pi + \theta) = \cos\theta$. Thus, $\cos(\frac{13\pi}{6}) = \cos(\frac{\pi}{6})$.
Since $\frac{\pi}{6}$ is in the PVB $[0, \pi]$, $\cos^{-1}(\cos(\frac{\pi}{6})) = \frac{\pi}{6}$.
Speed tip: Just divide $13$ by $6$. $13 = 2 \times 6 + 1$. Nearest even multiple of $\pi$ is $2\pi$. The remainder provides the principal angle $\pi/6$.
