<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take the [directed graph](../../../../../directed-graph.md) with source $1$ and weighted [edges](../../../../../edge-of-a-graph.md)

$$
1\to2:2,\qquad1\to3:5,\qquad3\to2:-4,\qquad2\to4:1.
$$

It is a [Directed acyclic graph](../../../../../directed-acyclic-graph.md), so has no negative-weight [graph cycle](../../../../../cycle-in-a-graph.md). The true [shortest path](../../../../../shortest-path.md) to $4$ is $1\to3\to2\to4$, of weight $5-4+1=2$.

The standard [label-setting shortest-path algorithm](../../../../../label-setting-shortest-path-algorithm.md) version of the [Dijkstra algorithm](../../../../../dijkstra-algorithm.md) extracts $1$, then $2$ at distance $2$, then $4$ at distance $3$, and only then $3$ at distance $5$. Thus it finalises **$d[4]=3$ instead of $2$**. Even if an implementation subsequently changes the stored label of the already settled vertex $2$, it does not reprocess its outgoing edge to $4$, so the error at $4$ remains. Allowing repeated reprocessing would instead be a [label-correcting shortest-path algorithm](../../../../../label-correcting-shortest-path-algorithm.md), not the usual Dijkstra guarantee.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2023](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
