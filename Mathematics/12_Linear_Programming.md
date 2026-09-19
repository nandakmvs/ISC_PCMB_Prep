# Chapter 12: Linear Programming

## Part 1: Exhaustive Theory & Precise ISC Terminology

Linear Programming (LP) is an optimization technique used to find the maximum or minimum value of a linear objective function subject to a set of linear constraints (equations or inequalities). In the context of ISC Class 12, the focus is exclusively on two-variable linear programming problems solvable via the graphical method.

### 1.1 Core Components of a Linear Programming Problem (LPP)

Every LPP fundamentally consists of three components:

1.  **Decision Variables**: These are the unknowns that need to be determined to optimize the outcome. Usually denoted as **$x$** and **$y$**. In formulation, they represent quantities (e.g., number of units produced, amount of ingredient used).
2.  **Objective Function**: This is the linear mathematical function of the decision variables that must be maximized or minimized. It is universally denoted by **$Z$**.
    *   *Form*: **$Z = ax + by$**, where '$a$' and '$b$' are constants representing costs, profits, weights, etc.
    *   *Types*: **Maximization** (e.g., maximizing profit, yield, or returns) or **Minimization** (e.g., minimizing cost, distance, or time).
3.  **Constraints**: These are the restrictions or limitations on the availability of resources (time, materials, capital, etc.) expressed as linear inequalities or equations in terms of the decision variables.
    *   *Structural Constraints*: Limitations on resources (e.g., $2x + 3y \le 120$).
    *   **Non-negativity Constraints**: The most critical and universal constraints, asserting that physical quantities cannot be negative. **$x \ge 0, y \ge 0$**.

### 1.2 Precise ISC Terminology (Keyword Mastery)

To secure full marks in the ISC Board examinations, the usage of specific terminology is non-negotiable. 

*   **Optimization Problem**: A problem that seeks to maximize or minimize a linear function subject to certain constraints as determined by a set of linear inequalities.
*   **Feasible Region**: The common region determined by all the constraints including non-negative constraints $x, y \ge 0$ of a linear programming problem. Every point in this region satisfies all the constraints simultaneously.
*   **Feasible Solution**: Any point $(x, y)$ that lies inside or on the boundary of the **Feasible Region**.
*   **Infeasible Solution**: Any point $(x, y)$ that lies *outside* the feasible region.
*   **Optimal Feasible Solution**: A feasible solution at which the objective function attains its maximum or minimum value.
*   **Corner Point (Vertex)**: A point in the feasible region that is the intersection of two boundary lines. The optimal solution, if it exists, *always* occurs at one of the corner points of the feasible region.
*   **Bounded Region**: A feasible region that can be enclosed within a circle. It has a finite perimeter and area. A bounded region *guarantees* both a maximum and a minimum value for the objective function.
*   **Unbounded Region**: A feasible region that extends indefinitely in at least one direction. It does not have a finite boundary. Optimization in unbounded regions requires the use of a secondary half-plane check.
*   **Redundant Constraint**: A constraint whose removal does not alter the shape or boundaries of the feasible region. (It provides a restriction that is already strictly satisfied by other constraints).

### 1.3 Types of Linear Programming Problems

1.  **Manufacturing Problems**: Determine the number of units of different products to be manufactured to maximize profit, subject to constraints on machine hours, labor hours, or raw materials.
2.  **Diet Problems**: Determine the amount of different types of food items to be consumed to satisfy minimal nutritional requirements at the minimum cost. (Usually, Minimization LPP).
3.  **Transportation Problems**: Minimize the cost of transporting commodities from sources to destinations. (While complex transportation models exist, ISC focuses on simplified 2-variable versions).
4.  **Investment/Allocation Problems**: Allocate a fixed capital across different investment avenues to maximize overall return.

## Part 2: Step-by-Step Derivations & Mechanisms

LPP in ISC requires a rigid, stepwise algorithmic execution. Skipping steps or doing mental math leads to heavy penalization.

### 2.1 Algorithm 1: Mathematical Formulation of an LPP

Often, the problem is presented as a word problem. You must construct the algebraic model before solving it.

