<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Run [depth-first search](../../../../../depth-first-search.md) on [Graph](../../../../../graph-split.md) B with the same lexical convention and put each [vertex](../../../../../vertex-graph-theory.md) on the front of the output when its search finishes. The finish order is

$$
4,6,7,5,2,1,3,
$$

so the returned [topological order](../../../../../topological-order.md) is

$$
\boxed{3,1,2,5,7,6,4.}
$$

For example, both [edges](../../../../../edge-of-a-graph.md) from $1$ point to later entries, the [edges](../../../../../edge-of-a-graph.md) from $5$ point to $4$ and $7$ later in the order, and $3$ precedes $6$. The construction is valid because in a [Directed acyclic graph](../../../../../directed-acyclic-graph.md) every [edge](../../../../../edge-of-a-graph.md) $u\to v$ has $f(u)>f(v)$: a newly found descendant finishes before its caller, and an already finished neighbour also has a smaller finish time; an active ancestor would instead witness a [directed cycle](../../../../../directed-cycle.md). Thus reversing the finish order puts every prerequisite before its successor. The time is $O(|V|+|E|)$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [7](../../7.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
