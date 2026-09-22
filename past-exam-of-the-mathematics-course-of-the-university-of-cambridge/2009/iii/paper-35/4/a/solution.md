<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Represent a feasible allocation by a label for each item saying which bidder receives it. Every such label vector gives disjoint bundles covering all items, so the following [heuristic optimization](../../../../../../heuristic-optimization.md) methods can search without violating allocation feasibility.

In [local search](../../../../../../local-search.md), begin with any feasible partition and repeatedly make an improving move, such as transferring one item between bidders or exchanging two items. For a transfer $j:i\to r$, evaluate the change

$$
v_i(S_i\setminus\{j\})-v_i(S_i)+v_r(S_r\cup\{j\})-v_r(S_r).
$$

Stop when no allowed move improves the objective. Several starting partitions can avoid dependence on one local optimum, but no guarantee of a global optimum follows for general bids.

In [simulated annealing](../../../../../../simulated-annealing.md), use the same feasible neighborhood but also accept a worsening move of loss $\Delta>0$ with [probability](../../../../../../probability.md) $e^{-\Delta/T}$ at temperature $T$. Begin with a relatively high temperature, gradually cool, and retain the best allocation seen. Worsening moves can cross a barrier between local optima; a practical finite cooling schedule does not guarantee optimality.

In [tabu search](../../../../../../tabu-search.md), retain a short memory of recent transfers or exchanges and temporarily prohibit their reversal. Select the best admissible move, possibly worsening the objective, to escape a local optimum. Permit an otherwise tabu move if it improves the best solution found, an aspiration rule. For the [winner determination problem](../../../../../../winner-determination-problem.md), bidder/item pairs or recent reverse transfers provide convenient tabu attributes. All three methods preserve the partition, but **for arbitrary bids they are heuristics rather than algorithms with a proved constant [approximation ratio](../../../../../../approximation-ratio.md)**.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
