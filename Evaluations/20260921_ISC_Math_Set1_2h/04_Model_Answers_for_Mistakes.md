# Model Answers for Missed Questions - Mathematics Test 02

**Q1: If A is a square matrix of order $3 \times 3$ such that $|A| = 4$, find the value of $|adj A|$.**
**Perfect ISC Answer:** 
Using the property: $|adj A| = |A|^{n-1}$ where $n$ is the order of the matrix.
Here, $n = 3$ and $|A| = 4$.
$|adj A| = (4)^{3-1} = 4^2 = \mathbf{16}$.

**Q12: Without expanding, prove that the determinant of a skew-symmetric matrix of odd order is always zero.**
**Perfect ISC Answer:**
Let $A$ be a skew-symmetric matrix of odd order $n$. By definition, $A^T = -A$.
Taking the determinant on both sides:
$|A^T| = |-A|$
By property of determinants, $|kA| = k^n|A|$. Therefore, $|-A| = (-1)^n|A|$.
Since $n$ is odd, $(-1)^n = -1$.
Also, $|A^T| = |A|$.
Substituting these into the equation gives:
$|A| = -|A|$
$2|A| = 0 \Rightarrow \mathbf{|A| = 0}$.

**Q14: Check whether the relation $R = \{(a,b) : a \le b^3\}$ is transitive.**
**Perfect ISC Answer:**
To prove a relation is NOT transitive, we must find a **counter-example** where $(a,b) \in R$ and $(b,c) \in R$, but $(a,c) \notin R$.
Let $a = 25, b = 3, c = 2$.
Check $(a,b)$: $25 \le 3^3 \Rightarrow 25 \le 27$ (True, so $(25,3) \in R$).
Check $(b,c)$: $3 \le 2^3 \Rightarrow 3 \le 8$ (True, so $(3,2) \in R$).
Check $(a,c)$: Is $25 \le 2^3$? No, $25 \not\le 8$ (False, so $(25,2) \notin R$).
Therefore, the relation is **not transitive**.
*(Note: You cannot prove transitivity by picking a single numerical example that works. You must use algebra for a general proof, or a numerical counter-example to disprove).*

**Q16: A die is thrown twice and the sum is 6. What is the conditional probability that 4 has appeared at least once?**
**Perfect ISC Answer:**
Let Event A = sum is 6 = $\{(1,5), (2,4), (3,3), (4,2), (5,1)\}$. So, $n(A) = 5$.
Let Event B = 4 appears at least once = $\{(4,1), (4,2), \dots (1,4), (2,4) \dots\}$.
$A \cap B = \{(2,4), (4,2)\}$. So, $n(A \cap B) = 2$.
We need the probability of B *given* A has occurred: $P(B|A)$.
$P(B|A) = \frac{n(A \cap B)}{n(A)} = \mathbf{\frac{2}{5}}$.
*(Note: Be extremely careful with notation. Writing $P(A|B)$ here is mathematically incorrect).*

**Q19: Discuss the continuity of the function at $x = 0$.**
**Perfect ISC Answer:**
*Presentation fix:* When evaluating left and right hand limits, you MUST use the correct directional notation.
Left Hand Limit (LHL): $\lim_{x \to 0^-} \frac{\sin 3x}{x} = \lim_{x \to 0^-} 3\left(\frac{\sin 3x}{3x}\right) = 3(1) = 3$.
Right Hand Limit (RHL): $\lim_{x \to 0^+} \frac{e^{3x}-1}{x} = \lim_{x \to 0^+} 3\left(\frac{e^{3x}-1}{3x}\right) = 3(1) = 3$.

**Q20: Find the intervals in which $f(x) = \sin x + \cos x, x \in [0, 2\pi]$ is strictly increasing or strictly decreasing.**
**Perfect ISC Answer:**
1. Find derivative: $f'(x) = \cos x - \sin x$.
2. Find critical points by setting $f'(x) = 0$: 
   $\cos x - \sin x = 0 \Rightarrow \tan x = 1 \Rightarrow x = \pi/4, 5\pi/4$.
3. Test intervals:
   - $[0, \pi/4)$: $f'(x) > 0$ (Strictly increasing)
   - $(\pi/4, 5\pi/4)$: $f'(x) < 0$ (Strictly decreasing)
   - $(5\pi/4, 2\pi]$: $f'(x) > 0$ (Strictly increasing)
*(Note: Never abandon a calculus question! Finding $f'(x)=0$ automatically secures step marks).*

**Q23: If $y = (\sin^{-1} x)^2$, prove $(1-x^2)y'' - xy' - 2 = 0$.**
**Perfect ISC Answer:**
1. First derivative: $y' = 2\sin^{-1}x \cdot \frac{1}{\sqrt{1-x^2}}$.
2. Rearrange and square: $\sqrt{1-x^2} y' = 2\sin^{-1}x \Rightarrow (1-x^2)(y')^2 = 4(\sin^{-1}x)^2 = 4y$.
3. **DO NOT STOP HERE!** Take the second derivative implicitly with respect to x using the product rule:
   $(1-x^2) \cdot 2y' \cdot y'' + (y')^2 \cdot (-2x) = 4y'$
4. Divide the entire equation by $2y'$:
   $(1-x^2)y'' - xy' = 2 \Rightarrow \mathbf{(1-x^2)y'' - xy' - 2 = 0}$. (Hence Proved).

**Q26: Equivalence relation modulus proof.**
**Perfect ISC Answer:**
*Presentation fix for Transitivity:*
If $(a,b) \in R \Rightarrow |a-b| = 4m \Rightarrow a-b = \pm 4m$.
If $(b,c) \in R \Rightarrow |b-c| = 4n \Rightarrow b-c = \pm 4n$.
Adding the two equations: $(a-b) + (b-c) = \pm 4m \pm 4n$.
$a-c = 4(\pm m \pm n) = 4k$ (where $k$ is an integer).
Therefore, $|a-c|$ is a multiple of 4, so $(a,c) \in R$. Transitive.
