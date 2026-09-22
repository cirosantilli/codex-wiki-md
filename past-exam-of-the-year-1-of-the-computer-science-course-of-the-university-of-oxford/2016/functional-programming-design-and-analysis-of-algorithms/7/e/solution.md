<h1 id="7/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Use an [indexed priority queue](../../../../../indexed-priority-queue.md) of unsettled [vertices](../../../../../vertex-graph-theory.md), keyed by their [tentative distances](../../../../../tentative-distance.md). Initialize the source to zero and other keys to $+\infty$. Each `ExtractMin` settles the currently closest [vertex](../../../../../vertex-graph-theory.md). Scan its outgoing edges; whenever [edge relaxation](../../../../../edge-relaxation.md) improves a neighbour's [tentative distance](../../../../../tentative-distance.md), update that neighbour with `DecreaseKey`. Already settled [vertices](../../../../../vertex-graph-theory.md) need no further update, by the correctness of [Dijkstra's algorithm](../../../../../dijkstra-algorithm.md) for nonnegative weights.

There are at most $|V|$ extractions and at most $|E|$ successful decreases. The [indexed priority queue](../../../../../indexed-priority-queue.md) maintains each [vertex](../../../../../vertex-graph-theory.md)'s current array position and updates this index table on every swap, so locating a key for `DecreaseKey` costs $O(1)$. Preallocate capacity $|V|$. Repeated insertion costs $O(|V|(1+\log_d|V|))$, or [bottom-up heap construction](../../../../../bottom-up-heap-construction.md) initializes the queue in $O(|V|)$ time. Scanning [adjacency lists](../../../../../adjacency-list.md) costs $O(|V|+|E|)$ in total.

For $|V|\geq2$ and $2\leq d\leq|V|$, the heap-operation contributions are therefore

$$
O(|V|d\log_d|V|)\quad\text{and}\quad O(|E|\log_d|V|),
$$

and the overall bound is

$$
\boxed{O\!\left((d|V|+|E|)\log_d|V|\right)}.
$$

A uniform bound including larger arity and tiny graphs is $O((d|V|+|E|)(1+\log_d(\max(2,|V|))))$. Arity greater than the number of [vertices](../../../../../vertex-graph-theory.md) offers no useful extra heap levels. These bounds assume [adjacency lists](../../../../../adjacency-list.md); with an [adjacency matrix](../../../../../adjacency-matrix.md), scanning neighbours contributes $O(|V|^2)$ instead. No rebuilding of the heap is required after each decrease.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [7](../../7.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
