# Chapter 13: Probability

## Part 1: Exhaustive Theory & Precise ISC Terminology

### 1. Conditional Probability
*   **Sample Space ($S$)**: The set of all possible outcomes of a random experiment.
*   **Event ($E$)**: A subset of the sample space.
*   **Conditional Probability**: The probability of an event $E$ occurring, given that another event $F$ has already occurred. It is denoted by $P(E|F)$.
*   **Formula**: $P(E|F) = \frac{P(E \cap F)}{P(F)}$, where $P(F) \neq 0$.
*   **Properties of Conditional Probability**:
    *   $P(S|F) = P(F|F) = 1$
    *   If $A$ and $B$ are any two events and $F$ is an event such that $P(F) \neq 0$, then $P(A \cup B|F) = P(A|F) + P(B|F) - P(A \cap B|F)$.
    *   $P(E'|F) = 1 - P(E|F)$

### 2. Multiplication Theorem on Probability
*   The probability of simultaneous occurrence of two events $E$ and $F$ is given by $P(E \cap F) = P(E) \cdot P(F|E)$, given $P(E) \neq 0$, or $P(E \cap F) = P(F) \cdot P(E|F)$, given $P(F) \neq 0$.
*   This can be extended to three or more events: $P(E \cap F \cap G) = P(E) \cdot P(F|E) \cdot P(G|E \cap F)$.

### 3. Independent Events
*   Two events $E$ and $F$ are said to be **Independent Events** if the probability of occurrence of one of them is not affected by the occurrence of the other.
*   **Condition for Independence**: $P(E|F) = P(E)$ and $P(F|E) = P(F)$.
*   **Mathematical Definition**: $E$ and $F$ are independent if and only if $P(E \cap F) = P(E) \cdot P(F)$.
*   **Mutually Exclusive vs. Independent**: Mutually exclusive events (cannot happen at the same time, $P(E \cap F) = 0$) are generally *not* independent, unless one of them has zero probability.

### 4. Theorem of Total Probability
*   **Partition of a Sample Space**: A set of events $E_1, E_2, \dots, E_n$ is said to represent a partition of the sample space $S$ if:
    1.  They are **pairwise mutually exclusive**: $E_i \cap E_j = \phi$ for $i \neq j$.
    2.  They are **exhaustive**: $E_1 \cup E_2 \cup \dots \cup E_n = S$.
    3.  They have **non-zero probabilities**: $P(E_i) > 0$ for all $i$.
*   **Theorem**: Let $E_1, E_2, \dots, E_n$ be a partition of the sample space $S$, and let $A$ be any event which occurs with $E_1$ or $E_2$ or ... or $E_n$. Then, $P(A) = \sum_{j=1}^{n} P(E_j) \cdot P(A|E_j)$.

### 5. Bayes' Theorem (Inverse Probability)
*   **Statement**: If $E_1, E_2, \dots, E_n$ are $n$ non-empty events which constitute a partition of sample space $S$, and $A$ is any event of non-zero probability, then the conditional probability of $E_i$ given that $A$ has occurred is given by:
    $P(E_i|A) = \frac{P(E_i) \cdot P(A|E_i)}{\sum_{j=1}^{n} P(E_j) \cdot P(A|E_j)}$
*   **Prior Probabilities**: The probabilities $P(E_1), P(E_2), \dots, P(E_n)$ which are known before the experiment.
*   **Posterior Probabilities**: The probabilities $P(E_i|A)$ determined after the results of the experiment are known.

### 6. Random Variables and Probability Distributions
*   **Random Variable ($X$)**: A real-valued function whose domain is the sample space of a random experiment. It associates a unique real number with each outcome.
*   **Probability Distribution**: A system of numbers describing the possible values of a random variable along with their respective probabilities. It is usually represented in a tabular form.
    *   $\sum_{i=1}^{n} P(x_i) = 1$ and $P(x_i) \ge 0$.
*   **Mean / Expected Value ($\mu$ or $E(X)$)**: $\mu = E(X) = \sum_{i=1}^{n} x_i \cdot P(x_i)$. Represents the average value in the long run.
*   **Variance ($\sigma^2$ or $Var(X)$)**: $\sigma^2 = E(X^2) - [E(X)]^2 = \sum (x_i^2 \cdot P(x_i)) - \mu^2$. Measures the spread or dispersion of the distribution.
*   **Standard Deviation ($\sigma$)**: $\sigma = \sqrt{Var(X)}$.

### 7. Bernoulli Trials and Binomial Distribution
*   **Bernoulli Trials**: A sequence of independent trials of an experiment is called Bernoulli trials if it satisfies:
    1.  There should be a finite number of trials.
    2.  The trials should be independent.
    3.  Each trial has exactly two outcomes: success or failure.
    4.  The probability of success ($p$) remains the same in each trial.
*   **Binomial Distribution**: The probability distribution of the number of successes $X$ in $n$ Bernoulli trials.
    *   $P(X = r) = \binom{n}{r} p^r q^{n-r}$, where $r = 0, 1, 2, \dots, n$, $p$ is the probability of success, and $q = 1 - p$ is the probability of failure.
*   **Mean and Variance of Binomial Distribution**:
    *   Mean ($\mu$) = $np$
    *   Variance ($\sigma^2$) = $npq$
    *   Standard Deviation ($\sigma$) = $\sqrt{npq}$
## Part 2: Step-by-Step Derivations & Mechanisms

### 1. Derivation of Conditional Probability Formula
*   **Context**: Event $F$ has occurred. The new sample space becomes $F$.
*   **Mechanism**: To find the probability of $E$ occurring given $F$, we look for outcomes that are in both $E$ and $F$ (i.e., $E \cap F$) out of the total outcomes in the new sample space $F$.
*   **Step 1**: Let $n(S)$ be the total number of equally likely outcomes in the sample space.
*   **Step 2**: Let $n(F)$ be the number of outcomes favorable to $F$, and $n(E \cap F)$ be the number of outcomes favorable to both $E$ and $F$.
*   **Step 3**: $P(E|F) = \frac{n(E \cap F)}{n(F)}$.
*   **Step 4**: Divide numerator and denominator by $n(S)$:
    $P(E|F) = \frac{n(E \cap F) / n(S)}{n(F) / n(S)} = \frac{P(E \cap F)}{P(F)}$.

### 2. Mechanism of Total Probability Theorem
*   **Goal**: Find the total probability of an event $A$ that can occur along with any of the mutually exclusive and exhaustive events $E_1, E_2, \dots, E_n$.
*   **Step 1**: Express $A$ in terms of the partition: $A = A \cap S = A \cap (E_1 \cup E_2 \cup \dots \cup E_n)$.
*   **Step 2**: Apply distributive law: $A = (A \cap E_1) \cup (A \cap E_2) \cup \dots \cup (A \cap E_n)$.
*   **Step 3**: Since $E_1, E_2, \dots, E_n$ are mutually exclusive, $(A \cap E_1), (A \cap E_2), \dots$ are also mutually exclusive.
*   **Step 4**: $P(A) = P(A \cap E_1) + P(A \cap E_2) + \dots + P(A \cap E_n)$.
*   **Step 5**: Apply Multiplication Theorem: $P(A \cap E_i) = P(E_i) \cdot P(A|E_i)$.
*   **Final Formula**: $P(A) = \sum P(E_i) \cdot P(A|E_i)$.

### 3. Derivation of Bayes' Theorem
*   **Goal**: Find $P(E_i|A)$, the probability that the partition $E_i$ caused the event $A$.
*   **Step 1**: Use the definition of conditional probability:
    $P(E_i|A) = \frac{P(E_i \cap A)}{P(A)}$.
*   **Step 2**: Expand the numerator using the Multiplication Theorem:
    $P(E_i \cap A) = P(E_i) \cdot P(A|E_i)$.
*   **Step 3**: Expand the denominator using the Theorem of Total Probability:
    $P(A) = \sum_{j=1}^{n} P(E_j) \cdot P(A|E_j)$.
*   **Step 4**: Substitute back into the equation:
    $P(E_i|A) = \frac{P(E_i) \cdot P(A|E_i)}{\sum_{j=1}^{n} P(E_j) \cdot P(A|E_j)}$.

### 4. Mean and Variance of a Random Variable Formula
*   **Mean $\mu$ (Expected Value)**:
    It acts as the center of gravity for the probability distribution.
    $E(X) = \sum_{i=1}^{n} x_i P(x_i)$.
*   **Variance $\sigma^2$**:
    Measures average squared deviation from the mean.
    $Var(X) = E((X - \mu)^2) = \sum (x_i - \mu)^2 P(x_i)$.
    Expanding this gives the computational formula:
    $Var(X) = \sum (x_i^2 - 2x_i\mu + \mu^2) P(x_i)$
    $= \sum x_i^2 P(x_i) - 2\mu \sum x_i P(x_i) + \mu^2 \sum P(x_i)$
    $= E(X^2) - 2\mu(\mu) + \mu^2(1) = E(X^2) - \mu^2$.
## Part 3: Diagram Blueprints & Labeling Checklists

### 1. Tree Diagrams for Total Probability and Bayes' Theorem
Tree diagrams are essential for breaking down complex conditional probability problems.

*   **Blueprint Structure**:
    *   **Root Node**: Represents the starting point of the experiment.
    *   **First-Level Branches (Causes / Partitions)**: Branch out to events $E_1, E_2, \dots, E_n$.
        *   **Label**: Write $P(E_1), P(E_2), \dots$ on these branches. Ensure their sum is 1.
    *   **Second-Level Branches (Effects)**: From each $E_i$, branch out to the event of interest $A$ and its complement $A'$.
        *   **Label**: Write $P(A|E_1), P(A'|E_1)$, etc. Ensure branches from the same node sum to 1.
    *   **Terminal Nodes (Intersections)**: The end of a path represents $E_i \cap A$.
        *   **Value**: Multiply the probabilities along the path: $P(E_i) \cdot P(A|E_i)$.
*   **ISC Labeling Checklist**:
    *   [ ] Event notations clearly defined ($E_1$: choosing Bag 1, $A$: drawing a red ball).
    *   [ ] Probabilities on branches clearly written as fractions.
    *   [ ] Total probability $P(A)$ calculated by summing the relevant terminal nodes.
    *   [ ] For Bayes' Theorem, clearly identify the specific path divided by the sum of all paths leading to $A$.

### 2. Probability Distribution Table
A systematic way to present a random variable and its probabilities.

*   **Blueprint Structure**:
    *   A horizontal table with two main rows: $X$ (Random Variable) and $P(X)$ (Probability).
    *   Additional rows for computation: $X \cdot P(X)$ (for Mean) and $X^2 \cdot P(X)$ (for Variance).
*   **Format**:
    | $X = x_i$ | $x_1$ | $x_2$ | $\dots$ | $x_n$ | **Total** |
    | :--- | :--- | :--- | :--- | :--- | :--- |
    | $P(X = x_i)$ | $p_1$ | $p_2$ | $\dots$ | $p_n$ | $\sum p_i = 1$ |
    | $x_i \cdot P(x_i)$ | $x_1p_1$ | $x_2p_2$ | $\dots$ | $x_np_n$ | $\sum x_ip_i = \mu$ |
    | $x_i^2 \cdot P(x_i)$ | $x_1^2p_1$| $x_2^2p_2$| $\dots$ | $x_n^2p_n$| $\sum x_i^2p_i = E(X^2)$ |
*   **ISC Labeling Checklist**:
    *   [ ] Header row clearly denoting the variable $X$ and its values.
    *   [ ] Verification row showing $\sum P(X) = 1$ (Mandatory for ISC step marks).
    *   [ ] Proper formulation of Expected Value and Variance formulas below the table.

### 3. Venn Diagrams for Probability
Useful for Set Theory-based probability questions ($P(A \cup B)$, $P(A \cap B)$, etc.).
*   **Blueprint Structure**:
    *   **Rectangle**: Represents the Sample Space ($S$), $P(S) = 1$.
    *   **Circles**: Represent Events $A$ and $B$.
    *   **Regions**:
        *   $A \cap B$: Intersection (both).
        *   $A - B$ or $A \cap B'$: Only $A$.
        *   $B - A$ or $B \cap A'$: Only $B$.
        *   $(A \cup B)'$: Neither $A$ nor $B$.
*   **ISC Labeling Checklist**:
    *   [ ] Universal set $S$ labelled in the corner.
    *   [ ] Regions shaded correctly according to the event asked (e.g., $P(A \cup B)$).
    *   [ ] Disjoint circles for mutually exclusive events.
## Part 4: "Avoid the Trap" & Distinction Tables

### 1. Objective vs. Subjective Traps (ISC & JEE)

| The Trap | The Mistake (What Students Do) | The Fix (What You Should Do) |
| :--- | :--- | :--- |
| **Independent vs. Mutually Exclusive** | Confusing the two concepts. Assuming if events are mutually exclusive, they are independent. | **Mutually Exclusive**: $P(A \cap B) = 0$. (Cannot happen together). <br> **Independent**: $P(A \cap B) = P(A) \cdot P(B)$. (One doesn't affect the other). If they are mutually exclusive, they *cannot* be independent (unless one has zero probability). |
| **"At least one" vs. "Exactly one"** | Misinterpreting the phrasing in Binomial Distribution or probability rules. | **At least one**: $1 - P(\text{None})$. (Use $1 - P(A' \cap B' \cap \dots)$). <br> **Exactly one**: $P(A \cap B') + P(A' \cap B)$. |
| **With Replacement vs. Without Replacement** | Treating 'without replacement' as independent events. | **With Replacement**: Independent events. Probabilities remain constant. <br> **Without Replacement**: Dependent events. Use Conditional Probability. The denominator decreases by 1 each draw. |
| **Bayes' Theorem vs. Total Probability** | Applying Bayes' Theorem when only the total probability is asked. | Read the last line carefully. If it asks "What is the probability of drawing a red ball?", use **Total Probability**. If it asks "Given a red ball is drawn, what is the probability it came from Bag 1?", use **Bayes' Theorem**. |
| **Binomial Distribution Check** | Applying binomial distribution when trials are not independent or probability of success changes. | Always verify: 1. Fixed number of trials ($n$). 2. Two outcomes (success/fail). 3. Independent trials. 4. Constant probability of success ($p$). |
| **Variance Calculation Trap** | Using $Var(X) = E(X^2)$ instead of $E(X^2) - (E(X))^2$. | Always remember to subtract the square of the mean: $\sum x^2 P(x) - \mu^2$. Forgetting $\mu^2$ is a common fatal error. |

### 2. Notation Distinction Table

| Notation | Meaning | When to Use |
| :--- | :--- | :--- |
| $P(A \cap B)$ | Probability of A **AND** B occurring. | Intersection. Multiplication theorem. $P(A) \cdot P(B\|A)$. |
| $P(A \cup B)$ | Probability of A **OR** B (or both) occurring. | Union. Addition theorem. $P(A) + P(B) - P(A \cap B)$. |
| $P(A\|B)$ | Probability of A **GIVEN** that B has occurred. | Conditional Probability. Reduces the sample space to $B$. |
| $P(A' \cap B')$ | Probability of **NEITHER** A **NOR** B. | De Morgan's Law: $P((A \cup B)') = 1 - P(A \cup B)$. |
| $P(A \cap B')$ | Probability of **ONLY A** (A but not B). | $P(A) - P(A \cap B)$. |
## Part 5: High-Yield Worked Model Problems

### Problem 1: Conditional Probability (Matrix Type)
**Question:** A family has two children. Find the probability that both are boys, given that at least one is a boy.

**ISC Step-by-Step Method:**
1.  **Define Sample Space**: $S = \{(B, B), (B, G), (G, B), (G, G)\}$, so $n(S) = 4$.
2.  **Define Events**:
    *   Let $E$ be the event that both children are boys: $E = \{(B, B)\}$.
    *   Let $F$ be the event that at least one child is a boy: $F = \{(B, B), (B, G), (G, B)\}$.
3.  **Find Probabilities**:
    *   $P(F) = \frac{n(F)}{n(S)} = \frac{3}{4}$
    *   $E \cap F = \{(B, B)\}$, so $P(E \cap F) = \frac{1}{4}$
4.  **Apply Formula**:
    *   $P(E|F) = \frac{P(E \cap F)}{P(F)} = \frac{1/4}{3/4} = \frac{1}{3}$.

**JEE Speed Method:**
Directly restrict the sample space. Given "at least one boy", the new sample space is $\{BB, BG, GB\}$ (size 3). We want "both boys", which is $\{BB\}$ (size 1). Probability = 1/3.

---

### Problem 2: Bayes' Theorem (The Urn/Bag Problem)
**Question:** Bag I contains 3 red and 4 black balls while another Bag II contains 5 red and 6 black balls. One ball is drawn at random from one of the bags and it is found to be red. Find the probability that it was drawn from Bag II.

**ISC Step-by-Step Method:**
1.  **Define Events**:
    *   $E_1$: Event of choosing Bag I.
    *   $E_2$: Event of choosing Bag II.
    *   $A$: Event of drawing a red ball.
2.  **State Prior Probabilities**:
    *   $P(E_1) = \frac{1}{2}$, $P(E_2) = \frac{1}{2}$ (Choosing either bag is equally likely).
3.  **State Conditional Probabilities**:
    *   $P(A|E_1) = \frac{3}{7}$ (Probability of Red given Bag I).
    *   $P(A|E_2) = \frac{5}{11}$ (Probability of Red given Bag II).
4.  **State Bayes' Theorem Formula**:
    $P(E_2|A) = \frac{P(E_2) \cdot P(A|E_2)}{P(E_1) \cdot P(A|E_1) + P(E_2) \cdot P(A|E_2)}$
5.  **Substitute and Calculate**:
    $P(E_2|A) = \frac{(1/2) \cdot (5/11)}{(1/2) \cdot (3/7) + (1/2) \cdot (5/11)}$
    $P(E_2|A) = \frac{5/11}{3/7 + 5/11} = \frac{5/11}{(33 + 35)/77} = \frac{5/11}{68/77} = \frac{5}{11} \cdot \frac{77}{68} = \frac{35}{68}$.
*(ISC Note: Explicitly defining $E_1, E_2, A$ and stating the formula carries 2 step marks).*

**JEE Speed Method:**
Use a mental tree diagram or ratios.
Path 1 (Bag 1 $\rightarrow$ Red): $\frac{1}{2} \cdot \frac{3}{7} = \frac{3}{14} = \frac{33}{154}$
Path 2 (Bag 2 $\rightarrow$ Red): $\frac{1}{2} \cdot \frac{5}{11} = \frac{5}{22} = \frac{35}{154}$
Total Red Prob = $\frac{68}{154}$.
$P(\text{Bag 2} | \text{Red}) = \frac{\text{Path 2}}{\text{Total Red}} = \frac{35/154}{68/154} = \frac{35}{68}$.

---

### Problem 3: Random Variable and Variance (Cards)
**Question:** Two cards are drawn simultaneously (or successively without replacement) from a well-shuffled pack of 52 cards. Find the mean and variance of the number of kings.

**ISC Step-by-Step Method:**
1.  **Define Random Variable**: Let $X$ denote the number of kings in two draws. $X$ can take values 0, 1, or 2.
2.  **Calculate Probabilities**:
    *   $P(X = 0)$ (No king): $\frac{\binom{48}{2}}{\binom{52}{2}} = \frac{48 \cdot 47}{52 \cdot 51} = \frac{188}{221}$
    *   $P(X = 1)$ (One king, one non-king): $\frac{\binom{4}{1} \cdot \binom{48}{1}}{\binom{52}{2}} = \frac{4 \cdot 48 \cdot 2}{52 \cdot 51} = \frac{32}{221}$
    *   $P(X = 2)$ (Two kings): $\frac{\binom{4}{2}}{\binom{52}{2}} = \frac{4 \cdot 3}{52 \cdot 51} = \frac{1}{221}$
3.  **Construct Probability Distribution Table**:
    *   Verify $\sum P(X) = \frac{188 + 32 + 1}{221} = 1$. (Checked).
4.  **Calculate Mean**:
    $E(X) = \sum X \cdot P(X) = 0 \cdot \left(\frac{188}{221}\right) + 1 \cdot \left(\frac{32}{221}\right) + 2 \cdot \left(\frac{1}{221}\right) = \frac{34}{221} = \frac{2}{13}$.
5.  **Calculate Variance**:
    *   $E(X^2) = \sum X^2 \cdot P(X) = 0 \cdot \left(\frac{188}{221}\right) + 1^2 \cdot \left(\frac{32}{221}\right) + 2^2 \cdot \left(\frac{1}{221}\right) = \frac{36}{221}$.
    *   $Var(X) = E(X^2) - [E(X)]^2 = \frac{36}{221} - \left(\frac{2}{13}\right)^2 = \frac{36 \cdot 13}{221 \cdot 13} - \frac{4 \cdot 17}{169 \cdot 17} = \frac{468 - 68}{2873} = \frac{400}{2873}$.

**JEE Speed Method:**
For Mean: Drawing without replacement has the same expected value as with replacement due to linearity of expectation! $E(X) = n \cdot p = 2 \cdot \frac{4}{52} = 2 \cdot \frac{1}{13} = \frac{2}{13}$. (Instant Mean calculation!)
For Variance without replacement, use the formula for Hypergeometric variance: $n \cdot p \cdot q \cdot \frac{N-n}{N-1}$
$n = 2$, $p = \frac{1}{13}$, $q = \frac{12}{13}$, $N = 52$.
$Var = 2 \cdot \left(\frac{1}{13}\right) \cdot \left(\frac{12}{13}\right) \cdot \frac{52 - 2}{52 - 1} = \frac{24}{169} \cdot \frac{50}{51} = \frac{8 \cdot 50}{169 \cdot 17} = \frac{400}{2873}$.
*(Matches exactly, huge time saver!)*
