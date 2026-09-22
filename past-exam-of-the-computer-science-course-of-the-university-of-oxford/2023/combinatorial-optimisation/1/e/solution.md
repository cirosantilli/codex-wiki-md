<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Use the [chain lower bound for a submodular set function](../../../../../chain-lower-bound-for-a-submodular-set-function.md). Order $T=\{x_1,\ldots,x_n\}$, set $P_j=\{x_1,\ldots,x_j\}$ with $P_0=\varnothing$, and put $a_j=f(P_j)-f(P_{j-1})$. For each $U\subseteq T$, reveal its elements in this same order. Since $U\cap P_{j-1}\subseteq P_{j-1}$, [diminishing returns](../../../../../diminishing-returns-characterization-of-submodularity.md) and the [normalised set function](../../../../../normalised-set-function.md) property give

$$
f(U)=\sum_{j:x_j\in U}\Delta_{x_j}f(U\cap P_{j-1})
\geq\sum_{j:x_j\in U}a_j.
$$

Apply this to each $T_i$ and interchange the finite sums. Every element occurs exactly $k$ times, so

$$
\boxed{\sum_{i=1}^t f(T_i)\geq\sum_{j=1}^n k a_j=k\bigl(f(T)-f(\varnothing)\bigr)=k f(T).}
$$

This is the [exact-cover inequality for submodular set functions](../../../../../exact-cover-inequality-for-submodular-set-functions.md). Some $a_j$ can be negative: exact multiplicity, rather than merely at least $k$ occurrences, is what makes the argument valid without monotonicity. In fact the [nonnegative function](../../../../../nonnegative-function.md) hypothesis is unnecessary here. If $T=\varnothing$, every $T_i$ is empty and both sides vanish.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Combinatorial optimisation](../../../combinatorial-optimisation-split.md)
4. [2023](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
