<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Use Model 3 and keep every prescribed row at its prescribed column. Initialize one queen in every other row, and minimize the conflict count

$$
E(C)=\sum_{1\le r<s\le N}\mathbf1_{\{C_r=C_s\ \text{or}\ |C_r-C_s|=s-r\}}.
$$

This [sum](../../../../../sum.md) counts attacking pairs; $E=0$ is exactly a valid completion. A neighbor changes the column of one unfixed row. Evaluate such neighbors and move to one with lower $E$, breaking equal choices arbitrarily. Minimizing $E$, or maximizing $-E$, is [hill climbing](../../../../../hill-climbing.md) on complete domain assignments; these assignments need not yet satisfy the inter-row constraints. Fixed rows are never moved.

The [min-conflicts algorithm](../../../../../min-conflicts-algorithm.md) chooses a conflicted unfixed queen and places it in a column giving the smallest conflict count against the other queens. Recomputing only the affected pair contributions makes a move cheaper than reevaluating every pair. Equal-cost moves can help cross plateaus; bounded sideways moves or repeated random starts of only the unfixed queens can escape some traps. These modifications still preserve the prescribed positions.

**Return a board only after checking $E=0$ and every prescribed position.** A [local minimum](../../../../../local-minimum.md) with positive $E$ is not proof of impossibility. A [queens completion problem](../../../../../queens-completion-problem.md) may be unsatisfiable even when its prescribed queens do not attack each other; unrestricted restart policies give no finite worst-case success bound. If every row is fixed, simply validate the one board. For a guaranteed decision procedure use finite [backtracking](../../../../../backtracking.md), possibly with [constraint propagation](../../../../../constraint-propagation.md), instead of relying on [hill climbing](../../../../../hill-climbing.md).

## ↑ Ancestors (11)

1. [F](../f.md)
2. [3](../../3.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2022](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
