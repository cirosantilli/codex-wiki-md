# Counting lemma for octahedrally quasirandom three-uniform hypergraphs

↑ **Parent:** [Octahedral quasirandomness of a three-uniform hypergraph](octahedral-quasirandomness-of-a-three-uniform-hypergraph.md)

Let a fixed simple three-[uniform hypergraph](uniform-hypergraph.md) $F$ have $m$ [hypergraph edges](edge-of-a-hypergraph.md), with one host [vertex of a hypergraph](vertex-of-a-hypergraph.md) class $V_i$ for each [vertex of a hypergraph](vertex-of-a-hypergraph.md). Assume each [hypergraph edge](edge-of-a-hypergraph.md) triple has indicator $h_e$, [subset density](density-of-a-finite-subset.md) $p_e$, and balanced [three-dimensional box norm](three-dimensional-box-norm.md) at most $\alpha^{1/8}$. The normalized [labelled hypergraph copy count](labelled-hypergraph-copy-count.md) is $\mathbb E\prod_{e\in E(F)}h_e$. Telescope this product against $\prod_ep_e$. In each error term, fix all variables outside the three [vertices of a hypergraph](vertex-of-a-hypergraph.md) of its balanced [hypergraph edge](edge-of-a-hypergraph.md). Every other [hypergraph edge](edge-of-a-hypergraph.md) intersects that triple in at most two [vertices of a hypergraph](vertex-of-a-hypergraph.md), so the remaining factors group into three pair [functions](function-split.md) bounded by one. The [pair-factor correlation bound for the three-dimensional box norm](pair-factor-correlation-bound-for-the-three-dimensional-box-norm.md) bounds the error by $\alpha^{1/8}$. Summing gives

$$
\left|\#F-\left(\prod_ep_e\right)\left(\prod_i|V_i|\right)\right|\leq m\alpha^{1/8}\prod_i|V_i|.
$$

For the [three-uniform tetrahedron](three-uniform-tetrahedron.md), $m=4$. The same argument with a common host [set](set-split.md) counts homomorphisms; excluding collisions of distinct abstract [vertices of a hypergraph](vertex-of-a-hypergraph.md) changes the count by at most $\binom{|V(F)|}{2}|V|^{|V(F)|-1}$.

## ↑ Ancestors (8)

1. [Octahedral quasirandomness of a three-uniform hypergraph](octahedral-quasirandomness-of-a-three-uniform-hypergraph.md)
2. [Uniform hypergraph](uniform-hypergraph.md)
3. [Hypergraph](hypergraph-split.md)
4. [Graph theory](graph-theory-split.md)
5. [Foundations of mathematics](foundations-of-mathematics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Labelled hypergraph copy count](labelled-hypergraph-copy-count.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-88/4/iii/solution.md)
