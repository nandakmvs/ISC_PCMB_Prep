# Chapter 13: Probability

## 1. Exhaustive Theory & Precise ISC Terminology

- **Conditional Probability**: Probability of event E given that F has already occurred. $P(E|F) = \frac{P(E \cap F)}{P(F)}$, where $P(F) \neq 0$.
- **Multiplication Theorem**: $P(E \cap F) = P(E) \cdot P(F|E) = P(F) \cdot P(E|F)$.
- **Independent Events**: Two events E and F are independent if the occurrence of one does not affect the other. Mathematically, $P(E \cap F) = P(E) \cdot P(F)$. This implies $P(E|F) = P(E)$.
- **Partition of a Sample Space**: A set of events $E_1, E_2, \dots, E_n$ that are pairwise mutually exclusive ($E_i \cap E_j = \phi$) and exhaustive ($E_1 \cup E_2 \dots \cup E_n = S$), with non-zero probabilities.
- **Theorem of Total Probability**: Let $E_1, \dots, E_n$ be a partition of $S$, and A be any event. $P(A) = \sum_{j=1}^n P(E_j) \cdot P(A|E_j)$.
- **Bayes' Theorem**: Reverses conditional probability. If A is observed, what is the probability it was caused by $E_i$?
  $P(E_i|A) = \frac{P(E_i) \cdot P(A|E_i)}{\sum_{j=1}^n P(E_j) \cdot P(A|E_j)}$.
- **Random Variable (X)**: A real-valued function whose domain is the sample space of a random experiment.
- **Probability Distribution**: A table listing all possible values of X ($x_1, x_2, \dots$) and their corresponding probabilities $p_1, p_2, \dots$, where $\sum p_i = 1$.
- **Mean / Expected Value**: $\mu = E(X) = \sum x_i p_i$.
- **Variance**: $Var(X) = E(X^2) - [E(X)]^2 = \sum x_i^2 p_i - \mu^2$.
- **Bernoulli Trials**: Trials of a random experiment with only two possible outcomes (success/failure), where probability of success remains constant across independent trials.
- **Binomial Distribution**: Probability of exactly $r$ successes in $n$ Bernoulli trials: $P(X=r) = ^nC_r p^r q^{n-r}$, where $p$ is prob of success, $q=1-p$.

## 2. Step-by-Step Derivations & Mechanisms

**Mechanism for Bayes' Theorem Problems:**
1. **Identify the Partition Events ($E_1, E_2, \dots$)**: These are the initial distinct scenarios (e.g., picking Box 1, Box 2, or Box 3). Assign prior probabilities $P(E_i)$.
2. **Identify the Common Event (A)**: This is the event that is observed or known to have happened (e.g., "a red ball is drawn").
3. **Determine Conditional Probabilities ($P(A|E_i)$)**: Probability of event A happening under each specific scenario.
4. **Apply Formula**: Calculate numerator (specific path: $P(E_i) \cdot P(A|E_i)$) and divide by the total probability (sum of all paths).

## 3. Diagram Blueprints & Labeling Checklists

- **Probability Tree Diagram**:
  - Draw root node branching into the partition events $E_1, E_2$. Label branches with $P(E_1), P(E_2)$.
  - From each $E_i$, branch out to Event A and Event A'. Label branches with $P(A|E_i)$ and $P(A'|E_i)$.
  - The probability of a specific path (e.g., $E_1 \cap A$) is the product of probabilities along the branches. The total probability of A is the sum of all paths leading to A.

## 4. "Avoid the Trap" & Distinction Tables

| Trap / Common Mistake | Strategy / Fact to Remember |
| :--- | :--- |
| Independent vs Mutually Exclusive | **Mutually Exclusive**: Cannot happen together ($P(A \cap B) = 0$). **Independent**: One doesn't affect the other ($P(A \cap B) = P(A)P(B)$). They are NOT the same. In fact, if non-zero probability events are mutually exclusive, they CANNOT be independent. |
| Bayes vs Total Probability | If question asks "Find the probability that the ball drawn is red", use **Total Probability**. If it asks "Given the ball is red, find the probability it came from Bag II", use **Bayes' Theorem**. |
| Binomial variables limits | Remember $p + q = 1$. The number of successes $r$ must be $0 \le r \le n$. |

## 5. High-Yield Worked Model Problems

**Problem (ISC Step-by-Step)**: A man is known to speak the truth 3 out of 4 times. He throws a die and reports that it is a six. Find the probability that it is actually a six.
**Solution**:
1. Let $E_1$ be the event "a six actually occurs". $P(E_1) = 1/6$.
2. Let $E_2$ be the event "a six does not occur". $P(E_2) = 5/6$.
3. Let $A$ be the event "the man reports it is a six".
4. $P(A|E_1)$ = Probability he reports a six when it is a six = Prob he speaks truth = 3/4.
5. $P(A|E_2)$ = Probability he reports a six when it is not a six = Prob he lies = 1 - 3/4 = 1/4.
6. We need to find $P(E_1|A)$. By Bayes' Theorem:
   $P(E_1|A) = \frac{P(E_1)P(A|E_1)}{P(E_1)P(A|E_1) + P(E_2)P(A|E_2)}$
   $= \frac{(1/6) \times (3/4)}{(1/6) \times (3/4) + (5/6) \times (1/4)} = \frac{3/24}{3/24 + 5/24} = \frac{3}{8}$.

**Problem (NEET/JEE Speed Method)**: A fair coin is tossed 10 times. Find the probability of getting exactly 6 heads.
**Solution**:
This is a binomial distribution problem. $n = 10$.
Success is getting a head. $p = 1/2$, $q = 1/2$.
We need $P(X = 6)$.
$P(X=r) = ^nC_r p^r q^{n-r}$
$P(X=6) = ^{10}C_6 (1/2)^6 (1/2)^4 = \frac{10 \times 9 \times 8 \times 7}{4 \times 3 \times 2 \times 1} \times (1/2)^{10} = \frac{210}{1024} = \frac{105}{512}$.