*   **Step 1: Identify the Decision Variables.** Read the last sentence of the problem carefully. What is it asking you to find? Assign these as $x$ and $y$.
    *   *ISC Presentation*: Write "Let the number of units of product A be $x$ and product B be $y$."
*   **Step 2: Identify the Objective.** Are you trying to maximize profit/yield or minimize cost/time? Formulate the objective function $Z$ in terms of $x$ and $y$.
    *   *ISC Presentation*: Write "Maximize $Z = 50x + 60y$" (for example).
*   **Step 3: Identify the Constraints.** Break down the problem statement into distinct resource limitations.
    *   "At most", "Maximum available", "Cannot exceed" translates to **$\le$** (Less than or equal to).
    *   "At least", "Minimum requirement", "Must be more than" translates to **$\ge$** (Greater than or equal to).
    *   *ISC Presentation*: Formulate a table for clarity (optional but highly recommended for accuracy), then write the constraints. "Subject to the constraints: $2x + y \le 10$, $x + 3y \le 15$".
*   **Step 4: Non-Negativity Constraints.** Never forget this. It is a guaranteed 1/2 to 1 mark deduction if missing.
    *   *ISC Presentation*: Write "$x \ge 0, y \ge 0$".

### 2.2 Algorithm 2: The Corner Point Method (Graphical Solution)

This is the standard ISC procedure for solving the formed LPP.

*   **Step 1: Convert inequalities to equations.**
    *   Let the constraints $ax + by \le c$ be written as $ax + by = c$.
*   **Step 2: Find the intercepts.** Find the x and y intercepts for each line to plot them easily.
    *   Put $x = 0$ to find the y-intercept.
    *   Put $y = 0$ to find the x-intercept.
    *   *ISC Presentation*: Create a small 2x2 table for *each* equation showing $(0, y_1)$ and $(x_1, 0)$.
*   **Step 3: Plot the lines on a Cartesian plane.**
    *   Use graph paper if provided, or draw a neat scale diagram. Mark the equations ON the respective lines.
*   **Step 4: Determine the feasible region (Shading).**
    *   Use the **Origin Test**. Substitute $(0,0)$ into the original inequality.
    *   If $(0,0)$ satisfies the inequality (e.g., $0 \le 10$ is True), the region contains the origin. Shade *towards* the origin.
    *   If $(0,0)$ does not satisfy it (e.g., $0 \ge 10$ is False), shade *away* from the origin.
    *   If the line passes through the origin, use another test point like $(1,0)$ or $(0,1)$.
    *   *Critical*: The region bounded by $x \ge 0$ and $y \ge 0$ restricts the feasible region strictly to the **First Quadrant**.
    *   Find the intersection of all shaded regions. Mark it prominently as the **Feasible Region**.
*   **Step 5: Identify the Corner Points (Vertices).**
    *   Locate the vertices of the shaded feasible region.
    *   For vertices formed by the intersection of two constraint lines, solve their equations simultaneously. Do *not* rely on visual estimation from the graph. Show the simultaneous solution algebra.
*   **Step 6: Evaluate Objective Function at Corner Points.**
    *   Create a table with columns: "Corner Point $(x,y)$" and "Value of $Z = ax + by$".
    *   Calculate $Z$ for each vertex.
*   **Step 7: Determine the Optimal Solution.**
    *   **If the region is Bounded**: The highest value of $Z$ is the Maximum, and the lowest is the Minimum.
    *   **If the region is Unbounded**: Let $M$ be the maximum value obtained.
        *   Draw a dashed (dotted) line for the open half-plane **$ax + by > M$**.
        *   If this open half-plane has *no point in common* with the feasible region, then $M$ is the maximum.
        *   If it *shares a point* with the feasible region, there is *no maximum value*.
        *   (Similarly, for minimum $m$, test the open half-plane $ax + by < m$).

## Part 3: Diagram Blueprints & Labeling Checklists

The graph is the heart of the LPP solution. ISC examiners have a strict rubric for evaluating LPP graphs. A technically correct mathematical answer will lose substantial marks if the graph is improperly formatted.

