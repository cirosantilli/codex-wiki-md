<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

**[Breadth-first tree search](../../../../../breadth-first-tree-search.md) is complete and optimal for minimizing rounds.** If a successful escape has finite length $d$, there are only finitely many nodes at depths below $d$, since the [branching factor](../../../../../branching-factor.md) is at most five. [Breadth-first tree search](../../../../../breadth-first-tree-search.md) therefore reaches a shallowest successful node after finite work, even if other branches continue forever.

It is an [optimal search algorithm](../../../../../optimal-search-algorithm.md) because every [search transition model](../../../../../search-transition-model.md) step costs one round, so minimum depth is exactly the desired minimum number of rounds. The [goal test](../../../../../goal-test.md) must be applied to the surviving complete-round successor. Here a [complete search algorithm](../../../../../complete-search-algorithm.md) guarantees finding an escape when one exists; it need not terminate on every unsolvable instance.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2023](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
