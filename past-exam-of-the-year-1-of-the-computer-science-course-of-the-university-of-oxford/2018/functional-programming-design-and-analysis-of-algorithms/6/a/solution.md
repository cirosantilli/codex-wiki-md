<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

There are three useful distinctions between [dynamic programming](../../../../../dynamic-programming.md) and a conventional [divide-and-conquer algorithm](../../../../../divide-and-conquer-algorithm.md).

- A [divide-and-conquer algorithm](../../../../../divide-and-conquer-algorithm.md) typically splits one instance into mostly separate smaller instances; [dynamic programming](../../../../../dynamic-programming.md) deliberately recognizes overlapping subproblems that recur along different decision histories.
- A [dynamic programming state](../../../../../dynamic-programming-state.md) is solved once and its result reused through a table or [memoization](../../../../../memoization.md). A direct [divide-and-conquer algorithm](../../../../../divide-and-conquer-algorithm.md) normally combines the results of its recursive children without retaining a table indexed by all repeated states.
- The dependency structure of a direct recursive decomposition is a [recursion tree](../../../../../recursion-tree.md); [dynamic programming](../../../../../dynamic-programming.md) evaluates a [Directed acyclic graph](../../../../../directed-acyclic-graph.md) of states in dependency order, either bottom-up or by [memoization](../../../../../memoization.md). Its cost is the number of distinct states times the work per state, rather than the number of occurrences in the expanded [recursion tree](../../../../../recursion-tree.md).

These are paradigm-level distinctions, not mutually exclusive definitions: a recursive algorithm can use [memoization](../../../../../memoization.md), and [dynamic programming](../../../../../dynamic-programming.md) need not be implemented iteratively. For optimization, the [dynamic programming state](../../../../../dynamic-programming-state.md) and [optimal substructure](../../../../../optimal-substructure.md) justify combining stored optimum values; storing repeated work alone does not prove the state is sufficient.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [6](../../6.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
