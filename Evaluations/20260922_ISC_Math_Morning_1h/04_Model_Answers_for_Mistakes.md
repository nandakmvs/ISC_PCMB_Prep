# Model Answers for Missed Questions - Mathematics Test 03 (Morning)

**Q16 (Option B): Verify that $A^3 - 6A^2 + 9A - 4I = 0$. Hence, find $A^{-1}$.**

**Perfect ISC Answer (for the "Hence" part):**
*Note: When a question says "Hence", you are strictly forbidden from using the $adj(A) / |A|$ method. You must use algebraic manipulation of the verified equation.*

We have proved:
$A^3 - 6A^2 + 9A - 4I = 0$

Multiply the entire equation by $A^{-1}$:
$A^{-1}(A^3 - 6A^2 + 9A - 4I) = A^{-1}(0)$
$A^2 - 6A + 9I - 4A^{-1} = 0$

Rearrange to solve for $A^{-1}$:
$4A^{-1} = A^2 - 6A + 9I$
$A^{-1} = \frac{1}{4} (A^2 - 6A + 9I)$

Now, substitute the known matrices:
$A^{-1} = \frac{1}{4} \left( \begin{bmatrix} 6 & -5 & 5 \\ -5 & 6 & -5 \\ 5 & -5 & 6 \end{bmatrix} - \begin{bmatrix} 12 & -6 & 6 \\ -6 & 12 & -6 \\ 6 & -6 & 12 \end{bmatrix} + \begin{bmatrix} 9 & 0 & 0 \\ 0 & 9 & 0 \\ 0 & 0 & 9 \end{bmatrix} \right)$

$A^{-1} = \frac{1}{4} \begin{bmatrix} 6-12+9 & -5+6+0 & 5-6+0 \\ -5+6+0 & 6-12+9 & -5+6+0 \\ 5-6+0 & -5+6+0 & 6-12+9 \end{bmatrix}$

$A^{-1} = \frac{1}{4} \begin{bmatrix} 3 & 1 & -1 \\ 1 & 3 & 1 \\ -1 & 1 & 3 \end{bmatrix}$
