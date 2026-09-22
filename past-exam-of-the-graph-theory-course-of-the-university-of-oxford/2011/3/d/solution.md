<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Choose a small density threshold $d>0$, then $\varepsilon\leq\min(d/2,1/4)$ sufficiently small and a lower partition bound $m_0$ sufficiently large that

$$
2\varepsilon+\frac1{2m_0}+\frac d2<\eta.
$$

Apply the regularity lemma. Delete all [edges](../../../../edge-of-a-graph.md) incident with $V_0$, all [edges](../../../../edge-of-a-graph.md) within a class $V_i$, all [edges](../../../../edge-of-a-graph.md) between [irregular pairs](../../../../irregular-pair-of-vertex-sets.md), and all [edges](../../../../edge-of-a-graph.md) between [regular pairs](../../../../regular-pair-of-vertex-sets.md) of density below $d$. Their total is at most

$$
\varepsilon n^2+\frac{n^2}{2k}+\varepsilon n^2+\frac d2 n^2<\eta n^2.
$$

If a [triangle](../../../../triangle-in-a-graph.md) remains, its [vertices](../../../../vertex-graph-theory.md) lie in three distinct nonexceptional classes, all whose pairs were regular with original density at least $d$. Part (c) then forces at least $(d^3/16)t^3$ [triangles](../../../../triangle-in-a-graph.md) in the original [graph](../../../../graph-split.md), where $t$ is the common class size. Since $k\leq M$ and $\varepsilon\leq1/4$, we have $t\geq n/(2M)$, so this is at least $d^3n^3/(128M^3)$.

Choose $c=d^3/(256M^3)$ and take $n_0$ large enough for the regularity lemma. An original [graph](../../../../graph-split.md) with at most $cn^3$ [triangles](../../../../triangle-in-a-graph.md) cannot leave any [triangle](../../../../triangle-in-a-graph.md) after these deletions. Thus **deleting at most $\eta n^2$ [edges](../../../../edge-of-a-graph.md) makes the [graph](../../../../graph-split.md) triangle-free**. This is the [triangle removal lemma](../../../../triangle-removal-lemma.md); boundedly many large regular clusters turn any surviving [triangle](../../../../triangle-in-a-graph.md) into a positive-density family of original [triangles](../../../../triangle-in-a-graph.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the graph theory course of the University of Oxford](../../../split.md)
5. [Graph theory course of the University of Oxford](../../../../graph-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
