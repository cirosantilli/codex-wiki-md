<h1 id="8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use [Kahn's algorithm](../../../../../kahn-s-algorithm.md) for [topological sorting](../../../../../topological-sorting.md). With an [adjacency list](../../../../../adjacency-list.md) representation, count every [vertex](../../../../../vertex-graph-theory.md)'s [indegree](../../../../../indegree.md) by scanning the [edges](../../../../../edge-of-a-graph.md). Put all zero-[indegree](../../../../../indegree.md) [vertices](../../../../../vertex-graph-theory.md) in a [queue](../../../../../queue-queueing-theory.md). Repeatedly remove one such [vertex](../../../../../vertex-graph-theory.md) $u$, append it to the output, and delete its outgoing [edges](../../../../../edge-of-a-graph.md) by decrementing the stored [indegree](../../../../../indegree.md) of each neighbour; enqueue a neighbour exactly when its count becomes zero.

The [loop invariant](../../../../../loop-invariant.md) is that stored counts are the [indegrees](../../../../../indegree.md) in the unreported subgraph and the [queue](../../../../../queue-queueing-theory.md) contains exactly its unreported zero-[indegree](../../../../../indegree.md) [vertices](../../../../../vertex-graph-theory.md). A nonempty finite [Directed acyclic graph](../../../../../directed-acyclic-graph.md) always has such a [vertex](../../../../../vertex-graph-theory.md): otherwise following incoming [edges](../../../../../edge-of-a-graph.md) would eventually repeat a [vertex](../../../../../vertex-graph-theory.md), creating a directed [graph cycle](../../../../../cycle-in-a-graph.md). Thus the [queue](../../../../../queue-queueing-theory.md) cannot become empty while any [vertex](../../../../../vertex-graph-theory.md) remains.

For every original [edge](../../../../../edge-of-a-graph.md) $u\to v$, $v$ cannot enter the output until that [edge](../../../../../edge-of-a-graph.md) has been removed by outputting $u$. Therefore

$$
\boxed{u\to v\implies\operatorname{position}(u)<\operatorname{position}(v).}
$$

Each [vertex](../../../../../vertex-graph-theory.md) enters and leaves the [queue](../../../../../queue-queueing-theory.md) once, and every [edge](../../../../../edge-of-a-graph.md) is scanned a constant number of times, giving $\boxed{\Theta(|V|+|E|)}$ time and $O(|V|)$ auxiliary space beyond the [adjacency lists](../../../../../adjacency-list.md). If given only an [adjacency matrix](../../../../../adjacency-matrix.md), scanning neighbours instead takes $\Theta(|V|^2)$ time.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [8](../../8.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
