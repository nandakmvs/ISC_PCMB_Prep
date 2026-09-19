# Chapter 12: Linear Programming

## 1. Exhaustive Theory & Precise ISC Terminology

**Linear Programming (LP)** deals with the optimization (maximization or minimization) of a linear function subject to a set of linear inequalities or equations.
- **Objective Function**: The linear function $Z = ax + by$ which has to be maximized or minimized.
- **Constraints**: The linear inequalities or equations or restrictions on the variables. $x \ge 0, y \ge 0$ are **non-negative constraints**.
- **Feasible Region**: The common region determined by all the constraints including non-negative constraints. Every point in this region is a **feasible solution**.
- **Infeasible Region / Solution**: Points outside the feasible region.
- **Optimal (Feasible) Solution**: Any point in the feasible region that gives the optimal value (maximum or minimum) of the objective function.

### Types of LP Problems
1. **Diet Problems**: Determine the amount of different foods to be consumed to meet nutrient requirements at minimum cost.
2. **Manufacturing Problems**: Determine the number of units of different products to produce to maximize profit subject to constraints like labor hours, machine hours, raw materials.
3. **Transportation Problems**: Determine a transportation schedule to minimize the total cost of transporting a commodity from various sources to various destinations.

## 2. Step-by-Step Derivations & Mechanisms

**Mechanism: The Corner Point Method**
1. **Formulate**: Write down the mathematical formulation (Objective function $Z$ and all inequality constraints).
2. **Graph**: Plot the constraint lines on a graph. Convert inequalities to equations to draw the lines.
3. **Shade**: Identify the feasible region by checking the inequalities (usually by testing the origin $(0,0)$).
4. **Find Corners**: Determine the coordinates of all the corner points (vertices) of the feasible region. Solve equations of intersecting lines simultaneously if not obvious from the graph.
5. **Evaluate**: Evaluate the objective function $Z = ax + by$ at each corner point.
6. **Conclude**:
   - If the region is **bounded**, the max/min values of Z evaluated at corners are the absolute max/min.
   - If the region is **unbounded** and we seek a max value $M$, check if the half-plane $ax+by > M$ has points in common with the feasible region. If no, $M$ is the max. If yes, no max exists. (Similar for minimum).

## 3. Diagram Blueprints & Labeling Checklists

- **Graphing Blueprint**:
  - Draw X and Y axes (Quadrant I is most important due to $x, y \ge 0$).
  - Draw solid lines for $\le$ or $\ge$.
  - Use arrows on lines pointing towards the valid region.
  - Shade the intersection area (Feasible Region).
  - Clearly label all corner points with coordinates $A(x_1, y_1), B(x_2, y_2)$ etc.

## 4. "Avoid the Trap" & Distinction Tables

| Trap / Common Mistake | Strategy / Fact to Remember |
| :--- | :--- |
| Forgetting non-negative constraints | Always state and graph $x \ge 0$ and $y \ge 0$. This restricts the feasible region exclusively to the first quadrant. |
| Misinterpreting "At least" vs "At most" | "At least" translates to $\ge$. "At most" translates to $\le$. Do not mix these up during formulation. |
| Not checking Unbounded regions | If the feasible region is open (unbounded), the extreme value found at a corner might not be the true maximum or minimum. You MUST perform the half-plane test. |

## 5. High-Yield Worked Model Problems

**Problem (ISC Step-by-Step)**: Solve the LP problem graphically. Maximize $Z = 4x + y$ subject to constraints: $x + y \le 50$, $3x + y \le 90$, $x \ge 0$, $y \ge 0$.
**Solution**:
1. **Graph the lines**: 
   Line 1: $x + y = 50$. Points: $(50, 0), (0, 50)$. Test $(0,0): 0 \le 50$ (True, shade towards origin).
   Line 2: $3x + y = 90$. Points: $(30, 0), (0, 90)$. Test $(0,0): 0 \le 90$ (True, shade towards origin).
2. **Find corner points of feasible region**: The region is bounded by the y-axis, x-axis, and the two lines.
   Corners:
   - Origin $O(0,0)$
   - Y-intercept of Line 1: $A(0, 50)$
   - X-intercept of Line 2: $B(30, 0)$
   - Intersection of Line 1 and 2: $C(x, y)$. Solve $x+y=50$ and $3x+y=90$. Subtraction gives $2x = 40 \implies x=20$. Thus $y=30$. Point $C(20, 30)$.
3. **Evaluate Z**:
   - At $O(0,0)$: $Z = 4(0) + 0 = 0$
   - At $A(0,50)$: $Z = 4(0) + 50 = 50$
   - At $B(30,0)$: $Z = 4(30) + 0 = 120$
   - At $C(20,30)$: $Z = 4(20) + 30 = 80 + 30 = 110$
4. **Conclusion**: The maximum value of Z is 120, which occurs at $(30, 0)$.

**Problem (NEET/JEE Concept)**: The corner points of the feasible region determined by linear constraints are $(0, 0), (0, 40), (20, 40), (60, 20), (60, 0)$. Let $Z = ax + by$ where $a, b > 0$. Find the condition on $a$ and $b$ such that the maximum of $Z$ occurs at both $(20, 40)$ and $(60, 20)$.
**Solution**:
If max occurs at two points, the value of Z must be equal at these points.
$Z$ at $(20, 40)$ = $20a + 40b$
$Z$ at $(60, 20)$ = $60a + 20b$
Equate them: $20a + 40b = 60a + 20b \implies 20b = 40a \implies b = 2a$.
(Any point on the line segment joining these two points will also yield the maximum value).
