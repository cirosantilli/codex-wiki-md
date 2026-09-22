<h1 id="r/r2/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Suppose a [graph](../../../../../../graph-split.md) satisfying [Ore's theorem](../../../../../../ore-s-theorem.md) were not Hamiltonian. Extend it, on the same vertices, to an [edge](../../../../../../edge-of-a-graph.md)-maximal non-[Hamiltonian graph](../../../../../../hamiltonian-graph.md) $H$. Adding edges preserves the degree-sum hypothesis. The [complete graph](../../../../../../complete-graph.md) is Hamiltonian, so $H$ has a missing [edge](../../../../../../edge-of-a-graph.md) $uv$. By maximality, $H+uv$ has a [Hamiltonian cycle](../../../../../../hamilton-cycle.md), which must use the new [edge](../../../../../../edge-of-a-graph.md). Removing it gives a [Hamiltonian path](../../../../../../hamiltonian-path.md) in $H$, labelled $u=v_1,v_2,\ldots,v_n=v$.

If some $i$ has both edges $uv_{i+1}$ and $vv_i$, the path can be closed into the cycle

$$
v_1,v_2,\ldots,v_i,v_n,v_{n-1},\ldots,v_{i+1},v_1,
$$

contradicting the choice of $H$. Thus the index sets $\{i:uv_{i+1}\in E(H)\}$ and $\{i:vv_i\in E(H)\}$ are disjoint subsets of $\{1,\ldots,n-1\}$. Their sizes are $\deg_Hu$ and $\deg_Hv$. Consequently $\deg_Hu+\deg_Hv\leq n-1$, contradicting the degree-sum condition for the nonadjacent pair $u,v$. Hence the original [graph](../../../../../../graph-split.md) is Hamiltonian.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [A](../../a.md)
3. [R2](../../../r2.md)
4. [R](../../../../r.md)
5. [2011](../../../../../2011-split.md)
6. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../../split.md)
7. [Probability, statistics and options II course of the University of Oxford](../../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Mathematics and statistics course of the University of Oxford](../../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
