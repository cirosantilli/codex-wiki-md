<h1 id="7/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $T$ be the unique [minimum spanning tree](../../../../../minimum-spanning-tree.md). If $e=ab$ is an [edge](../../../../../edge-of-a-graph.md) outside $T$, adding it creates a unique [graph cycle](../../../../../cycle-in-a-graph.md) consisting of $e$ and the [tree](../../../../../tree-graph-theory-split.md) [graph path](../../../../../path-in-a-graph.md) $P_T(a,b)$. Every [edge](../../../../../edge-of-a-graph.md) $f$ on that [graph path](../../../../../path-in-a-graph.md) has $w(f)<w(e)$: otherwise the distinct weights would give $w(f)>w(e)$, and replacing $f$ by $e$ would produce a cheaper [spanning tree](../../../../../spanning-tree.md). This is the [minimum spanning tree cycle property](../../../../../minimum-spanning-tree-cycle-property.md) in exchange form.

By the domination inequality in (i), it follows more strongly that

$$
\boxed{w(P_T(a,b))<w(e).}
$$

Now consider any simple [graph path](../../../../../path-in-a-graph.md) $P$ from $v$ to $u$ that is not the [tree](../../../../../tree-graph-theory-split.md) [graph path](../../../../../path-in-a-graph.md). It must use an [edge](../../../../../edge-of-a-graph.md) outside $T$. Replace every such [edge](../../../../../edge-of-a-graph.md) by the corresponding [tree](../../../../../tree-graph-theory-split.md) [graph path](../../../../../path-in-a-graph.md). Each replacement strictly reduces length and produces a walk entirely in $T$. Removing any repeated-vertex excursions leaves the unique [tree](../../../../../tree-graph-theory-split.md) [graph path](../../../../../path-in-a-graph.md) $P_T(v,u)$ and can only reduce length further. Therefore

$$
w(P_T(v,u))<w(P).
$$

So every root-to-vertex [graph path](../../../../../path-in-a-graph.md) in $T$ is the unique shortest [graph path](../../../../../path-in-a-graph.md) in $G$, and

$$
\boxed{T_{\mathrm{MST}}=T_{\mathrm{shortest},v}.}
$$

The argument works for every choice of root $v$.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
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
