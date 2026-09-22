<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

An infinite trace exists **exactly when a directed cycle is reachable from $s$**, by the [infinite walk criterion in a finite directed graph](../../../../../infinite-walk-criterion-in-a-finite-directed-graph.md). Compute the reachable set with [depth-first search](../../../../../depth-first-search.md), compute its [strongly connected components](../../../../../strongly-connected-component.md), and return true if any component has at least two vertices or contains a self-loop. A singleton without a self-loop does not qualify.

If the test succeeds, follow a path from $s$ to the cycle and traverse the cycle forever. Conversely, an infinite trace in a finite graph repeats a vertex, producing a reachable nonempty closed walk and hence a directed cycle. Reachability, component construction and the self-loop check all scan [adjacency lists](../../../../../adjacency-list.md) only a constant number of times. The worst-case time is **$O(|V|+|E|)$**, with $O(|V|+|E|)$ auxiliary space for a straightforward transpose-based implementation.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [6](../../6.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