### 3.1 The Perfect ISC LPP Graph Checklist

Before moving to the calculation table, ensure your graph meets all these criteria:

- [ ] **Axes Labeling**: The X-axis and Y-axis are clearly marked with proper arrows indicating direction. The origin is marked as $O(0,0)$.
- [ ] **Scale Declaration**: A clear scale is written in the top right corner (e.g., *Scale: X-axis: 1 cm = 10 units; Y-axis: 1 cm = 10 units*).
- [ ] **Line Equations**: Every plotted line MUST have its corresponding equation (e.g., $2x + 3y = 12$) written alongside it. Do not write the inequality ($<, >$) on the line, write the equation ($=$).
- [ ] **Directional Arrows for Half-Planes**: Instead of messy, chaotic shading over the whole graph, draw small perpendicular arrows on the line indicating which side the inequality points to.
- [ ] **Feasible Region Shading**: Once the common region is found (almost always in the 1st quadrant due to $x, y \ge 0$), shade it neatly using diagonal pencil lines or a light highlighter. Do not over-shade.
- [ ] **Vertex Marking**: Every corner point of the feasible region must be named with a capital letter (e.g., A, B, C, D) AND its coordinates explicitly written next to it: $A(0, 10)$, $B(5, 5)$.
- [ ] **First Quadrant Boundary**: The shading MUST NOT cross the X and Y axes downwards or leftwards. It must strictly adhere to the $x \ge 0, y \ge 0$ boundary.

### 3.2 Diagrammatic Variations (The Blueprint)

Visualizing the type of LPP based on the constraint slopes helps in anticipating the feasible region.

1.  **The "Inward" Polygon (Standard Maximization)**
    *   Constraints generally of type $\le$.
    *   Feasible region is bounded, pinned to the origin (0,0).
    *   Maximum usually occurs at the outermost vertex.
2.  **The "Outward" Open Region (Standard Minimization)**
    *   Constraints generally of type $\ge$.
    *   Feasible region is unbounded, moving infinitely outward into the 1st quadrant.
    *   Minimum occurs at the vertices closest to the origin. Requires the $Z < m$ half-plane check.
3.  **The "Corridor" (Mixed Constraints)**
    *   A mix of $\le$ and $\ge$ constraints.
    *   The feasible region is bounded but does *not* touch the origin. It forms a polygon floating in the 1st quadrant.
4.  **No Feasible Region (Infeasible)**
    *   Constraints are contradictory (e.g., $x + y \le 2$ and $x + y \ge 5$).
    *   The directional arrows point away from each other, leaving no common overlapping area in the 1st quadrant.
    *   *Result*: No solution exists.

### 3.3 The "Open Half-Plane" Plot (For Unbounded Regions)

When the feasible region is unbounded and you need to verify if $Z_{max} = M$ or $Z_{min} = m$:
1.  Form the inequality: $ax + by > M$ (for max) or $ax + by < m$ (for min).
2.  Plot the line $ax + by = M$ (or $m$).
3.  **CRITICAL**: This line must be plotted as a **DASHED or DOTTED line** (`- - - -`). A solid line implies the boundary is included, which is false for strict inequalities ($>, <$).
4.  If the dashed line passes through the interior of your shaded feasible region, write: *"Since the open half-plane has points in common with the feasible region, no maximum/minimum exists."*
5.  If it only touches the vertex or stays completely outside, write: *"Since the open half-plane has no points in common with the feasible region, the max/min value is valid."*

## Part 4: "Avoid the Trap" & Distinction Tables

LPP might seem straightforward, but it is heavily trapped with nuances that cost students the perfect 100.

### 4.1 Objective (JEE/NEET) vs Subjective (ISC) Traps

