# Model Answers for Missed Questions - Math CBE Simulator 01

**Q2: The cost function is $C(x) = 3x^2 - 5x + 10$. The marginal cost when $x = 10$ is:**
**Model Answer:** 
Marginal cost is the rate of change of total cost with respect to output, i.e., the derivative $C'(x)$.
$C'(x) = \frac{d}{dx}(3x^2 - 5x + 10) = 6x - 5$.
At $x = 10$, Marginal Cost = $6(10) - 5 = 60 - 5 = 55$.
*(You had this initially, but crossed it out to evaluate $C(10)$ instead!)*

**Q35: Find its inverse $f^{-1}(x)$.**
**Model Answer:** 
After proving it is a bijection and finding $x = \frac{5y-3}{4}$, you must conclude by explicitly writing the inverse function in terms of $x$:
$\therefore f^{-1}(x) = \frac{5x - 3}{4}$

**Q36: Solve the following LPP graphically.**
**Model Answer:**
*(Algebraic corner point calculation is not enough. You must sketch the Cartesian plane, plot the lines $x+y=2$ and $x+3y=3$, shade the unbounded region above the lines in the first quadrant, and visually identify the corner points (0,2), (3/2, 1/2), and (3,0) from the graph before testing them in the objective function).*

**Q37: Using vector methods, prove that the angle subtended in a semicircle is a right angle.**
**Model Answer:**
1. Let the center of the semicircle be the origin $O(0,0)$.
2. Let the diameter lie along the x-axis, with endpoints $A$ and $B$. Let the position vector of $A$ be $\vec{a}$. Since $B$ is opposite to $A$ on the diameter, its position vector is $-\vec{a}$.
3. Let $P$ be any point on the semicircle with position vector $\vec{p}$.
4. Since $A, B,$ and $P$ lie on a circle centered at the origin, their magnitudes (radii) are equal: $|\vec{a}| = |-\vec{a}| = |\vec{p}| = r$.
5. The vector forming side $AP$ is $\vec{AP} = \vec{p} - \vec{a}$.
6. The vector forming side $BP$ is $\vec{BP} = \vec{p} - (-\vec{a}) = \vec{p} + \vec{a}$.
7. To prove the angle at $P$ is a right angle, we must prove the dot product of $\vec{AP}$ and $\vec{BP}$ is zero.
   $\vec{AP} \cdot \vec{BP} = (\vec{p} - \vec{a}) \cdot (\vec{p} + \vec{a})$
   $= |\vec{p}|^2 - |\vec{a}|^2$
   Since $|\vec{p}| = |\vec{a}| = r$, this becomes $r^2 - r^2 = 0$.
8. Since the dot product is zero, the vectors are perpendicular. Hence, the angle subtended in a semicircle is a right angle.
