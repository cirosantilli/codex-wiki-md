<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

A lower bound on individual [step costs](../../../../../step-cost.md) does **not** bound the difference between consecutive [path cost](../../../../../path-cost.md) thresholds. Two different paths can have costs differing by an arbitrarily small amount, even though every edge costs at least $\epsilon$.

Let $C^*$ be the optimal solution cost. Every unsuccessful threshold is the [path cost](../../../../../path-cost.md) of some [search node](../../../../../search-node.md) below $C^*$. Such a node has depth strictly less than $C^*/\epsilon$. For a uniform [branching factor](../../../../../branching-factor.md) $b>1$, the number of passes is therefore bounded by

$$
1+\sum_{j=0}^{\lceil C^*/\epsilon\rceil-1}b^j=O\!\left(b^{\lceil C^*/\epsilon\rceil}\right).
$$

If a solution of depth $d$ exists, each of its edges costs at most one, so $C^*\leq d$ and an associated bound is **$O(b^{\lceil d/\epsilon\rceil})$ passes**. If $d$ denotes the optimal solution's depth, the same inequality applies. With no solution-cost or solution-depth bound, $b$ and $\epsilon$ alone give no finite uniform iteration bound.

The exponential behavior is possible. Put a depth-$d$ goal on a branch with unit costs and let a large competing subtree use costs just above $\epsilon$. Choose tiny distinct perturbations so that its many [search nodes](../../../../../search-node.md) below cost $d$ have distinct [path costs](../../../../../path-cost.md). The threshold can advance through those costs one at a time. Thus **a bound such as $\lceil d/\epsilon\rceil$ on the number of passes is unjustified**: it bounds admitted depth, not the number of distinct costs. For $b=1$ there is only one path, so the corresponding count is linear in the admitted depth rather than exponential.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2019](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