| Feature | Objective Trap (JEE/NDA) | Subjective Trap (ISC) | The Fix |
| :--- | :--- | :--- | :--- |
| **Finding Intersections** | Estimating from the graph to save time. | Deducting marks for lack of algebraic proof. | Always solve the two intersecting line equations simultaneously on paper. |
| **Non-negativity** | Assumed implicitly. | -1 Mark if $x \ge 0, y \ge 0$ is not explicitly written in formulation. | Memorize it as the final step of *every* formulation. |
| **Unbounded Regions** | Often directly asking if unbounded. | Assuming the lowest calculated value is the absolute minimum without the half-plane test. | Always execute the $Z < m$ or $Z > M$ dashed-line test for unbounded regions. |
| **Line types** | Rough sketches suffice. | Drawing solid lines for open half-plane tests. | Use strict dashed lines for inequalities lacking "$=$". |
| **Multiple Optima** | Identifying "infinite solutions". | Failing to state that the optimal value lies on the entire line segment joining two vertices. | If two vertices give the same optimal $Z$, state: "Max/Min occurs at all points on the line segment joining A and B." |

### 4.2 Concept Distinction Tables

**Bounded vs. Unbounded Region**

| Feature | Bounded Region | Unbounded Region |
| :--- | :--- | :--- |
| **Shape** | Closed polygon (can be enclosed in a circle). | Open on one or more sides (extends to infinity). |
| **Max/Min Existence** | Both maximum and minimum values are guaranteed to exist at corner points. | Max/Min *might* not exist. Requires secondary verification. |
| **Verification Tool** | Corner Point Method is sufficient. | Corner Point Method + Open Half-Plane Test. |

**Infeasible vs. Unbounded Solution**

| Concept | Meaning | Graph Appearance |
| :--- | :--- | :--- |
| **Infeasible Region** | No single point satisfies all constraints simultaneously. | No common shaded area. |
| **Unbounded Solution** | The objective function can be increased/decreased infinitely without violating constraints. | Feasible region extends infinitely in the direction of optimization. |

### 4.3 Common Phrasing Translations (The "English to Math" Trap)

Students often misinterpret word problems. Memorize these direct translations:

*   *"At least 50 units"* $\rightarrow \ge 50$
*   *"Not more than 200 units"* $\rightarrow \le 200$
*   *"Exactly 30 units"* $\rightarrow = 30$ (Rare in LPP, but reduces the dimension).
*   *"Demand for A is at most twice the demand for B"* $\rightarrow x \le 2y$ (Trap: Writing $2x \le y$).
*   *"Availability is restricted to 500"* $\rightarrow \le 500$
*   *"Minimum requirement is 100"* $\rightarrow \ge 100$

## Part 5: High-Yield Worked Model Problems

### Problem Type 1: The Standard Manufacturing Problem (Maximization, Bounded)

**Question:** A furniture dealer deals in only two items—tables and chairs. He has ₹50,000 to invest and has storage space of at most 60 pieces. A table costs ₹2500 and a chair ₹500. He estimates that from the sale of one table, he can make a profit of ₹250 and that from the sale of one chair a profit of ₹75. He wants to know how many tables and chairs he should buy from the available money so as to maximize his total profit, assuming that he can sell all the items which he buys. Formulate as LPP and solve.

**Step-by-Step ISC Solution:**

**1. Formulation:**
*   Let the number of tables bought be $x$ and chairs be $y$.
*   Objective Function: Maximize Profit $Z = 250x + 75y$
*   Subject to constraints:
    *   Investment constraint: $2500x + 500y \le 50000 \implies 5x + y \le 100$
    *   Storage constraint: $x + y \le 60$
    *   Non-negativity: $x \ge 0, y \ge 0$

**2. Graphing Constraints (Equations):**
*   Line 1: $5x + y = 100$
    *   If $x=0, y=100 \rightarrow (0, 100)$
    *   If $y=0, x=20 \rightarrow (20, 0)$
    *   Origin test $(0,0)$: $0 \le 100$ (True, shade towards origin)
*   Line 2: $x + y = 60$
    *   If $x=0, y=60 \rightarrow (0, 60)$
    *   If $y=0, x=60 \rightarrow (60, 0)$
    *   Origin test $(0,0)$: $0 \le 60$ (True, shade towards origin)

