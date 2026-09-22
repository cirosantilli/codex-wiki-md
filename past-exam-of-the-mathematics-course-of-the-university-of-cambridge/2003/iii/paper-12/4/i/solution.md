<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

We first establish the [labelled forest count with prescribed roots](../../../../../../labelled-forest-count-with-prescribed-roots.md). For a prescribed root set $R$ of size $k<n$, orient each [tree](../../../../../../tree-graph-theory.md) toward its unique root. Repeatedly delete the smallest remaining nonroot leaf, recording its parent. There are $n-k$ deletions, and the final recorded parent belongs to $R$. Conversely, start with any code of length $n-k$ whose last entry lies in $R$. At each step select the smallest remaining nonroot absent from the remaining code, connect it to the code's first entry, and delete that vertex and entry. Such a vertex exists: among $s$ remaining nonroots, the remaining code has $s$ entries but at least its last entry is a root, so at most $s-1$ nonroots occur in it. Previously deleted vertices never recur in the code, so the selected parent is still present. Every edge goes from a vertex being deleted to one retained, excluding a cycle. The resulting forest has one root in each [graph component](../../../../../../component-graph-theory.md), and the two constructions are inverse. Its count is therefore

$$
F(n,k)=kn^{n-k-1};
$$

for $k=n$, interpret this as one, the empty [forest](../../../../../../forest.md).

A connected [simple graph](../../../../../../simple-graph.md) with $n$ edges has exactly one cycle: a [spanning tree](../../../../../../spanning-tree.md) uses $n-1$ edges, and the remaining edge creates its unique cycle. If that [graph cycle](../../../../../../cycle-in-a-graph.md) has length $k$, choose its vertex set in $\binom nk$ ways and its unoriented cyclic order in $(k-1)!/2$ ways. All other edges form a forest rooted at those $k$ vertices, with exactly one cycle vertex per forest component; two roots in one attached component would create an additional cycle. Conversely every such cycle and rooted forest gives a unique [unicyclic component](../../../../../../unicyclic-component.md). Thus

$$
\begin{aligned}
C(n,n)&=\sum_{k=3}^n\binom nk\frac{(k-1)!}{2}\,kn^{n-k-1}\\
&=\frac{(n-1)!}{2}\sum_{k=3}^n\frac{n^{n-k}}{(n-k)!}
=\boxed{\frac{(n-1)!}{2}\sum_{j=0}^{n-3}\frac{n^j}{j!}}.
\end{aligned}
$$

This is the [labelled unicyclic graph count](../../../../../../labelled-unicyclic-graph-count.md). The term $k=n$ correctly counts a cycle with no attached nonroot vertices.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 12](../../../paper-12-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
