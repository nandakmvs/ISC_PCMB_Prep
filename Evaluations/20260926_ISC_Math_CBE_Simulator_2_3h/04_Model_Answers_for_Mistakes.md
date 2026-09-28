# Model Answers for Missed Questions - Math CBE Simulator 02

**Q14: If $x = a\cos t$ and $y = a\sin t$, then $\frac{dy}{dx}$ is:**
**Model Answer:**
$\frac{dx}{dt} = -a\sin t$
$\frac{dy}{dt} = a\cos t$
$\frac{dy}{dx} = \frac{dy/dt}{dx/dt} = \frac{a\cos t}{-a\sin t} = -\cot t$. 
*(You selected $-\tan t$. Be careful with your trigonometric derivatives!)*

**Q26: Differentiate $y = \sin(x^x)$ with respect to $x$.**
**Model Answer:**
Use the chain rule. $\frac{dy}{dx} = \cos(x^x) \cdot \frac{d}{dx}(x^x)$.
To find the derivative of $x^x$, let $u = x^x$. Take log on both sides: $\ln u = x \ln x$.
Differentiate implicitly: $\frac{1}{u}\frac{du}{dx} = 1 \cdot \ln x + x \cdot \frac{1}{x} = \ln x + 1$.
$\frac{du}{dx} = x^x(\ln x + 1)$.
Substitute back: $\frac{dy}{dx} = \cos(x^x) \cdot x^x(\ln x + 1)$.

**Q27: Using vector methods, prove that the diagonals of a rhombus bisect each other at right angles.**
**Model Answer:**
1. Let the rhombus be $ABCD$ with adjacent sides represented by vectors $\vec{a} = \vec{AB}$ and $\vec{b} = \vec{AD}$.
2. Since it is a rhombus, all sides have equal magnitude: $|\vec{a}| = |\vec{b}|$.
3. The diagonal $\vec{AC} = \vec{a} + \vec{b}$ (by triangle law).
4. The diagonal $\vec{BD} = \vec{b} - \vec{a}$.
5. To prove they intersect at right angles, their dot product must be zero:
   $\vec{AC} \cdot \vec{BD} = (\vec{a} + \vec{b}) \cdot (\vec{b} - \vec{a})$
   $= |\vec{b}|^2 - |\vec{a}|^2$
6. Since $|\vec{a}| = |\vec{b}|$, the dot product is $0$. Hence proved.

**Q32: A spherical balloon is being inflated such that its volume is increasing at $25 \text{ cm}^3/\text{sec}$. Find the rate of change of surface area when radius is $5 \text{ cm}$.**
**Model Answer:**
Given: $\frac{dV}{dt} = 25$.
Volume $V = \frac{4}{3}\pi r^3 \implies \frac{dV}{dt} = 4\pi r^2 \frac{dr}{dt} \implies 25 = 4\pi (5)^2 \frac{dr}{dt} \implies 25 = 100\pi \frac{dr}{dt} \implies \frac{dr}{dt} = \frac{1}{4\pi}$.
Surface Area $S = 4\pi r^2 \implies \frac{dS}{dt} = 8\pi r \frac{dr}{dt}$.
Substitute values: $\frac{dS}{dt} = 8\pi (5) (\frac{1}{4\pi}) = 40\pi (\frac{1}{4\pi}) = 10 \text{ cm}^2/\text{sec}$.

**Q33: Find the local maximum and minimum values of $f(x) = 2x^3 - 6x^2 + 6x + 5$.**
**Model Answer:**
1. $f'(x) = 6x^2 - 12x + 6 = 6(x^2 - 2x + 1) = 6(x-1)^2$.
2. Set $f'(x) = 0 \implies x = 1$.
3. Check the sign of $f'(x)$ around $x=1$. Since $6(x-1)^2$ is always positive for $x \neq 1$, $f'(x)$ does not change sign as $x$ passes through 1.
4. Therefore, $x=1$ is a point of inflection. There are no local maximum or minimum values.

**Q37: Verify Rolle's Theorem for $f(x) = x^2 - 4x + 3$ on $[1, 3]$.**
**Model Answer:**
1. $f(x)$ is a polynomial, hence continuous on $[1,3]$.
2. $f'(x) = 2x - 4$, which exists for all $x \in (1,3)$, hence differentiable.
3. Check endpoints: $f(1) = 1 - 4 + 3 = 0$. $f(3) = 9 - 12 + 3 = 0$. Since $f(1) = f(3)$, all three conditions of Rolle's theorem are satisfied.
4. There must exist some $c \in (1,3)$ such that $f'(c) = 0$.
   $2c - 4 = 0 \implies 2c = 4 \implies c = 2$.
   Since $2 \in (1,3)$, Rolle's Theorem is verified.
