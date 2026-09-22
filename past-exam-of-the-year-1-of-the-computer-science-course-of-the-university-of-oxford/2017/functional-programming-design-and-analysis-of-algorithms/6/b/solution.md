<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Apply the [two-pass strongly connected component algorithm](../../../../../two-pass-strongly-connected-component-algorithm.md):

1. Run [depth-first search](../../../../../depth-first-search.md) over all vertices of $G$, recording their finish order.  
2. Construct the [graph transpose](../../../../../graph-transpose.md) by reversing every edge.  
3. Mark every vertex unvisited again. In decreasing first-pass finish order, start a transpose search whenever the next vertex is unvisited. The vertices newly reached by each search form one [strongly connected component](../../../../../strongly-connected-component.md).

The finish order prevents a second-pass search from entering a different still-unassigned component, while mutual reachability makes it visit the entire current component. With [adjacency lists](../../../../../adjacency-list.md), each traversal and the transposition scan takes $O(|V|+|E|)$ time. Thus the total worst-case time is **$\Theta(|V|+|E|)$**, including isolated vertices.

## ↑ Ancestors (12)

1. [B](../b.md)
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
