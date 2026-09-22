<h1 id="7/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

First run [breadth-first search](../../../../../../breadth-first-search.md) from $s$ to compute each distance $D(v)$. All are finite by hypothesis. Next compute the [strongly connected components](../../../../../../strongly-connected-component.md) and their [condensation graph](../../../../../../condensation-graph.md) $H$. For every component $C$, initialize a representative $b(C)$ minimizing $D(v)$ over $v\in C$. Process components in reverse [topological order](../../../../../../topological-order.md), using

$$
b(C)=\operatorname*{arg\,min}_{x\in\{b(C)\}\cup\{b(B):C\to B\text{ in }H\}}D(x).
$$

Break equal-distance ties consistently, for example by fixed vertex index. Return $b(C)$ for every $u\in C$.

Every [vertex](../../../../../../vertex-graph-theory.md) of one [strongly connected component](../../../../../../strongly-connected-component.md) reaches every other; every reachable different component is reached through some first outgoing [edge](../../../../../../edge-of-a-graph.md) of $H$. Since $H$ is a [Directed acyclic graph](../../../../../../directed-acyclic-graph.md), reverse [topological order](../../../../../../topological-order.md) has already solved every successor. [Induction](../../../../../../mathematical-induction.md) over that order proves that the representative minimizes $D$ over all reachable [vertices](../../../../../../vertex-graph-theory.md). This is [minimum reachable label propagation](../../../../../../minimum-reachable-label-propagation.md).

All stages take **$O(|V|+|E|)$ time** and $O(|V|+|E|)$ space with explicit [adjacency lists](../../../../../../adjacency-list.md). Retaining parallel component edges is harmless: they can be scanned once each without sorting or deduplication. Reachability here includes the length-zero path, so $u\in P(u)$; this standard convention also makes the requested answer meaningful at a sink.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [7](../../../7.md)
4. [Functional programming, design and analysis of algorithms](../../../../functional-programming-design-and-analysis-of-algorithms-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
