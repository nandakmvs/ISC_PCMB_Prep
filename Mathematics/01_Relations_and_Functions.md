# Module 01: Relations and Functions

## Part 1: Exhaustive Theory & Precise ISC Terminology

### 1.1 Fundamentals of Relations
A **Relation** $R$ from a non-empty set $A$ to a non-empty set $B$ is a subset of the Cartesian product $A \times B$. If $A=B$, we say $R$ is a relation on $A$.
*   **Domain**: The set of all first elements of the ordered pairs in $R$. $\text{Dom}(R) = \{a \in A : (a,b) \in R\}$.
*   **Range**: The set of all second elements of the ordered pairs in $R$. $\text{Range}(R) = \{b \in B : (a,b) \in R\}$.
*   **Codomain**: The entire set $B$. Note that $\text{Range} \subseteq \text{Codomain}$.

### 1.2 Types of Relations (ISC Core Focus)
*   **Empty Relation**: No element of $A$ is related to any element of $A$. $R = \emptyset \subseteq A \times A$.
*   **Universal Relation**: Each element of $A$ is related to every element of $A$. $R = A \times A$.
*   **Identity Relation ($I_A$)**: Every element of $A$ is related to itself **and only itself**. $I_A = \{(a,a) : a \in A\}$.
*   **Reflexive Relation**: A relation $R$ on set $A$ is reflexive if $(a,a) \in R$ for **every** $a \in A$. 
    *   *Note*: Identity relation is always reflexive, but a reflexive relation is not necessarily the identity relation.
*   **Symmetric Relation**: A relation $R$ on set $A$ is symmetric if $(a,b) \in R \implies (b,a) \in R$ for all $a, b \in A$.
*   **Transitive Relation**: A relation $R$ on set $A$ is transitive if $(a,b) \in R$ and $(b,c) \in R \implies (a,c) \in R$ for all $a, b, c \in A$.
    *   *ISC Trap*: If $(a,b) \in R$ but there is no $(b,c) \in R$ to pair it with, the relation is **vacuously transitive**.

### 1.3 Equivalence Relation & Equivalence Classes
*   **Equivalence Relation**: A relation $R$ is an equivalence relation if it is simultaneously **Reflexive, Symmetric, and Transitive**.
*   **Equivalence Class**: Let $R$ be an equivalence relation on a set $X$. The equivalence class of $a \in X$, denoted by $[a]$, is the set of all elements of $X$ related to $a$.
    $[a] = \{x \in X : (x,a) \in R\}$.
*   **Partition**: An equivalence relation partitions the set into pairwise disjoint subsets (equivalence classes) whose union is the whole set.

### 1.4 Functions and Their Types
A **Function** $f: A \to B$ is a relation where **every** element in the domain $A$ has a **unique** image in the codomain $B$.
*   **One-One (Injective) Function**: A function $f: A \to B$ is one-one if distinct elements of $A$ have distinct images in $B$.
    *   *Mathematical Definition*: $f(x_1) = f(x_2) \implies x_1 = x_2$ for all $x_1, x_2 \in A$.
*   **Many-One Function**: A function that is not one-one. At least two elements in $A$ map to the same element in $B$.
*   **Onto (Surjective) Function**: A function $f: A \to B$ is onto if every element in $B$ is the image of at least one element in $A$.
    *   *Key Condition*: $\text{Range of } f = \text{Codomain of } f = B$.
*   **Into Function**: A function that is not onto. There is at least one element in $B$ with no pre-image in $A$. ($\text{Range} \subset \text{Codomain}$).
*   **Bijective Function**: A function that is both **One-One (Injective)** and **Onto (Surjective)**.

### 1.5 Composition of Functions
Let $f: A \to B$ and $g: B \to C$ be two functions. The **composition** of $f$ and $g$, denoted by $g \circ f$, is a function defined as $(g \circ f)(x) = g(f(x))$ for all $x \in A$.
*   *Requirement*: The range of $f$ must be a subset of the domain of $g$.

### 1.6 Invertible Functions
A function $f: A \to B$ is invertible if there exists a function $g: B \to A$ such that $g \circ f = I_A$ (Identity function on $A$) and $f \circ g = I_B$ (Identity function on $B$).
*   *Theorem*: A function $f$ is invertible **if and only if** $f$ is a **bijective** function. The function $g$ is called the inverse of $f$ and is denoted by $f^{-1}$.

### 1.7 Binary Operations (Brief Reference)
A binary operation $*$ on a set $A$ is a function $* : A \times A \to A$. It denotes combining two elements of $A$ to produce another element of $A$. (Check current ISC syllabus for depth required; primarily associative and commutative properties).
## Part 2: Step-by-Step Derivations & Mechanisms

