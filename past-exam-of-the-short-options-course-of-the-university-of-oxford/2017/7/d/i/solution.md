<h1 id="7/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $d(u)$ be the weight of a shortest $vu$-path, and let $p(u)$ be the predecessor of $u$ on the chosen $P_u$. Its prefix to $p(u)$ must also be shortest: a cheaper prefix followed by the final edge would give a cheaper walk to $u$, and [cycle erasure in minimum-weight walks](../../../../../cycle-erasure-in-minimum-weight-walks.md) would produce a cheaper path because every edge weight is positive. Therefore

$$
d(u)=d(p(u))+w(e_u)>d(p(u)).
$$

Following predecessor arrows strictly decreases $d$, so cannot revisit a vertex. Since each nonroot vertex has a predecessor, finiteness forces every predecessor chain to end at $v$. Thus $T$ is connected.

The edges $e_u$ are distinct: if two vertices selected the same undirected edge, each would be the other's predecessor, contradicting strict decrease. Hence $T$ has exactly $|V(G)|-1$ edges. A finite connected graph with this edge count is a tree. This proves that [positive-weight shortest-path predecessors form a tree](../../../../../positive-weight-shortest-path-predecessors-form-a-tree.md), without requiring the initially chosen paths to be mutually consistent.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [D](../../d.md)
3. [7](../../../7.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the short options course of the University of Oxford](../../../../split.md)
6. [Short options course of the University of Oxford](../../../../../short-options-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
