# Chapter 1: Relations and Functions

## 1. Exhaustive Theory & Precise ISC Terminology

A **Cartesian Product** $A \times B$ is the set of all ordered pairs $(a,b)$ where $a \in A$ and $b \in B$.
A **Relation** $R$ from a non-empty set A to a non-empty set B is a subset of the Cartesian product $A \times B$.
**Domain**: The set of all first elements of the ordered pairs in a relation.
**Range**: The set of all second elements of the ordered pairs in a relation.
**Codomain**: The entire set B. Range $\subseteq$ Codomain.

### Types of Relations
1. **Empty Relation**: No element of $A$ is related to any element of $A$, i.e., $R = \phi \subset A \times A$.
2. **Universal Relation**: Each element of $A$ is related to every element of $A$, i.e., $R = A \times A$.
3. **Reflexive Relation**: $(a, a) \in R$ for every $a \in A$.
4. **Symmetric Relation**: $(a, b) \in R \implies (b, a) \in R$ for all $a, b \in A$.
5. **Transitive Relation**: $(a, b) \in R$ and $(b, c) \in R \implies (a, c) \in R$ for all $a, b, c \in A$.
6. **Equivalence Relation**: A relation which is reflexive, symmetric, and transitive.

**Equivalence Class**: For an equivalence relation $R$ on set $X$, the equivalence class of $a \in X$, denoted by $[a]$, is the set of all elements of $X$ related to $a$.

### Types of Functions
A relation $f: A \to B$ is a **Function** if every element of $A$ has one and only one image in $B$.
1. **One-One (Injective)**: Distinct elements of $A$ have distinct images in $B$. $f(x_1) = f(x_2) \implies x_1 = x_2$.
2. **Many-One**: Two or more elements of $A$ have the same image in $B$.
3. **Onto (Surjective)**: Every element of $B$ is the image of some element of $A$. Range = Codomain.
4. **Into**: There is at least one element in $B$ which is not the image of any element of $A$.
5. **Bijective Function**: A function that is both One-One and Onto.

### Composition of Functions & Invertible Functions
**Composition**: Let $f: A \to B$ and $g: B \to C$. The composition $g \circ f: A \to C$ is given by $(g \circ f)(x) = g(f(x))$ for all $x \in A$.
**Invertible Function**: A function $f: X \to Y$ is invertible if there exists a function $g: Y \to X$ such that $g \circ f = I_X$ and $f \circ g = I_Y$. A function is invertible if and only if it is bijective.

## 2. Step-by-Step Derivations & Mechanisms

**Mechanism to Prove a Relation is an Equivalence Relation:**
1. **Reflexive**: Substitute $y = x$ in the relation condition. Show it holds true for all $x \in A$.
2. **Symmetric**: Assume $(x, y) \in R$. Manipulate the condition to show $(y, x) \in R$.
3. **Transitive**: Assume $(x, y) \in R$ and $(y, z) \in R$. Combine both conditions to deduce $(x, z) \in R$.

**Mechanism to Prove Bijectivity (One-One & Onto):**
1. **Injective (One-One)**: Let $x_1, x_2 \in Domain$. Set $f(x_1) = f(x_2)$. Solve to show $x_1 = x_2$.
2. **Surjective (Onto)**: Let $y \in Codomain$. Set $y = f(x)$. Solve for $x$ in terms of $y$. Show that for every $y \in Codomain$, the resulting $x$ belongs to the Domain.

## 3. Diagram Blueprints & Labeling Checklists

- **Mapping/Arrow Diagrams**: Draw two distinct ovals for Set A and Set B.
  - **One-One**: Every dot in Set A points to a unique dot in Set B. No two arrows converge on the same dot in B.
  - **Onto**: Every dot in Set B has at least one incoming arrow from Set A. No dots in B are left without an arrow.
  - **Bijective**: Perfect 1:1 pairing. Equal number of elements in both sets if finite.

## 4. "Avoid the Trap" & Distinction Tables

| Trap / Common Mistake | Strategy / Fact to Remember |
| :--- | :--- |
| Assuming $f \circ g = g \circ f$ | Composition of functions is generally **not commutative**. Always calculate both carefully if required. |
| Forgetting Domain restrictions | When finding inverses, ensure the derived $f^{-1}(y)$ produces an $x$ that is actually in the original domain. |
| Confusion over Transitivity | If $(a,b) \in R$ but there is NO $(b,c) \in R$, the relation is **still transitive** vacuously. Transitivity only fails if $(a,b)$ and $(b,c)$ exist, but $(a,c)$ does NOT. |

## 5. High-Yield Worked Model Problems

**Problem (ISC Step-by-Step)**: Show that the relation $R$ in the set $Z$ of integers given by $R = \{(a, b) : 2 \text{ divides } a - b\}$ is an equivalence relation.
**Solution**:
1. **Reflexivity**: For any $a \in Z$, $a - a = 0$. Since 2 divides 0, $(a, a) \in R$. Therefore, $R$ is reflexive.
2. **Symmetry**: Let $(a, b) \in R$. Then $2$ divides $a - b$. So, $a - b = 2k$ for some integer $k$. Then $b - a = 2(-k)$. Since $-k$ is an integer, 2 divides $b - a$. Thus, $(b, a) \in R$. Therefore, $R$ is symmetric.
3. **Transitivity**: Let $(a, b) \in R$ and $(b, c) \in R$. Then $a - b = 2k_1$ and $b - c = 2k_2$ for some integers $k_1, k_2$. Adding them: $(a - b) + (b - c) = 2k_1 + 2k_2 \implies a - c = 2(k_1 + k_2)$. Since $k_1+k_2$ is an integer, 2 divides $a-c$, so $(a,c) \in R$. Therefore, $R$ is transitive.
Since $R$ is reflexive, symmetric, and transitive, it is an equivalence relation.

**Problem (NEET/JEE Speed Method)**: Let $f: R \to R$ be defined by $f(x) = \frac{x-1}{x+1}$. Find $f(f(x))$.
**Solution**: 
$f(f(x)) = f\left(\frac{x-1}{x+1}\right) = \frac{\frac{x-1}{x+1} - 1}{\frac{x-1}{x+1} + 1} = \frac{x-1 - (x+1)}{x-1 + x+1} = \frac{-2}{2x} = -\frac{1}{x}$.
Speed tip: Recognize the fractional linear transformation form $T(x) = \frac{ax+b}{cx+d}$. Matrix multiplication of coefficients can be used for multiple compositions.
