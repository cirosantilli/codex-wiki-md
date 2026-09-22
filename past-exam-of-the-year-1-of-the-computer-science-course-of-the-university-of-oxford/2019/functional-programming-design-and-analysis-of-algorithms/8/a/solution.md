<h1 id="8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Initialize $d[s]=0$ and $d[v]=\infty$ elsewhere. Perform $|V|-1$ full passes over the directed [edges](../../../../../edge-of-a-graph.md), applying [edge relaxation](../../../../../edge-relaxation.md) $d[v]\gets\min\{d[v],d[u]+w(u,v)\}$ whenever $d[u]$ is finite. For an [undirected graph](../../../../../undirected-graph.md), process each [edge](../../../../../edge-of-a-graph.md) in both directions. Stop early if a pass makes no change.

Each finite label records the cost of a discovered [directed walk](../../../../../directed-walk.md), so it never understates the true infimum. After $t$ passes, relaxation has propagated along every route of at most $t$ [edges](../../../../../edge-of-a-graph.md), so the label is no greater than the cost of any such route. If no reachable negative-cost closed walk exists, an optimal route can be chosen without repeated [vertices](../../../../../vertex-graph-theory.md) and has at most $|V|-1$ [edges](../../../../../edge-of-a-graph.md). These inequalities prove that the final labels are the desired [shortest path](../../../../../shortest-path.md) lengths.

An additional pass checks for an improving [edge](../../../../../edge-of-a-graph.md) from a reachable [vertex](../../../../../vertex-graph-theory.md). If one exists, report a reachable negative-cost cycle: finite shortest distances cannot be assigned to [vertices](../../../../../vertex-graph-theory.md) reachable from that cycle. Mark those [vertices](../../../../../vertex-graph-theory.md) by forward reachability if individual $-\infty$ answers are wanted. In particular, a reachable negative undirected [edge](../../../../../edge-of-a-graph.md) becomes a negative two-arc closed walk under the bidirected interpretation; generic signed weights do not guarantee finite answers.

Each pass costs $O(|E|)$, giving **$O(|V||E|)$** for the usual [Bellman-Ford algorithm](../../../../../bellman-ford-algorithm.md) bound. Including initialization gives $O(|V|+|V||E|)$, which also handles an edgeless [graph](../../../../../graph-split.md) honestly; these coincide in order when $|E|\ge1$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [8](../../8.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
