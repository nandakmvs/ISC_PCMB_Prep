# Chapter 5 & 6: Continuity, Differentiability & Derivatives

## 1. Exhaustive Theory & Precise ISC Terminology

**Continuity**: A function $f(x)$ is continuous at a point $x=a$ if $\lim_{x \to a^-} f(x) = \lim_{x \to a^+} f(x) = f(a)$. A polynomial is everywhere continuous.
**Differentiability**: A function $f$ is differentiable at $c$ if the left-hand derivative (LHD) equals the right-hand derivative (RHD) at $c$. Note: **Every differentiable function is continuous, but the converse is not true.**

### Algebra of Derivatives (Rules)
- Sum/Difference: $\frac{d}{dx}(u \pm v) = \frac{du}{dx} \pm \frac{dv}{dx}$
- **Product Rule**: $\frac{d}{dx}(uv) = u\frac{dv}{dx} + v\frac{du}{dx}$
- **Quotient Rule**: $\frac{d}{dx}(\frac{u}{v}) = \frac{v\frac{du}{dx} - u\frac{dv}{dx}}{v^2}$
- **Chain Rule**: If $y = f(u)$ and $u = g(x)$, then $\frac{dy}{dx} = \frac{dy}{du} \cdot \frac{du}{dx}$

### Specific Differentiation Methods
1. **Implicit Differentiation**: When relations are given as $f(x, y) = 0$. Differentiate both sides wrt $x$, treating $y$ as a function of $x$ (so append $\frac{dy}{dx}$ when differentiating $y$ terms), and solve for $\frac{dy}{dx}$.
2. **Logarithmic Differentiation**: Used for functions of the form $[f(x)]^{g(x)}$ or complex products/quotients. Take natural log ($\ln$) on both sides, use log properties, then differentiate implicitly.
3. **Parametric Differentiation**: If $x = f(t)$ and $y = g(t)$, then $\frac{dy}{dx} = \frac{dy/dt}{dx/dt}$ (provided $dx/dt \neq 0$).
4. **Higher Order Derivatives**: $\frac{d^2y}{dx^2}$ is the derivative of $\frac{dy}{dx}$. Note: For parametric equations, $\frac{d^2y}{dx^2} = \frac{d}{dx}\left(\frac{dy}{dx}\right) = \frac{d}{dt}\left(\frac{dy}{dx}\right) \cdot \frac{dt}{dx}$.

## 2. Step-by-Step Derivations & Mechanisms

**Mechanism for Logarithmic Differentiation:**
Given $y = u(x)^{v(x)}$
1. Take natural logarithm: $\ln y = v(x) \ln u(x)$
2. Differentiate with respect to $x$: $\frac{1}{y} \frac{dy}{dx} = v(x) \cdot \frac{1}{u(x)} \cdot u'(x) + \ln u(x) \cdot v'(x)$ (using product rule).
3. Isolate $\frac{dy}{dx}$ and substitute $y$ back: $\frac{dy}{dx} = y \left[ \frac{v(x)}{u(x)} u'(x) + v'(x) \ln u(x) \right]$.

## 3. Diagram Blueprints & Labeling Checklists

- **Continuity vs Differentiability Visualization**:
  - Draw a smooth curve. Label as continuous and differentiable.
  - Draw a curve with a "sharp point" or "cusp" (like $y = |x|$ at $x=0$). Label as continuous but NOT differentiable at the cusp.
  - Draw a curve with a jump or hole. Label as discontinuous (and thus non-differentiable).

## 4. "Avoid the Trap" & Distinction Tables

| Trap / Common Mistake | Strategy / Fact to Remember |
| :--- | :--- |
| Forgetting Chain Rule | Always check if the argument of a function is anything other than '$x$'. E.g., derivative of $\sin(x^2)$ is $\cos(x^2) \cdot 2x$, not just $\cos(x^2)$. |
| Incorrect 2nd Derivative of Parametrics | $\frac{d^2y}{dx^2} \neq \frac{d^2y/dt^2}{d^2x/dt^2}$. You MUST differentiate $\frac{dy}{dx}$ with respect to $t$ and multiply by $\frac{dt}{dx}$. |
| Differentiating $a^x$ vs $x^a$ vs $x^x$ | $x^a$ uses power rule ($ax^{a-1}$). $a^x$ uses exponential rule ($a^x \ln a$). $x^x$ requires **logarithmic differentiation**. |

## 5. High-Yield Worked Model Problems

**Problem (ISC Step-by-Step)**: If $x = a(\theta - \sin\theta)$ and $y = a(1 - \cos\theta)$, find $\frac{d^2y}{dx^2}$ at $\theta = \frac{\pi}{2}$.
**Solution**:
1. Find $\frac{dx}{d\theta} = a(1 - \cos\theta)$ and $\frac{dy}{d\theta} = a(0 - (-\sin\theta)) = a\sin\theta$.
2. $\frac{dy}{dx} = \frac{dy/d\theta}{dx/d\theta} = \frac{a\sin\theta}{a(1-\cos\theta)} = \frac{2\sin(\theta/2)\cos(\theta/2)}{2\sin^2(\theta/2)} = \cot(\frac{\theta}{2})$.
3. Find second derivative: $\frac{d^2y}{dx^2} = \frac{d}{dx}(\cot(\frac{\theta}{2})) = \frac{d}{d\theta}(\cot(\frac{\theta}{2})) \cdot \frac{d\theta}{dx}$.
4. $\frac{d^2y}{dx^2} = -\frac{1}{2}\text{cosec}^2(\frac{\theta}{2}) \cdot \frac{1}{a(1-\cos\theta)}$.
5. Since $1-\cos\theta = 2\sin^2(\theta/2)$, we have $\frac{d^2y}{dx^2} = \frac{-\text{cosec}^4(\theta/2)}{4a}$.
6. At $\theta = \pi/2$, $\theta/2 = \pi/4$. $\text{cosec}(\pi/4) = \sqrt{2}$. Result: $\frac{-(\sqrt{2})^4}{4a} = -\frac{4}{4a} = -\frac{1}{a}$.

**Problem (NEET/JEE Speed Method)**: Differentiate $y = \sin^{-1}(\frac{2x}{1+x^2})$.
**Solution**:
Instead of complex chain rule, substitute $x = \tan\theta$.
$y = \sin^{-1}(\frac{2\tan\theta}{1+\tan^2\theta}) = \sin^{-1}(\sin 2\theta) = 2\theta$.
Since $\theta = \tan^{-1}x$, $y = 2\tan^{-1}x$.
Therefore, $\frac{dy}{dx} = \frac{2}{1+x^2}$.
Speed tip: Memorize the inverse trig substitution identities. They turn massive chain-rule headaches into 2-second problems.
