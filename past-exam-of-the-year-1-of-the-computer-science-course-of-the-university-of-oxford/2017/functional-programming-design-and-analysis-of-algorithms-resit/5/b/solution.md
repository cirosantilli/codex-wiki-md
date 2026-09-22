<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Every finite distance label is the weight of a discovered [directed walk](../../../../../directed-walk.md), so it can never underestimate a finite shortest-path distance. After $k$ complete passes, each label is at most the cost of every source-to-vertex path using at most $k$ edges. To prove that assertion, consider such a path's last edge $u\to v$: after the previous pass, $u$ already has a label no greater than the prefix cost, and the current pass relaxes that last edge. In-place improvements can only make the label smaller, preserving the assertion.

When no negative-weight cycle is reachable, any repeated-vertex portion of an optimal walk can be removed without increasing its cost. Some shortest path therefore has at most $|V|-1$ edges. The two bounds meet after that many passes, proving correctness. If a complete pass makes no change, all [edge relaxation](../../../../../edge-relaxation.md) inequalities already hold and further passes cannot improve anything. A further strict relaxation after $|V|-1$ passes implies a reachable negative cycle by the same simple-path bound.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
