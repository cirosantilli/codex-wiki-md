<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

**Yes. [Greedy best-first search](../../../../../greedy-best-first-search.md) needs only the ordering of remaining-cost estimates.** Store generated but unexpanded [search nodes](../../../../../search-node.md) in a [search frontier](../../../../../search-frontier.md). To choose the next [search node](../../../../../search-node.md), compare candidates with $\kappa$ and retain the one it returns; a linear scan suffices, or a [priority queue](../../../../../priority-queue.md) can use the comparison rule. Remove that [search node](../../../../../search-node.md), apply the [goal test](../../../../../goal-test.md), and otherwise generate its children.

This implements [best-first search](../../../../../best-first-search.md) ordered by $h^*$ without ever evaluating $h^*$. If stable tie handling is wanted, comparing both argument orders distinguishes equality, after which insertion order can break ties. No estimate of accumulated-plus-remaining cost is required for this greedy ordering.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2021](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
