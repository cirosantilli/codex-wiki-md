<h1 id="7/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Assume throughout (c) that the [graph](../../../../../graph-split.md) is finite and connected, as needed for the asserted spanning [trees](../../../../../tree-graph-theory-split.md). List its [edge](../../../../../edge-of-a-graph.md) weights as $w_1<\cdots<w_m$. The stated separation implies $w_{j+1}>2w_j$, so for every $k$,

$$
\sum_{j<k}w_j<w_k\sum_{r=1}^{k-1}2^{-r}<w_k.
$$

Thus the weights form a [superincreasing sequence](../../../../../superincreasing-sequence.md). If $A,B$ are distinct [edge](../../../../../edge-of-a-graph.md) sets, let $e$ be the heaviest [edge](../../../../../edge-of-a-graph.md) in their [symmetric difference](../../../../../symmetric-difference.md). Suppose $e\in A$. All other uncancelled [edges](../../../../../edge-of-a-graph.md) are lighter, so

$$
\sum_{a\in A}w(a)-\sum_{b\in B}w(b)\ge w(e)-\sum_{w(f)<w(e)}w(f)>0.
$$

Therefore different [edge](../../../../../edge-of-a-graph.md) sets have different total costs. In particular all distinct [spanning trees](../../../../../spanning-tree.md) have different costs. Since a finite [connected graph](../../../../../connected-graph.md) has at least one [spanning tree](../../../../../spanning-tree.md) and only finitely many choices,

$$
\boxed{\text{the minimum spanning tree exists and is unique}.}
$$

This domination of every collection of smaller [edges](../../../../../edge-of-a-graph.md) will also be used in (iii).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [7](../../../7.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the short options course of the University of Oxford](../../../../split.md)
6. [Short options course of the University of Oxford](../../../../../short-options-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