### 2.1 Mechanism: Proving an Equivalence Relation
**ISC Presentation Rule**: To score full marks in the subjective section, you must explicitly write down the theoretical conditions for Reflexivity, Symmetry, and Transitivity, state the generic elements, and conclude correctly.

**Example Task**: Prove that relation $R$ on $\mathbb{Z}$ defined by $R = \{(a,b) : 2 \text{ divides } (a-b)\}$ is an equivalence relation.

**Step 1: Reflexivity**
*   *Statement*: Let $a \in \mathbb{Z}$ be an arbitrary element.
*   *Logic*: $a - a = 0$. Since $0 = 2 \times 0$, $2$ divides $(a-a)$.
*   *Conclusion*: Therefore, $(a,a) \in R$ for all $a \in \mathbb{Z}$. Hence, $R$ is **reflexive**.

**Step 2: Symmetry**
*   *Statement*: Let $a, b \in \mathbb{Z}$ such that $(a,b) \in R$.
*   *Logic*: Since $(a,b) \in R$, $2$ divides $(a-b)$. Thus, $a-b = 2k$ for some integer $k$.
    This implies $-(a-b) = -2k \implies b-a = 2(-k)$. Since $-k$ is also an integer, $2$ divides $(b-a)$.
*   *Conclusion*: Therefore, $(b,a) \in R$. Hence, $R$ is **symmetric**.

**Step 3: Transitivity**
*   *Statement*: Let $a, b, c \in \mathbb{Z}$ such that $(a,b) \in R$ and $(b,c) \in R$.
*   *Logic*: $a-b = 2k_1$ and $b-c = 2k_2$ for some integers $k_1, k_2$.
    Adding the two equations: $(a-b) + (b-c) = 2k_1 + 2k_2 \implies a-c = 2(k_1+k_2)$.
    Since $(k_1+k_2)$ is an integer, $2$ divides $(a-c)$.
*   *Conclusion*: Therefore, $(a,c) \in R$. Hence, $R$ is **transitive**.

**Final Step**: Since $R$ is reflexive, symmetric, and transitive, it is an **equivalence relation**.

---

### 2.2 Mechanism: Proving Bijectivity (One-One and Onto)
**Example Task**: Prove that $f: \mathbb{R} \to \mathbb{R}$ given by $f(x) = 3x + 4$ is bijective.

**Step 1: Prove Injectivity (One-One)**
*   *Initialization*: Let $x_1, x_2$ be arbitrary elements in the domain ($\mathbb{R}$).
*   *Assumption*: Assume $f(x_1) = f(x_2)$.
*   *Execution*: $3x_1 + 4 = 3x_2 + 4 \implies 3x_1 = 3x_2 \implies x_1 = x_2$.
*   *Conclusion*: Since $f(x_1) = f(x_2) \implies x_1 = x_2$, the function $f$ is **one-one**.

**Step 2: Prove Surjectivity (Onto)**
*   *Initialization*: Let $y$ be an arbitrary element in the codomain ($\mathbb{R}$).
*   *Equation formulation*: Let $f(x) = y$. Thus, $3x + 4 = y$.
*   *Solve for x*: $x = \frac{y-4}{3}$.
*   *Verification*: For every $y \in \mathbb{R}$, $x = \frac{y-4}{3} \in \mathbb{R}$ (Domain). 
    Check: $f\left(\frac{y-4}{3}\right) = 3\left(\frac{y-4}{3}\right) + 4 = y - 4 + 4 = y$.
*   *Conclusion*: Since for every $y$ in the codomain there exists an $x$ in the domain such that $f(x) = y$, $f$ is **onto**.

**Final Step**: Since $f$ is both one-one and onto, $f$ is **bijective**.

---

