<h1 id="8/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Assume the graph is connected so that a [minimum spanning tree](../../../../../minimum-spanning-tree.md) exists, and let $T$ be the output of [Kruskal's algorithm](../../../../../kruskal-s-algorithm.md). With distinct weights there is a strict total [edge](../../../../../edge-of-a-graph.md) ordering. Suppose another [minimum spanning tree](../../../../../minimum-spanning-tree.md) $T'\ne T$ existed. Choose $e\in T\setminus T'$ and increase only $w(e)$ by a positive $\varepsilon$ so small that the strict ordering of _all_ [edge](../../../../../edge-of-a-graph.md) weights remains unchanged. For a finite graph such an $\varepsilon$ exists, using less than the gap to the next larger weight; if $e$ is largest, any sufficiently small positive increase works.

Running [Kruskal's algorithm](../../../../../kruskal-s-algorithm.md) again examines exactly the same order and makes exactly the same component decisions. It therefore still returns $T$, which must remain optimal for the perturbed weights. But $T$ has become more expensive by $\varepsilon$, while $T'$ is unchanged. They had equal original weight, so now $T'$ is cheaper, a contradiction. This proves that [distinct weights imply a unique minimum spanning tree](../../../../../distinct-weights-imply-a-unique-minimum-spanning-tree.md).

The converse is **false**. A triangle with [edge](../../../../../edge-of-a-graph.md) weights $1,1,2$ has a unique [minimum spanning tree](../../../../../minimum-spanning-tree.md), consisting of its two weight-one [edges](../../../../../edge-of-a-graph.md). Its total is $2$, while either other spanning tree has total $3$. Thus equal [edge](../../../../../edge-of-a-graph.md) weights permit, but do not force, multiple optimum trees. The same perturbation proof applies componentwise to a [minimum spanning forest](../../../../../minimum-spanning-forest.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [8](../../8.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
