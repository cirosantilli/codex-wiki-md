<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a finite [constraint satisfaction problem](../../../../../constraint-satisfaction-problem.md) with $v$ variables, all complete assignments have depth $v$ when each step assigns one new variable. Thus the shallowest-solution property of [breadth-first search](../../../../../breadth-first-search.md) offers no advantage: every complete solution is already at that depth.

[Depth-first search](../../../../../depth-first-search.md) with [backtracking](../../../../../backtracking.md) stores a path and pending choices, using $O(vd)$ auxiliary space with ordinary explicit choice bookkeeping, or $O(v)$ when each level stores only a current value index. [Breadth-first search](../../../../../breadth-first-search.md) may store an exponentially large frontier, up to $O(d^v)$ partial assignments. [Depth-first search](../../../../../depth-first-search.md) can also combine naturally with immediate [constraint propagation](../../../../../constraint-propagation.md) and undoing changes. The finite depth avoids the infinite-branch obstruction of unrestricted [depth-first tree search](../../../../../depth-first-tree-search.md). Neither traversal removes the possible exponential [time complexity](../../../../../time-complexity.md).

## ↑ Ancestors (11)

1. [C](../c.md)
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