### 2.3 Mechanism: Finding the Inverse of a Function
1.  Verify/State that $f$ is a bijection. (If the question says "Find the inverse", assume it's bijective, but mention it).
2.  Set $f(x) = y$.
3.  Algebraically isolate $x$ in terms of $y$. $x = g(y)$.
4.  Replace $x$ with $f^{-1}(y)$, giving $f^{-1}(y) = g(y)$.
5.  Swap variables (optional but conventional): $f^{-1}(x) = g(x)$.
## Part 3: Diagram Blueprints & Labeling Checklists

### 3.1 Arrow Diagram Blueprint for Relations
When asked to visualize or check if a relation is reflexive, symmetric, or transitive on a small finite set (e.g., $A = \{1, 2, 3\}$), use a directed graph / arrow diagram.
*   **Reflexive Rule**: Every node MUST have a self-loop (an arrow pointing to itself). Missing even one means it's not reflexive.
*   **Symmetric Rule**: Every arrow going from $x$ to $y$ MUST have a returning arrow from $y$ to $x$. Single-direction arrows break symmetry.
*   **Transitive Rule**: For every path of two arrows ($x \to y$ and $y \to z$), there MUST be a direct shortcut arrow ($x \to z$).

### 3.2 Mapping Diagrams for Functions
**Checklist for Function Validity**:
1.  **Every element in the Domain (Set A)** must have exactly one outgoing arrow. (No element left behind).
2.  **No element in the Domain** can have more than one outgoing arrow (No splitting).

**Identifying Function Types via Mapping**:
*   **One-One (Injective)**: No element in the Codomain (Set B) receives more than one incoming arrow.
*   **Many-One**: At least one element in the Codomain receives two or more incoming arrows.
*   **Onto (Surjective)**: EVERY element in the Codomain receives at least one incoming arrow (No element in B is left un-pointed to).
*   **Into**: At least one element in the Codomain has zero incoming arrows.
*   **Bijective**: Perfect one-to-one pairing. Every element in A points to exactly one distinct element in B, and no elements in B are left out.

### 3.3 Graphical Blueprint (JEE/NEET Speed Tool)
If the function is plotted on a 2D Cartesian plane:
*   **Vertical Line Test (Function Test)**: If any vertical line intersects the graph more than once, the relation is **NOT** a function.
*   **Horizontal Line Test (One-One Test)**: If any horizontal line intersects the graph more than once, the function is **Many-One**. If every horizontal line intersects at most once, it is **One-One**.
*   **Onto Test (Range Evaluation)**: Project the graph onto the y-axis. If the projection covers the entire given Codomain perfectly, it is **Onto**.

### 3.4 Important Standard Graphs to Memorize
*   **Modulus Function $f(x) = |x|$**: V-shape. Many-one (fails horizontal line test). Not onto $\mathbb{R}$ (range is $[0, \infty)$).
*   **Signum Function $f(x) = \text{sgn}(x)$**: Three flat segments. Many-one, Range = $\{-1, 0, 1\}$.
*   **Greatest Integer Function $f(x) = [x]$**: Step function. Many-one, Range = $\mathbb{Z}$.
## Part 4: "Avoid the Trap" & Distinction Tables

### 4.1 Objective (JEE) vs Subjective (ISC) Distinctions

| Feature | ISC Subjective Method | JEE Objective Speed Method |
| :--- | :--- | :--- |
| **Testing One-One** | Strictly use $f(x_1) = f(x_2) \implies x_1 = x_2$. | Use calculus: If $f'(x) > 0$ strictly or $f'(x) < 0$ strictly for all $x \in$ Domain, it's one-one. |
| **Testing Onto** | Set $y=f(x)$, find $x$ in terms of $y$, show $x \in$ Domain for all $y \in$ Codomain. | Find Max and Min values using limits or derivatives. If $[\text{Min}, \text{Max}] = \text{Codomain}$, it's onto. |
| **Equivalence Relation** | Write full descriptive statements with arbitrary elements $a,b,c$. | Quickly draw mental arrow diagrams or check counter-examples mentally. |

### 4.2 Concept Traps to Avoid
> [!WARNING] **TRAP 1: The Domain/Codomain Swap**
> A function's bijectivity depends ENTIRELY on its defined domain and codomain.
> *Example*: $f(x) = x^2$ is **not one-one** and **not onto** if $f: \mathbb{R} \to \mathbb{R}$.
> BUT, $f(x) = x^2$ is **bijective** if $f: [0, \infty) \to [0, \infty)$.
> *Always check the set definitions before concluding.*

> [!CAUTION] **TRAP 2: Vacuous Truth in Transitivity**
> In relations, if you have $(1,2) \in R$ but there is NO pair starting with $2$, you **cannot** say transitivity fails. Transitivity only fails if $(a,b)$ and $(b,c)$ exist, but $(a,c)$ is missing. If the "if" part is incomplete, the condition is *vacuously true*.
> *Example*: $R = \{(1,2)\}$ on set $\{1,2,3\}$ is **transitive**.

> [!IMPORTANT] **TRAP 3: $x^2 = y^2$ Implications**
> When doing $f(x_1) = f(x_2)$ for $f(x) = x^2$, remember that $x_1^2 = x_2^2 \implies x_1 = \pm x_2$.
> Because $x_1$ does not purely equal $x_2$, it is Many-One on $\mathbb{R}$. Do not blindly write $x_1 = x_2$.

### 4.3 Key Distinction Table
| Term | Meaning | Key Formula/Requirement |
| :--- | :--- | :--- |
| **Reflexive** | Every element relates to itself. | $(a,a) \in R \; \forall a \in A$ |
| **Identity** | Every element relates to itself, AND NOTHING ELSE. | $R = \{(a,a) \mid a \in A\}$ strictly |
| **Range** | The actual outputs produced by the function. | Set of all $f(x)$ |
| **Codomain** | The universe of possible outputs declared in the definition. | The set $B$ in $f: A \to B$ |
| **Inverse $f^{-1}$**| Function that reverses the mapping. | Exists ONLY if $f$ is bijective. |
## Part 5: High-Yield Worked Model Problems

### Problem 1: Equivalence Relation (ISC Guaranteed Type)
**Q:** Let $\mathbb{N}$ be the set of natural numbers and $R$ be a relation on $\mathbb{N} \times \mathbb{N}$ defined by $(a,b) R (c,d) \iff ad = bc$. Show that $R$ is an equivalence relation.
**Solution (ISC Method):**
*   **Reflexivity**: Let $(a,b) \in \mathbb{N} \times \mathbb{N}$. Since multiplication is commutative in $\mathbb{N}$, $ab = ba$. Thus, $(a,b) R (a,b)$. $R$ is reflexive.
*   **Symmetry**: Let $(a,b), (c,d) \in \mathbb{N} \times \mathbb{N}$ and $(a,b) R (c,d)$.
    $\implies ad = bc$.
    We can rewrite this as $cb = da$ (commutativity).
    $\implies (c,d) R (a,b)$. Thus, $R$ is symmetric.
*   **Transitivity**: Let $(a,b) R (c,d)$ and $(c,d) R (e,f)$.
    $\implies ad = bc$ and $cf = de$.
    Multiply the two equations: $(ad)(cf) = (bc)(de)$.
    Cancel common terms $c$ and $d$ (since they are in $\mathbb{N}$, neither is zero):
    $af = be \implies (a,b) R (e,f)$. Thus, $R$ is transitive.
Since $R$ is reflexive, symmetric, and transitive, it is an equivalence relation.

### Problem 2: Proving Bijectivity and Finding Inverse (Standard 4-Marker)
**Q:** Consider $f: \mathbb{R} - \{-\frac{4}{3}\} \to \mathbb{R} - \{\frac{4}{3}\}$ defined by $f(x) = \frac{4x+3}{3x+4}$. Show $f$ is bijective and find $f^{-1}$.
**Solution:**
**1. One-One (Injectivity):**
Let $x_1, x_2 \in \text{Domain}$ such that $f(x_1) = f(x_2)$.
$\frac{4x_1+3}{3x_1+4} = \frac{4x_2+3}{3x_2+4}$
$(4x_1+3)(3x_2+4) = (4x_2+3)(3x_1+4)$
$12x_1x_2 + 16x_1 + 9x_2 + 12 = 12x_1x_2 + 16x_2 + 9x_1 + 12$
$16x_1 - 9x_1 = 16x_2 - 9x_2 \implies 7x_1 = 7x_2 \implies x_1 = x_2$.
Therefore, $f$ is one-one.

**2. Onto (Surjectivity):**
Let $y \in \text{Codomain}$. Let $y = \frac{4x+3}{3x+4}$.
$y(3x+4) = 4x+3 \implies 3xy + 4y = 4x + 3$
$3xy - 4x = 3 - 4y \implies x(3y - 4) = 3 - 4y \implies x = \frac{3-4y}{3y-4}$.
For every $y \in \mathbb{R} - \{\frac{4}{3}\}$, $x$ is well-defined and $x \in \mathbb{R} - \{-\frac{4}{3}\}$.
Hence, $f$ is onto.
Since $f$ is one-one and onto, $f$ is bijective and hence invertible.

**3. Inverse:**
From the onto proof, we isolated $x = \frac{3-4y}{3y-4}$.
Thus, $f^{-1}(y) = \frac{3-4y}{3y-4}$.
Replacing with $x$: $f^{-1}(x) = \frac{3-4x}{3x-4}$.

### Problem 3: JEE Speed Hacks - Number of Functions
**Concept:** Let $|A| = m$ and $|B| = n$.
*   **Total number of functions**: $n^m$
*   **Number of One-One functions**:
    *   If $m > n$: 0
    *   If $m \le n$: $P(n, m) = \frac{n!}{(n-m)!}$
*   **Number of Bijective functions**:
    *   If $m \ne n$: 0
    *   If $m = n$: $n!$
*   **Number of Onto functions**: 
    *   If $m < n$: 0
    *   If $m \ge n$: $\sum_{r=1}^{n} (-1)^{n-r} \binom{n}{r} r^m$

**Q (JEE Main):** If $A = \{1, 2, 3, 4, 5\}$ and $B = \{a, b, c\}$, find the total number of onto functions from A to B.
**Solution (Speed formula):** Here $m=5, n=3$.
Number of onto functions = $\sum_{r=1}^{3} (-1)^{3-r} \binom{3}{r} r^5$
$= (-1)^2 \binom{3}{1} (1)^5 + (-1)^1 \binom{3}{2} (2)^5 + (-1)^0 \binom{3}{3} (3)^5$
$= 3(1) - 3(32) + 1(243) = 3 - 96 + 243 = 150$.
