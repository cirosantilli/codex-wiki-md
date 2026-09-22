<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [two-pass strongly connected component algorithm](../../../../../two-pass-strongly-connected-component-algorithm.md): first run [depth-first search](../../../../../depth-first-search.md) on the original [directed graph](../../../../../directed-graph.md), then search its [graph transpose](../../../../../graph-transpose.md) in decreasing order of the first pass's finishing times. The first-pass order from part (a) is

$$
3,1,2,5,7,6,4.
$$

Reversing the [edges](../../../../../edge-of-a-graph.md) gives outgoing [adjacency lists](../../../../../adjacency-list.md)

$$
1:(4),\quad2:(1),\quad3:(),\quad4:(7),\quad5:(2,4),\quad6:(2,3,7),\quad7:(5).
$$

The second pass first visits only $3$. Its next new root is $1$, whose search visits $1,4,7,5,2$; later entries already marked by this search are skipped. The next new root is $6$, whose [graph transpose](../../../../../graph-transpose.md) neighbours have already been assigned. Therefore the components are

$$
\boxed{\{3\},\qquad\{1,2,4,5,7\},\qquad\{6\}.}
$$

Within the middle component the [directed cycle](../../../../../directed-cycle.md) $1\to2\to5\to7\to4\to1$ demonstrates mutual reachability. The source [edge](../../../../../edge-of-a-graph.md) structure does not provide return paths from $6$ or to $3$. More generally, decreasing finish order chooses a remaining component whose [graph transpose](../../../../../graph-transpose.md) search cannot escape to another still-unassigned component, so each second-pass tree is exactly one component. This explains the partition rather than merely listing it. The [algorithm](../../../../../algorithm-split.md) takes $O(|V|+|E|)$ with [adjacency lists](../../../../../adjacency-list.md).[§§6.5–6.6, strong components, condensation and the two-search construction](../../../../../depth-first-search-by-jeff-erickson.md)

## ↑ Ancestors (12)

1. [B](../b.md)
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