**3. Finding Vertices of Feasible Region:**
*   The feasible region is bounded by coordinates (0,0), (20,0), intersection of lines, and (0,60).
*   Solving $5x + y = 100$ and $x + y = 60$:
    *   Subtracting: $4x = 40 \implies x = 10$
    *   Substitute $x=10$ in $x+y=60 \implies 10 + y = 60 \implies y = 50$.
    *   Intersection Vertex: $B(10, 50)$

**4. Evaluation Table:**
Vertices of feasible region: $O(0,0), A(20,0), B(10,50), C(0,60)$

| Corner Point $(x, y)$ | Value of $Z = 250x + 75y$ |
| :--- | :--- |
| $O(0, 0)$ | $250(0) + 75(0) = 0$ |
| $A(20, 0)$ | $250(20) + 75(0) = 5000$ |
| $B(10, 50)$ | $250(10) + 75(50) = 2500 + 3750 = 6250$ | **(Maximum)** |
| $C(0, 60)$ | $250(0) + 75(60) = 4500$ |

**5. Final Conclusion:**
The maximum profit is ₹6250 when he buys 10 tables and 50 chairs.

---

### Problem Type 2: Diet Problem (Minimization, Unbounded Region)

**Question:** A diet is to contain at least 80 units of vitamin A and 100 units of minerals. Two foods $F_1$ and $F_2$ are available. Food $F_1$ costs ₹4 per unit and $F_2$ costs ₹6 per unit. One unit of $F_1$ contains 3 units of vitamin A and 4 units of minerals. One unit of $F_2$ contains 6 units of vitamin A and 3 units of minerals. Formulate LPP to find minimum cost.

**1. Formulation:**
*   Let units of $F_1$ be $x$ and $F_2$ be $y$.
*   Objective: Minimize Cost $Z = 4x + 6y$
*   Constraints:
    *   Vitamin A: $3x + 6y \ge 80$
    *   Minerals: $4x + 3y \ge 100$
    *   $x \ge 0, y \ge 0$

**2. Graphing & Vertices:**
*   $3x + 6y = 80 \implies (0, 13.3), (26.6, 0)$. Test $(0,0) \ge 80$ (False, shade outward).
*   $4x + 3y = 100 \implies (0, 33.3), (25, 0)$. Test $(0,0) \ge 100$ (False, shade outward).
*   Intersection: $3x + 6y = 80$ and $8x + 6y = 200 \implies 5x = 120 \implies x = 24$.
    *   $3(24) + 6y = 80 \implies 72 + 6y = 80 \implies 6y = 8 \implies y = 4/3$. Intersection $B(24, 4/3)$.
*   Feasible region is UNBOUNDED. Vertices: $A(80/3, 0), B(24, 4/3), C(0, 100/3)$.

**3. Evaluation:**

| Corner Point | $Z = 4x + 6y$ |
| :--- | :--- |
| $A(80/3, 0)$ | $4(80/3) = 106.67$ |
| $B(24, 4/3)$ | $4(24) + 6(4/3) = 96 + 8 = 104$ | **(Minimum $m$)** |
| $C(0, 100/3)$| $6(100/3) = 200$ |

**4. Unbounded Region Test (Crucial Step):**
Since region is unbounded, we must check the half-plane $4x + 6y < 104 \implies 2x + 3y < 52$.
Plot the dashed line $2x + 3y = 52$.
This open half-plane has *no points in common* with the feasible region.
**Conclusion:** Therefore, the minimum cost is indeed ₹104 at 24 units of $F_1$ and $4/3$ units of $F_2$.

### JEE/NEET Speed Shortcut (Iso-Cost/Iso-Profit Method)

While ISC requires the corner-point evaluation table, objective exams demand speed.
1. Find the slope of the objective function line $Z = ax + by \implies \text{slope } m = -a/b$.
2. For Maximization: Imagine moving the objective function line parallel to itself away from the origin. The *last vertex* it touches before leaving the feasible region is the maximum.
3. For Minimization: Move the line towards the origin. The *first vertex* it touches in the feasible region is the minimum.
*Advantage:* Bypasses calculating $Z$ for every single vertex, saving critical minutes in MCQs.
